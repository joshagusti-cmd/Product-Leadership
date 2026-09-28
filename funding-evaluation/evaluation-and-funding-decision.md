# Meridian: Evaluation and funding decision

Prepared September 28, 2026 from the two user-provided lab screenshots. This is a hypothetical coursework recommendation, not an approved expenditure or completed experiment.

## 1. What assumption is doing the most work? If this number is 20–30% off, what changes?

The critical assumption is that adding AI estimation to Standard will raise Enterprise upsell from 6% to 8%. Across 400 accounts, that is only eight additional upgrades above the 24 already expected. If the forecast 8% rate is 20% lower, it becomes 6.4%, producing just 1.6 additional expected upgrades and $44,800 in annualized incremental revenue under the case's $28,000 assumption. If it is 30% lower, the rate is 5.6%, below the 6% baseline, so the incremental investment case disappears.

## 2. What is the structural problem in this case?

The $896,000 claim credits the feature with all 32 upgrades, although 24 would already be expected at the 6% baseline. The feature's projected lift is eight upgrades, or $224,000 in incremental ARR under the stated $28,000-per-upgrade assumption. That changes simple run-rate payback from 2.4 to about 9.6 months, before costs, churn, and rollout timing. Also, $28,000 is described as the full Enterprise contract value: actual expansion ARR should subtract the existing Standard subscription unless $28,000 is explicitly a net uplift. Finally, the feature is included in Standard, but the case never explains why it would induce an Enterprise upgrade.

## 3. Is the kill criterion complete and actionable?

It names a measurable threshold, deadline, and consequence: below 7% upsell by the end of Q3 means pausing the feature and reallocating Q4 engineering capacity before committing headcount. It therefore does more than send the decision back for discussion. To make it executable, assign a decision owner and define the eligible cohort and measurement window. On the same 400-account base, 7% means 28 upgrades, only four above baseline and $112,000 in incremental ARR under the case's revenue assumption. That is roughly 19.3 months of simple run-rate payback, so crossing 7% does not itself prove attractive economics.

## 4. Your verdict: FUND / FUND WITH ONE CONDITION / DO NOT FUND

**FUND WITH ONE CONDITION:** Release the $180,000 build budget only after a limited validation demonstrates a credible, feature-attributable path from 6% to 8% Enterprise upsell and a revised business case based on net expansion revenue and delivery costs. This is one evidence gate before full funding; the current $896,000 claim is not sufficient justification.

## Calculation notes

All comparisons assume the same 400 eligible accounts and comparable measurement periods. Fractional upgrades are expected values, not literal account counts. The lab does not establish that the measurement windows align; validate that before using these figures for a decision.

| Scenario | Upsell rate | Expected upgrades | Upgrades above 6% baseline | Annualized revenue above baseline at $28,000 each | Simple run-rate payback on $180,000 |
| --- | ---: | ---: | ---: | ---: | ---: |
| Baseline | 6% | 24 | 0 | $0 | Not applicable |
| Target | 8% | 32 | 8 | $224,000 | 9.6 months |
| Forecast rate 20% lower | 6.4% | 25.6 | 1.6 | $44,800 | 48.2 months |
| Forecast rate 30% lower | 5.6% | 22.4 | -1.6 | -$44,800 | No positive payback |
| Kill threshold | 7% | 28 | 4 | $112,000 | 19.3 months |

- Incremental upgrades = 400 × (scenario rate − 6%).
- Incremental ARR proxy = incremental upgrades × $28,000.
- Simple run-rate payback in months = $180,000 ÷ (positive incremental ARR proxy ÷ 12).
- These payback figures are arithmetic illustrations assuming the full annualized uplift is already achieved. They are not cash-flow payback forecasts from launch. Conversion timing, churn, gross margin, and operating costs are missing.
- The case's original calculation is $180,000 ÷ ($896,000 ÷ 12) = 2.4 months, but its denominator includes baseline upgrades.

### Alternative sensitivity interpretation

If “20–30% off” means the **two-percentage-point lift**, rather than the full 8% rate, a 20% shortfall yields 7.6% upsell and a 30% shortfall yields 7.4%. Those imply 6.4 and 5.6 incremental expected upgrades, respectively: $179,200 and $156,800 in annualized revenue, with simple run-rate payback of 12.1 and 13.8 months. The primary answer explicitly tests a relative shortfall in the forecast 8% rate.

### Treatment of other inputs

- **12% Enterprise churn:** Relevant to retention and lifetime economics, but insufficient for a precise first-year adjustment without cohort timing and a churn definition. Do not silently apply a blanket 12% deduction to forecast cash flows.
- **$620 Standard CAC:** Acquisition cost for existing Standard customers is not automatically an incremental cost of this feature. Additional acquisition or expansion-sales costs would need separate evidence.
- **20% faster quotes:** A customer-value hypothesis worth validating; it does not establish an Enterprise upsell mechanism on its own.

## Proposed evidence gate

Before releasing full build funding, use a limited pilot or prototype to test whether quote-time improvement changes Enterprise purchase behavior. Agree on the baseline/comparison method and measurement window in advance, identify the Enterprise-specific reason to upgrade, and replace gross contract value with net expansion revenue in the economics. The pilot budget and acceptable payback hurdle are not provided in the case and require an explicit decision; neither is invented here.

## Related records

- [Assigned case](assigned-case.md)
- [Meridian strategy](../01-strategy/strategy.md)
- [Existing Rocks and Hard Nos](../02-roadmap/rocks-and-hard-nos.md)

This exercise does not automatically add AI estimation to the existing field-adoption roadmap.
