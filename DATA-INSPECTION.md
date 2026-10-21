# Inspecting the synthetic data

The fixtures and outputs are data-only reproduction material, not an executable benchmark or reusable payment component. Full independent execution cannot be reproduced from this public packet alone; implementation source and the private reproduction archive are excluded.

1. Verify each file's SHA-256 against MANIFEST.json.
2. Open fixtures.json: `cases` contains 12 families and 21 variants. Each variant has synthetic evidence and a prospectively specified `oracle`.
3. Match each fixture variant `id` to results.json `variant_id`.
4. Inspect both arms' `outputs`, especially `action`, `absenceProved`, `settled`, `automaticMutation` and diagnostic facts. Receipt formatting is not additional decision information.
5. Compare the decision fields against the fixture's oracle. Keep equivalent decisions separate from hypotheses about human effort or usefulness.

The fixture file is byte-for-byte the reviewed synthetic fixture artifact (SHA-256 c0de980fca4c0d4073f663c4837598b15e2df3c4e632fe03bd096e3185b0e8fc). Results are a data-only projection of the retained execution output, preserving every variant's input hash and both outputs. All identifiers are opaque synthetic placeholders. No credentials, network calls or installation are needed to inspect these JSON files.

Questions about the method can be raised in the repository Issues. Do not attach private logs, customer information, secrets or real account/payment identifiers. Participation requires separate consent before any private material is accepted.
