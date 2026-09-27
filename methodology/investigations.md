# Investigation Methodology

CryptoStrapon publishes independent investigations into crypto scams: phishing
campaigns, fake support accounts, fraudulent airdrops, impersonation of
exchanges and public figures, and wallet-drain schemes.

## Principles

- **On-chain first.** Claims about a wallet, contract, or transaction are
  checked against public blockchain explorers (Ethereum, Polygon, Arbitrum,
  TRON) before publication.
- **No accusation without evidence.** A case is only published when there is
  a reproducible artifact: a captured message, a URL, a wallet address with
  on-chain activity, or a matching pattern against a known scam template.
- **Correction over silence.** When new evidence changes a verdict, the case
  is updated and the change is noted rather than the original silently
  replaced.
- **No private data.** Investigations do not publish victims' personal
  information. Wallet addresses and public scam infrastructure (URLs,
  Telegram handles, etc.) are in scope; individuals' identities are not,
  unless the individual is the scammer operating in public.

## What counts as a published case

A case is added to the site's investigation archive when it includes:

1. A description of the scam mechanism (what it claims, what it asks the
   victim to do).
2. Supporting evidence (screenshots, URLs, on-chain transaction links).
3. A plain-language explanation of why it is a scam, written for a
   non-technical reader.

## Scope limits

This methodology describes how investigations are researched and verified.
It does not include the detector's internal scoring logic, prompts, or
infrastructure — see `detector.md` for the public-facing description of how
the automated scanner works.
