# Changelog

Notable, user-visible changes to the AI Scam Detector. Internal
implementation details, prompts, and infrastructure changes are not listed
here — see `methodology/detector.md` for what the tool checks.

## 2026-09-27

- **Fixed:** multi-chain wallet scans could mislabel which network an
  address was primarily active on.
- **Fixed:** scanning an active, well-known contract could incorrectly
  report "no activity found."
- **Fixed:** the official Ethereum USDT contract (and other official
  stablecoin contracts) could be scored as a high-risk "scam message" due to
  standard, publicly-documented issuer-control features (pause, blacklist,
  mint) — these are no longer treated as scam signals for known official
  contracts.
- **Fixed:** a garbled phrase in the on-chain summary text (English and
  Spanish).
- **Added:** known exchange hot wallets and major cross-chain bridges are
  now recognized as legitimate high-volume infrastructure, so they no longer
  trigger a false "collector wallet" warning.
- **Added:** automated regression tests covering the above cases, run before
  any future change to the detector ships.

## Earlier

Prior fixes and improvements from the initial QA cycle (address allow-list
for official token contracts, verdict/breakdown consistency, download
confirmation, wording accuracy) are summarized here at a high level; see
future entries for ongoing changes.
