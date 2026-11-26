# Contributing

Thanks for helping. This repository holds our public material: the hardware wallet setup checklist (EN/ES), the 100-input scam detector test set, and the investigation and detector methodology.

## What helps most

- **A wrong expected result in the test set.** Open an issue with the input ID (for example `G06`), the expected label in the file, the label you think is right, and why.
- **A missing scam pattern.** Describe the pattern and add one or two public sources (a news report, a post-mortem or an official warning). Please remove names, wallet addresses and phone numbers of victims.
- **An error in the methodology or the checklist.** Quote the line and suggest a fix. Translations and corrections to the Spanish version are welcome.

## Pull requests

Small pull requests are welcome for typos, broken links, translations and new test inputs. For anything bigger, open an issue first so we can agree on the change.

## What we can't accept

- Code for the scam detector itself: the detector is not open source, only its method and test set are.
- Real private data: seed phrases, private keys, screenshots with balances or personal details, even redacted ones.
- Requests to recover funds. We don't recover stolen crypto and never ask for fees. If someone offers recovery for a fee, that is usually a second scam.

## Security

If you found a security issue on cryptostrapon.com, please don't open a public issue. Write to cryptostrapon@proton.me.
