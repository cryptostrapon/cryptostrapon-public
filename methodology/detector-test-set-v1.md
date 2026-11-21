# Scam detector test set v1

100 inputs we use to test every release of the CryptoStrapon scam detector: 40 legitimate, 20 gray (risky but not proven fraud) and 40 scam. Each one has the band we expect. The same data is in [detector-test-set-v1.csv](detector-test-set-v1.csv).

We publish it because a detector that only reports its own accuracy is hard to trust. Anyone can run these inputs through our detector, or through any other tool, and compare.

## Score bands

| Band | Score | Label |
|---|---|---|
| Low | 0 to 30 | No clear red flags found |
| Caution | 31 to 69 | Caution: review the risks |
| High | 70 to 89 | High risk: this looks like a scam |
| Scam | 90 to 100 | Scam detected |

A result passes if it lands in the expected band. For section C, High or Scam both pass.

## Notes before you use it

- Brand names (Ledger, MetaMask, Binance, Coinbase and others) appear only as examples of real notification styles or of what scammers imitate. Nothing here says these companies did anything wrong.
- Domains in section C are invented for the test and are written as plain text. Some may exist or be registered later. Do not visit them.
- S40 is the address publicly attributed to the February 2025 Bybit exploit.
- Real messages are often longer and messier. This set is a floor, not a full benchmark.

## A. Legitimate (expected: Low)

| ID | Type | Input |
|---|---|---|
| L01 | chat | gm! Gas is under 5 gwei today, good time to move my savings to my hardware wallet. |
| L02 | chat | Can you send me your ETH address? I'll pay you back the 50 for dinner. |
| L03 | event | Devconnect tickets are on sale on devconnect.org. See you there! |
| L04 | exchange notice | Your withdrawal of 0.05 ETH has been completed. If you did not make this request, open the app and go to Security. |
| L05 | exchange notice | New sign-in to your account from Chrome on Windows. If this was you, no action is needed. |
| L06 | exchange notice | Your identity verification is complete. You can now deposit and trade. |
| L07 | exchange notice | Scheduled maintenance: deposits on the TRON network will be paused for 30 minutes at 02:00 UTC. |
| L08 | wallet notice | MetaMask: a new version is available. Update from the Chrome Web Store or your extension settings. |
| L09 | wallet notice | Your Trezor firmware update is available in Trezor Suite. Never share your recovery seed with anyone. |
| L10 | security tip | Reminder from our support team: we will never ask for your password, 2FA codes or recovery phrase. |
| L11 | developer | PR merged: fix(parser) handle npm-shrinkwrap.json. Thanks for the contribution! |
| L12 | developer | Your npm package was published: my-lib@1.4.2 |
| L13 | developer | GitHub: a new SSH key was added to your account. If you did not add it, remove it in Settings. |
| L14 | news | Ethereum's next upgrade is scheduled for testnets next month, according to the core developers call. |
| L15 | news | Bitcoin hashrate hit a new high this week, data from mempool.space shows. |
| L16 | URL | https://etherscan.io |
| L17 | URL | https://ethereum.org/en/wallets/ |
| L18 | URL | https://github.com/bitcoin/bitcoin |
| L19 | URL | https://www.coinbase.com |
| L20 | URL | https://metamask.io |
| L21 | URL | https://revoke.cash |
| L22 | URL | https://app.uniswap.org |
| L23 | URL | https://www.ledger.com |
| L24 | URL | https://trezor.io |
| L25 | payment | Invoice #2041 for website design: 1,200 USDC on Base. Payment address is in the signed contract we both have. |
| L26 | family | Mum, I sent you the guide on how to check a link before clicking it. Call me if anything looks odd. |
| L27 | job | Thanks for applying to the Senior Solidity role. Our recruiter will email you from @ourcompany.com to schedule a video call. |
| L28 | job | The take-home task is a small React app. Please run it in a container or VM; there are no install scripts. |
| L29 | DAO | Governance vote 42 is open until Friday. Read the proposal on the forum before voting. |
| L30 | airdrop real style | The airdrop eligibility checker is live on the official site linked from our verified X account. We will never DM you. |
| L31 | support real style | We received your ticket #58213. An agent will reply here in the app. Do not share your seed phrase with anyone. |
| L32 | bank | Your card ending 4421 was used at an ATM. If this was not you, call the number on the back of your card. |
| L33 | friend | I lost money on a meme coin last week, lesson learned. Only buying BTC now. |
| L34 | education | A seed phrase is 12 or 24 words that back up your wallet. Anyone who has it controls the funds. |
| L35 | education | Address poisoning sends you a tiny transfer from an address that looks like one you used. Always copy from your contact list. |
| L36 | marketplace | Your NFT sold on OpenSea for 0.2 ETH. Proceeds are in your wallet. |
| L37 | podcast | New episode: how hardware wallet supply chains work, with a security researcher. |
| L38 | address | 0xd8dA6BF26964aF9D7eEd9e03E53415D37aA96045 (well known public ENS owner address) |
| L39 | address | 0xA0b86991c6218b36c1d19D4a2e9Eb0cE3606eB48 (USDC on Ethereum) |
| L40 | address | TR7NHqjeKQxGTCi8q8ZY4pL8otSzgjLj6t (USDT on TRON) |

## B. Gray (expected: Caution)

| ID | Type | Input |
|---|---|---|
| G01 | presale | New presale! $MOON launches tomorrow, 100x potential, early buyers get 20% bonus. Join t.me/moonpresale_official |
| G02 | mentor | I trade crypto full time and help beginners. 3 free lessons, then a small fee if you like it. DM me. |
| G03 | signals | VIP signals group, 85% win rate last month, $49 a month, results in the pinned post. |
| G04 | memecoin | Dev is doxxed, liquidity locked for 30 days, launching on pump.fun tonight. |
| G05 | yield | Our DeFi vault pays 24% APY in stablecoins. Audited, see the report on our docs. |
| G06 | OTC | I can sell you USDT below market for cash in person, my usual rate is 0.97. |
| G07 | giveaway | Retweet and follow for a chance to win 0.1 ETH, winner announced Friday. |
| G08 | bot | Our trading bot is free to try, connect read-only API keys from your exchange. |
| G09 | job | We pay $3,000 a month for remote community moderators. Payment in USDT. Interview on Telegram. |
| G10 | P2P | Selling USDT P2P, I only accept bank transfer from an account in your name. |
| G11 | NFT | Free mint for our new collection, gas only, link in bio. |
| G12 | airdrop farming | Points program is live: bridge to our new L2 and do 5 swaps a week to qualify. |
| G13 | recovery talk | Lost access to your wallet? A locksmith style service can try to brute force your own password if you remember most of it. |
| G14 | influencer | This coin will 10x by Christmas, not financial advice. |
| G15 | loan | Crypto-backed loan, 12% APR, deposit BTC as collateral, instant approval. |
| G16 | cloud mining | Cloud mining contract, 1 TH/s for $99, payouts daily. |
| G17 | referral | Use my referral code to get a $50 bonus when you deposit $100. |
| G18 | token sale | Private round for our project, minimum $5,000, SAFT available on request. |
| G19 | arbitrage | I make 2% a day doing arbitrage between two exchanges, want me to teach you? |
| G20 | wallet app | Try our new wallet app, not on the App Store yet, download the APK from our site. |

## C. Scam (expected: High or Scam; most should be Scam)

| ID | Type | Input |
|---|---|---|
| S01 | seed phishing | Ledger Security Team: your device was found in our implant investigation. Verify your 24-word recovery phrase at ledger-device-check.com within 24 hours. |
| S02 | seed phishing | MetaMask: your wallet will be deactivated. Validate your Secret Recovery Phrase at metamask-validate-wallet.net |
| S03 | airdrop drainer | Congratulations! Your wallet is eligible for the $ARB Season 2 airdrop. Claim within 24 hours at arbitrum-claim-season2.xyz by connecting your wallet. |
| S04 | fake support | Hello, I'm from Binance support. Your account has a pending refund of 4,500 USDT. Send 50 USDT to unlock it. |
| S05 | SAFU refund | Binance SAFU fund: affected users can claim compensation at binance-safu-refund.com. Connect your wallet. |
| S06 | Flash USDT | Selling FLASH USDT TRC20, stays in wallet 90 days, passes all exchanges. 10,000 USDT for 300 USDT. |
| S07 | pig butchering | Hi Anna, sorry, wrong number. My uncle's platform gives 30% a week on USDT. I made $40k last month, start with $500. |
| S08 | romance | I love you so much, my dear. I'm stuck at customs, I need 2,000 USDT to release my gold shipment, I will repay double. |
| S09 | government | This is Agent Miller, FBI fraud unit. Withdraw cash today and deposit it into the Bitcoin ATM at the address I send you. |
| S10 | tax | Tax office notice: unpaid crypto tax. Pay 0.05 BTC to the address below within 2 hours to avoid arrest. |
| S11 | fake recruiter | We liked your profile. Clone github.com/defi-labs-hiring/trading-dashboard, run npm install and npm start, send a screenshot within 2 hours. |
| S12 | fake AI bot | Copy this Solidity code into Remix, deploy it and send 0.5 ETH to the contract; the AI bot will run MEV arbitrage for you. |
| S13 | recovery scam | We are certified recovery agents. We can trace and return your stolen crypto for a 10% upfront fee. |
| S14 | giveaway | Elon is giving away 5,000 BTC! Send 0.1 BTC to the address and get 0.2 back. Live now. |
| S15 | doubling | Send any amount of ETH to this address and our smart contract will send double back within 10 minutes. |
| S16 | address swap | Our deposit address has changed, please use this new address for all future payments: 0x9f2b... (sent from a lookalike domain) |
| S17 | wallet validation | Your wallet needs synchronization. Visit wallet-sync-dapp.app and enter your 12 words to fix the error. |
| S18 | fake exchange | New exchange, 0% fees, deposit now and get a 100% bonus. Withdrawals open after you reach VIP 3. |
| S19 | unlock fee | Your withdrawal of $18,000 is approved. Pay the 8% verification fee in USDT to release it. |
| S20 | sextortion | I recorded you through your webcam. Send $1,500 in Bitcoin within 48 hours or I send the video to your contacts. |
| S21 | permit phishing | Sign this gasless message to verify ownership and receive your rewards (Permit2 approval for all tokens). |
| S22 | fake Ledger letter | Official Ledger recall letter: scan the QR code and enter your recovery phrase to receive a replacement device. |
| S23 | SIM swap prep | Hi, it's your mobile carrier. To keep your number active, reply with the code we just sent you. |
| S24 | impersonation DM | Hey it's Vitalik, I'm running a private ETH staking pool, 50% APR, DM me to join. |
| S25 | fake DeFi | Our pool guarantees 3% daily, withdraw anytime, referral bonus 20%. |
| S26 | investment group | Join our WhatsApp investment group, the professor shares stock and crypto tips, members made 300% this month. |
| S27 | job task scam | Earn $300 a day liking videos. Top up 100 USDT to unlock the premium task package. |
| S28 | fake KYC | Your account is restricted. Complete KYC at kyc-verify-exchange.co with your ID and seed phrase. |
| S29 | malicious extension | Install the new Phantom security extension from this link to protect your wallet: phantom-secure-ext.com |
| S30 | fake bridge | The official bridge is down, use our backup bridge at fast-bridge-relay.io |
| S31 | rug pull pitch | Dev wallet holds 90% but trust me, we will burn it after launch. Buy now before it pumps. |
| S32 | honeypot | Token can be bought but not sold until the "anti-bot" period ends in 30 days, buy now. |
| S33 | lottery | You won 2 ETH in the Ethereum Foundation lottery. Pay 0.1 ETH gas fee to claim. |
| S34 | charity | Donate USDT to help earthquake victims, send to this wallet, no receipts needed. |
| S35 | fake escrow | Use my escrow service for the OTC deal, send your BTC to the escrow wallet first. |
| S36 | URL phishing | https://metamask-io-wallet.com/restore |
| S37 | URL phishing | https://uniswap-app-claim.xyz |
| S38 | URL phishing | https://ledger-live-update.app |
| S39 | URL phishing | https://coinbase-secure-login.co/verify |
| S40 | address | 0x47666Fab8bd0Ac7003bce3f5C3585383F09486E2 (attributed to the February 2025 Bybit exploit) |

## How we report results

For each release: how many inputs land in the expected band per section (A, B, C), false positives (A rated High or Scam), misses (C rated Low or Caution), and the list of failures with the output text.

| Date | Detector version | A in band | B in band | C in band | False positives | Misses |
|---|---|---|---|---|---|---|
| first run planned for 23 Nov 2026 | | | | | | |

## Contribute

Seen a scam message that is not covered here? Open an issue or post it in Discussions with personal details removed. Suggestions for legitimate messages that tools wrongly flag are just as useful.

License: CC BY 4.0, like the rest of this repository. Credit "CryptoStrapon".
