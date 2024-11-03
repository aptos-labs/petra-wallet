![](https://pbs.twimg.com/profile_banners/1553173121586249728/1666028736/1500x500)

## Reporting a Security Concern

**DO NOT CREATE AN ISSUE** to report a security problem.

Send an email to [security@aptoslabs.com](mailto:security@aptoslabs.com) and provide your GitHub username. The team will create a new draft security advisory for further discussion.

For security reasons, DO NOT include attachments.

If you haven't done so already, please **enable two-factor auth** in your GitHub account.

Send the email from an email domain that is less likely to get flagged for spam by gmail.

This is an actively monitored account, the team will quickly respond.

If you do not receive a response within 24 hours, please directly followup with the team in [Discord](https://discord.com/invite/petrawallet) by reaching out to anyone with the role “Aptos Labs”.

As above, please DO NOT include attachments or provide detail regarding the security issue in this email.

# Petra Bug Bounty

Aptos Labs offers bounties for security reports. Reports will be validated against the current released version of the [Petra wallet](https://chrome.google.com/webstore/detail/petra-aptos-wallet/ejjladinnckdgjemekebdpeokbikhfci) and no others. This includes only features that have been explicitly enabled by the team and not those that might have been toggled on by modifying debug flags, etc.

Aptos Labs considers the following levels of severity:

****************Critical — Up to $100,000 USD in APT tokens (locked for 12 months)****************

- Website can retrieve plaintext (decrypted) sensitive data or files from the wallet (excluding non-sensitive environment variables, open source code, or usernames), such as plaintext private keys, plaintext sensitive passwords, plaintext recovery phrases.
- Taking state-modifying authenticated actions without any interaction by that user via websites (not via an user’s unlocked computer), such as signing arbitrary bytes, and signing/submitting malicious transactions without user knowledge.
- Malicious interactions with the wallet, without user knowledge, such as modifying transaction arguments or parameters, substituting contract addresses, and being able to extract the private keys without user consent.
- Injection of malicious HTML or XSS into the wallet, via injected DApp API, DApp controlled error messages, and NFT metadata.

**Other Issues**

We are working on a process to accept non-critical bugs that result in heavy negative impact to the user experience.

## **Report Details**
- Summary of the issue
- Does this relate to the definition of a critical issue as defined above? Which point?
- Clear and complete steps to repro the issue
- If applicable, proposed solution

## **Payment of Bug Bounties**

- Bounties are currently awarded on a rolling/weekly basis and paid out within 30 days upon receipt of successful KYC and payment contract.
- The APT/USD conversion rate used for payments is the market price of APT (denominated in USD) at 11:59 PM PST the day that both KYC and the payment contract are completed.
- The reference for this price is the Closing Price given by Coingecko.com on that date given here: [https://www.coingecko.com/en/coins/aptos/historical_data#panel](https://www.coingecko.com/en/coins/aptos/historical_data#panel)
- Bug bounties that are paid out in APT are locked to the account provided by the reporter with a lockup expiring 12 months from the date of the delivery of APT.

## Duplicate Reports

Compensation for duplicate reports will be split among reporters with the first to report taking priority using the following equation:

```
R: total reports
ri: report priority
bi: bounty share

bi = 2 ^ (R - ri) / ((2^R) - 1)
```

Where report priority derives from the set of integers beginning at 1, where the first reporter has `ri = 1`, the second reporter `ri = 2`, and so forth.

Note, reports that come in after the issue has been fully triaged and resolved will not be eligible for splitting.

## KYC Requirements

This bug bounty program is only open to individuals [outside the OFAC restricted countries](https://home.treasury.gov/policy-issues/financial-sanctions/sanctions-programs-and-country-information). Bug bounty hunters will be required to provide evidence that they are not a resident or citizen of these countries in case the submission is eligible for a reward. If the individual is a US person, tax information will be required, such as a W-9, in order to properly issue a 1099. Aptos requires KYC to be done for all bug bounty hunters submitting a report and wanting a reward. Form W-9 or Form W-8 is required for tax purposes. All bug bounty hunters are required to use Persona for KYC, links will be provided upon resolution of the issue The collection of this information will be done by the Aptos Labs.

If an impact can be caused to any other asset managed by Aptos that isn’t on this table but for which the impact is in the Impacts in Scope section below, you are encouraged to submit it for consideration by the project.
