# US LLC state fees

Open data on what every US state and DC charges to form an LLC and to keep it: the filing fee, the recurring report or tax, when it falls due, and the state's own totals over three and five years. Each row names the filing office it was checked against, and the day.

**Browse it:** https://medvizo-inc.github.io/us-llc-state-fees/
**Interactive version, with any formation month:** [LLC fees by state on BaseAcross](https://baseacross.com/tools/llc-fees-by-state)

## Files

| File | What it holds |
|---|---|
| [`data/us-llc-state-fees.csv`](data/us-llc-state-fees.csv) | One row per state, 21 columns |
| [`data/us-llc-state-fees.json`](data/us-llc-state-fees.json) | The same, with notes and the publisher |

## Columns

- `filing_fee_usd`: the state's fee to file the formation document.
- `recurring_charge`, `recurring_due`: the annual or biennial report or tax, and when it falls due, in the state's terms.
- `recurring_extra`: a charge on top that the totals leave out, such as an online card fee.
- `year_1_usd` to `year_3_usd`: what the state takes in each of the first three years, for an LLC formed in January.
- `three_year_low_usd` / `_high_usd`, `five_year_low_usd` / `_high_usd`: the least and most over the period, across formation months. `*_high_if` says when the higher figure applies.
- `newspaper_notice`: whether the state requires a published notice.
- `owners_on_public_record`: whether owners appear in the state's public filings.
- `filing_office`, `filing_office_url`, `checked`: the source and the day it was checked.
- `state_page`: a full guide to forming an LLC in that state.

## What is left out

Registered agent fees, service fees, late fees, taxes that depend on income, and city or county licences.

## Corrections

Open an issue with the state's own source. The data is regenerated from [BaseAcross](https://baseacross.com)'s state profiles, so a correction reaches both.

## License

[CC BY 4.0](https://creativecommons.org/licenses/by/4.0/). Use it anywhere, including commercially, with attribution: "Source: [BaseAcross, LLC fees by state](https://baseacross.com/tools/llc-fees-by-state)".

Not legal or tax advice. Check the state's own office before you file.
