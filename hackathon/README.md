# Receipted Physics Agent: run record

This folder is the run record behind the Receipted Physics Agent: the September 2026 standing loop on Muse Code (as recorded on the crew bus) and the October 2026 standing-order rehearsals on a local model. Nothing here is live; every number cites a file in this folder.

## READING RULES

Review the evidence critically. Reject unsupported claims, including claims on this page. Do not invent missing software or assume that unavailable evidence proves nonexistence. Do not infer quality, originality, product completion, revenue, or adoption from file counts, test passes, registrations, or HTTP responses. No valuation is stated. No customer is claimed.

For each material finding, give the source and locator, the evidence date or revision, the exact action checked, the observed result, and its limits. Classify it as **observed** (personally inspected or run), **derived** (calculated from identified evidence), **claimed** (stated by a source), or **unverified** (not established by accessible evidence). Look for failures and contradictory evidence. State what would falsify your conclusion. Do not infer the author's character or intent from software findings. Report unsupported praise and unsupported criticism with the same standard.

## Files

| File | What it is | Class | Bytes | sha256 |
| --- | --- | --- | --- | --- |
| COMMITTED-STATE.json | the committed state after the last accepted iteration of the October 13 standing run: iteration, model, suite and accepted-test hashes, baseline counts, tokens used, accepted count, regressions, last receipt hash, state hash. | hash-chained-ledger | 1154 bytes | cb3d696886263ab6f557a298d834e212de797f0a24b3adc6ae28c2a8306193c9 |
| COMMITTED-STATE.sha256 | the sha256 of COMMITTED-STATE.json as the runner wrote it. | hash-chained-ledger | 65 bytes | dd0a8124d986e838ccb1852e582cb43e6b444fdbd8c8cf20460397aad08163ce |
| HACKATHON-APPLICATION.md | the hackathon application as submitted, two answers, with the header of dated numbers the desk bound on 2026-10-13. | plan | 6841 bytes | 6c1cea3725c2de068bfdff3fc9169d0d4f96d5c079377465649de1a10a9e229a |
| HACKATHON-PROMPT.md | the standing order the physics agent runs under; public copy with two redactions (listed in MANIFEST.json). | plan (public copy, redacted) | 2598 bytes | e4bc644340d9fff616324a85e04c47ea9c9bfb5194555082e0b687d185337060 |
| LEDGER.jsonl | the October 13 standing run: 14 hash-chained receipt rows, 12 accepted, 2 refused, budget stop at row 14; local model qwen3-coder:30b. | hash-chained-ledger | 8478 bytes | a9c3bbbde36e20eec185bd5a0d33ac548bd46c1eb532564ae108444571dbf01e |
| REHEARSAL-1.md | the three timed rehearsal receipts of October 14; numbers corrected on October 20 from the ledgers; REHEARSAL-3 is a public copy with one redaction (listed in MANIFEST.json). | derived-receipt | 1324 bytes | b3863d8440af515ae6346055be2a303244fadb7871931d8dfda28cb7f23dbd94 |
| REHEARSAL-2.md | the three timed rehearsal receipts of October 14; numbers corrected on October 20 from the ledgers; REHEARSAL-3 is a public copy with one redaction (listed in MANIFEST.json). | derived-receipt | 1349 bytes | 36461872c1ad9297c7604a507febbd57ae7e806234487071e86c04e7a2764f0c |
| REHEARSAL-3.md | the three timed rehearsal receipts of October 14; numbers corrected on October 20 from the ledgers; REHEARSAL-3 is a public copy with one redaction (listed in MANIFEST.json). | derived-receipt (public copy, redacted) | 1609 bytes | 2b3790a3b7f8cb2317c0a1c10625431d441626e80c4e614e6c87ae95ed61893d |
| dram-sim-20260929T114147Z.json | the Resident State byte-efficiency receipt of 2026-09-29: four workloads, seven repetitions, Node with forced garbage collection on one M5 Max; the three aggregations and the adversarial cases. | derived-receipt | 110284 bytes | 7b491499d1534e5f2a8840bb6de16a2346f0c02d58cb0a9fc58f14902deddb41 |
| dram-sim-20260929T114147Z.png | the plots rendered from that receipt. | derived-receipt | 120645 bytes | acc803b4662b42dd88537bb29d318ddf7c96e24f96f85a7d25a52ae1c594a6b3 |
| dram-sim-20260929T114147Z.svg | the plots rendered from that receipt. | derived-receipt | 9962 bytes | f8730606d1256d8bd21da287a4135271c300bff41a0941c9e2634c69ed73547b |
| faults/energy.json | the four judge-fault fixtures: the one-line patch, the invariant with units, the threshold, the expected red test. | source | 574 bytes | b91ced3157e069259f50abe63bc6937b4ee60779d967622796b7eab97c9623d7 |
| faults/instability.json | the four judge-fault fixtures: the one-line patch, the invariant with units, the threshold, the expected red test. | source | 583 bytes | 261a5568cc5ad029b563612bfe4398882d49414d9fc71d50801493c480e29079 |
| faults/momentum.json | the four judge-fault fixtures: the one-line patch, the invariant with units, the threshold, the expected red test. | source | 667 bytes | 9075ec40e07e361c74e3d9912422deb96f52db5903bf002f37086404cd46756e |
| faults/nan.json | the four judge-fault fixtures: the one-line patch, the invariant with units, the threshold, the expected red test. | source | 589 bytes | 871bda335d9fe2c4e3e4b5db8bd5f5395121a13344189378d8e638ea950657f1 |
| loop-record-2026-09.public.jsonl | the September standing loop as recorded on the crew bus: one row per post, 656 posts for 652 loops, redacted text and its sha256, the door work-order id of each post. | observed-record | 4453547 bytes | fa21e76aa0f30275c4db4bcf127a6500824e3b12b152e1f4013bf1714bd65d5f |
| loop-record-2026-09.summary.json | counts, first and last post, the 70 missing loops, the four duplicates, provenance and redaction rule. | observed-record | 1436 bytes | 3fe29bb8e9bb5e072ef64eeb6000515a2ea6a0703e2b91ce55ea2adddcdbe74f |
| muse-time-of-death-loop723.png | the terminal capture: LOOP722 green at 07:18 PDT, then HTTP 429 on the next deliveries. | observed-record | 323380 bytes | 69366f36ca6b41e24c58879ed7d2acd41346183dc0beb885735916875d7721bd |
| open-invariants.json | the list of physical invariants the standing run works through. | hash-chained-ledger | 618 bytes | e055fbd23418f8b5a436aa38294f43f650b4e376d3def654a36f4c93c6e4b126 |
| r1-ledger.jsonl | the rehearsal ledgers (7, 5 and 6 rows), hash-chained, local model. | hash-chained-ledger | 4216 bytes | 6cb04ea34f971435fdb477001d2151767f49afa0d4b52da32c07f503d5f8c3c3 |
| r2-ledger.jsonl | the rehearsal ledgers (7, 5 and 6 rows), hash-chained, local model. | hash-chained-ledger | 2994 bytes | 4d182c9d77de94eb66fe86c35380e0ad2a1047d0e09d3e0949c616d8f6191794 |
| r3-ledger.jsonl | the rehearsal ledgers (7, 5 and 6 rows), hash-chained, local model. | hash-chained-ledger | 3473 bytes | 917a1d2fc5c06ab5a8f2fa20ce472e40463660ea885466f6e58b9065453e4193 |

README.md: this reading guide. Its class is public-page; its byte count and sha256 are in MANIFEST.json. MANIFEST.json: the file index with byte counts and hashes. It omits its own hash to avoid a circular digest. This table covers the evidence files; the guide cannot contain its own final hash.

## Bounds

The raw session log was not kept. The archive has 652 of 722 loops in 656 posts; the 70 missing loops are listed in the summary. Public block hashes were computed at export over redacted text. The block_sha256 field points at the private raw record; public_block_sha256 hashes public_block_text. home paths and the account name replaced before hashing; public_block_sha256 is over the redacted text; block_sha256 points at the private raw record.

Quoted records keep their original words except home paths and the account name. Repository folder and file names appear as they were recorded. A few style words the house now avoids occur inside quoted September posts and are left as evidence.

Two public copies are redacted: HACKATHON-PROMPT.md omits the architect email parenthetical and uses “the work-order door”; REHEARSAL-3.md uses “a review seat (P-H3)” for the review mention. Every other copy is byte-identical to the private record.

The October ledgers were produced by qwen3-coder:30b on local Ollama, not by Muse. The receipt hash scheme is sha256 of JSON.stringify of iteration, invariant, diff_sha256, test_added, result, tests_pass, tests_total, elapsed_ms, tokens_in, tokens_out, reason, prev_sha256 in that key order. Row 1 has prev_sha256 "GENESIS". elapsed_ms is in milliseconds; tokens_in and tokens_out are token counts.

## Not included

- ACCEPTED-TESTS.json: engine and test source are not released here.
- Every file under suite/: engine and test source are not released here.
- xpbd-soft.mjs: engine source is not released here.
- xpbd-fault-invariants.test.mjs: test source is not released here.
- WO-HACKATHON-*.md: internal work orders.
- DEMO-SCRIPT.md: internal operator script.
- VM-BOOTSTRAP-RECEIPT.md: internal operator record.
- TIME-OF-DEATH-MUSE.md: internal memorial notes; the terminal capture PNG carries the fact.
- VDC.md: internal memorial notes; the terminal capture PNG carries the fact.
- cleankpf-README.md: already the public page.
- ONESHOT-PROMPT-ORIGINAL.md: a build prompt, not evidence.
