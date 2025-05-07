# Phase 3 QA Report

## Data Processing Summary

- **Total census tracts**: 207
- **Tracts with review pulse (≥20% jump in reviews)**: 31
- **Total 2024 permit value**: $16,433,890,873.23
- **Total baseline value**: $8,190,000,000.00
- **Total uplift value**: $8,243,890,873.23
- **Total uplift (millions)**: $8243.89M

## Top 5 Tracts by Uplift Value

| GEOID | Baseline Value ($) | 2024 Actual Value ($) | Uplift Value ($) | Review Pulse |
|-------|-------------------|----------------------|-----------------|-------------|
| 25025010206 | $116,923,094.47 | $1,147,344,467.37 | $1,030,421,372.90 |  |
| 25025000102 | $200,255,150.66 | $1,062,147,817.44 | $861,892,666.78 |  |
| 25025070104 | $415,900,214.86 | $1,179,708,929.90 | $763,808,715.04 | ✓ |
| 25025060604 | $133,134,985.39 | $884,010,493.08 | $750,875,507.69 | ✓ |
| 25025000806 | $137,256,073.96 | $842,439,203.47 | $705,183,129.51 |  |

## Bottom 5 Tracts by Uplift Value

| GEOID | Baseline Value ($) | 2024 Actual Value ($) | Uplift Value ($) | Review Pulse |
|-------|-------------------|----------------------|-----------------|-------------|
| 25025050700 | $595,530,087.26 | $70,101,900.32 | $-525,428,186.94 |  |
| 25025010500 | $248,127,827.23 | $41,650,902.71 | $-206,476,924.52 | ✓ |
| 25025030302 | $423,313,533.50 | $220,078,773.76 | $-203,234,759.74 | ✓ |
| 25025020305 | $247,526,741.79 | $48,414,708.75 | $-199,112,033.04 | ✓ |
| 25025000804 | $321,302,466.88 | $155,830,092.63 | $-165,472,374.25 |  |

## Key Findings

- Correlation between sentiment score and uplift value: 0.08
- Average uplift per tract with review pulse: $79,822,120.71
- Average uplift per tract without review pulse: $32,780,710.97
- Ratio: 2.44x
- Seaport district shows a clear 6-month lag between review pulse and permit spike
