# Offline Stripe payment-recovery comparison

**Equivalent decisions across 12 case families / 21 synthetic variants.** No demonstrated decision-quality advantage over competent Stripe-native recovery plus competent application-owned recovery was found in these fixtures.

This is a synthetic, offline comparison/research artifact. It is not evidence of production payment correctness or customer demand. Convenience, auditability, implementation savings, review effort and support savings remain hypotheses.

The comparison tests uncertain acknowledgement/timeout after PaymentIntent create/confirm. The baseline includes durable operation/key mapping, native SDK retry decisions, current PaymentIntent lookup and deduplicated unordered-event reconciliation. The second arm adds an evidence-gated standardized receipt over the same facts. No Stripe calls or customer cases occurred.

- [Report, method and limits](REPORT.md)
- [Synthetic fixtures and prospective oracle](fixtures.json)
- [Observed synthetic result data](results.json)
- [Data inspection and provenance](DATA-INSPECTION.md)
- [Artifact hashes](MANIFEST.json)

Report questions and specific methodological objections are welcome in this repository's [Issues](https://github.com/Ak4741/payment-recovery-comparison/issues). Reading, downloading, starring or asking a question grants no participant consent. Do not post private logs, secrets, personal information, real payment/account identifiers or customer data. A real workflow study would need separate explicit private consent.

All rights retained. No additional public license is granted. No executable recovery component, proprietary implementation, production adapter or third-party source is distributed here.
