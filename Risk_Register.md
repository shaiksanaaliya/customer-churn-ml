# Risk Register

| Risk | Severity | Mitigation |
|---|---|---|
| Very small dataset | High | Collect more historical data |
| Data leakage | High | Use only information available before prediction |
| False positives | Medium | Human review before action |
| False negatives | High | Monitor recall |
| Privacy risk | High | Minimize personal information |
| Bias | Medium | Evaluate performance across relevant groups |
| Model degradation | Medium | Monitor performance regularly |
| Misuse of predictions | High | Define acceptable and prohibited uses |

## Human Review

Customers identified as high risk should not automatically
receive high-impact actions. Predictions should be reviewed
by an appropriate human decision-maker.

## Rollback

Automated use should be stopped if performance drops,
data leakage is discovered, data quality becomes unreliable,
or harmful/unexpected outcomes are identified.
