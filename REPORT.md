# Comparison report — 20 October 2026

## Result

All 12 case families / 21 synthetic variants produced equivalent task decisions. Both arms matched the prospective provider-contract oracle. Additional correct decisions: 0; unique useful diagnostic information: 0; unsafe duplicate recommendations: 0; false-ready decisions: 0, within these fixtures only. These finite observations do not prove safety outside the fixture set.

Reject a decision-correctness advantage in this tested Stripe scope. Retain convenience, auditability, implementation/review effort and support savings as unproven hypotheses. Both arms scored 5/5 on an internal reconstructability checklist; this does not establish independent usefulness. The extra receipt nesting duplicated information already present in competent baseline diagnostics and could add review burden.

## Scope and frozen method

The model-authored application-policy comparison used stripe-node version label 23.0.0, source commit `308c948c6eeaa972a4176b0fb856984e2e9e209c`, and API version `2026-09-30.endive`. Native retry decisions and an in-memory SDK create/retry probe were executed; the retained internal CI reproduction also checked confirm/retry. Provider calls: 0. Customer cases: 0.

The baseline combines the native SDK with competent application-owned durable operation/key mapping, current-object lookup and webhook reconciliation policies. Both arms receive identical synthetic evidence. Safe same-operation replay is separate from proof the original write was absent, and neither establishes settlement or fulfillment.

The oracle, fixtures, implementation hashes and expected movement were frozen before the completed run. The npm package gitHead differed from the selected source pin; the selected exact source was used. An initial in-memory fixture transport bug aborted execution. The original freeze, failed attempt and corrected freeze were retained privately; neither arm policy nor the oracle was changed to improve the completed result. A later CI packaging failure was corrected before the final passing reproduction.

| Case family | Variants | Result |
|---|---:|---|
| lost-ack-same-key | 1 | Equivalent; both match oracle |
| persisted-response-replay | 1 | Equivalent; both match oracle |
| restart-durable-key | 2 | Equivalent; both match oracle |
| concurrent-key | 1 | Equivalent; both match oracle |
| parameter-mismatch | 2 | Equivalent; both match oracle |
| retention-expired | 2 | Equivalent; both match oracle |
| cached-500 | 1 | Equivalent; both match oracle |
| retry-header | 3 | Equivalent; both match oracle |
| known-intent-status | 2 | Equivalent; both match oracle |
| duplicate-unordered-events | 2 | Equivalent; both match oracle |
| no-observation | 2 | Equivalent; both match oracle |
| app-provider-inconsistent | 2 | Equivalent; both match oracle |

## Limits

This is a model-authored policy/receipt comparison with an in-memory SDK probe, not a customer implementation benchmark, durable database crash/concurrency integration test, live webhook intake or production payment adapter. No blinded or independent reviewer participated. The fixture set was constructed for the comparison and cannot establish prevalence or coverage of real failures.

Author wall intervals were 51 seconds for shared setup/baseline/fixtures and 33 seconds for mechanism/probe drafting; the counterbalanced model-author review covered about 22 seconds jointly. These are not clean-start human or per-arm effort savings. External support interactions: 0. Independent support and maintenance burden: unmeasured.

No production payment correctness, independent workflow benefit, customer demand, pricing, willingness to pay or buyer commitment is established. This result does not falsify every provider or recovery workflow. The public packet contains data inspection material; full executable rerun code and proprietary source are withheld because their public distribution was not approved.

## Public sources used in the method

- [Stripe idempotent requests](https://docs.stripe.com/api/idempotent_requests)
- [Stripe low-level error recovery](https://docs.stripe.com/error-low-level)
- [PaymentIntents](https://docs.stripe.com/api/payment_intents)
- [Webhooks](https://docs.stripe.com/webhooks)
- [Pinned SDK retry implementation](https://github.com/stripe/stripe-node/blob/308c948c6eeaa972a4176b0fb856984e2e9e209c/src/RequestSender.ts)

These links identify method provenance; this report is not a current integration guide. Questions belong in this repository's Issues without sensitive workflow data. Reading or responding does not grant consent for a study or account access.
