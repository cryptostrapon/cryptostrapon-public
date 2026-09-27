# Detector Methodology

The free AI Scam Detector at https://cryptostrapon.com/scam-detector accepts
three kinds of input: pasted text/URLs, screenshots, and wallet/mixer
addresses. It is free, requires no sign-up, and does not ask for private
keys or seed phrases.

## What it checks

At a high level, a scan runs through the same layers shown in the tool's own
"How it works" panel on the site:

- **Message scan** — looks for known scam phrasing and structure (urgency,
  impersonation, fake support, fake giveaways).
- **URL inspection** — checks links for typosquatting, redirect chains, and
  known phishing infrastructure.
- **Blacklist / threat-intel check** — cross-references addresses and
  domains against public threat-intel sources.
- **Wallet & blockchain check** — for a wallet or contract address, pulls
  public on-chain data (transaction history, first-activity date, network
  presence, token-security signals) from public explorers and scanners.
- **Verdict** — combines the above into a severity score (LOW / MEDIUM /
  HIGH / CRITICAL) with a plain-language explanation.

## Known-safe infrastructure

Official token contracts (e.g. USDT, USDC on Ethereum, Polygon, Arbitrum,
TRON) and well-known exchange hot wallets / cross-chain bridges are
recognized as legitimate, high-volume, publicly-labeled infrastructure. A
high number of senders or standard issuer-control features (pause,
blacklist, mint) on these addresses does not by itself indicate a scam — a
message that *quotes* a real address while asking the victim to act is still
judged on its own content.

## What's not in this repository

This document describes the detector's behavior from a user's perspective.
It does not include the underlying prompts, scoring code, allow-lists, or
infrastructure — those remain internal so they can't be reverse-engineered
and gamed by scammers.

## Limitations

The detector is a heuristic tool, not a guarantee. A LOW score means no
known red flags were found — it does not certify that an address or message
is safe. Always verify independently before sending funds.
