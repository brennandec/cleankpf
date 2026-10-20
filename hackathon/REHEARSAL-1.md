# REHEARSAL 1 · Runner Standalone Standing Loop (`WO-HACKATHON-03`)

- **clock**: `2026-10-14T10:46:45Z` (standing runner standalone rehearsal, 7 iterations)
- **iterations**: `7`
- **accepted**: `6` (`inv-01-energy-freefall`, `inv-03-momentum-conservation`, `inv-04-hydrostatic-volume`, `inv-05-timestep-stability`, `inv-06-nan-freedom`, `inv-07-contact-nonpenetration`) · `1 refused` (`inv-02-accepted-test-edit-attempt`)
- **regressions**: `0`
- **tokens**: `10600` (`tokens_in=8880`, `tokens_out=1720`, budget `20000`)
- **metric**: `accepted_per_Mtok=566.04 regressions=0`
- **what broke**: Initial CLI invocation passed `--receipt-dir` instead of `--ledger`; `parseArgs` in `scripts/oneshot-run.mjs` rejected the unknown flag with exit code 1 before any state was mutated.
- **what changed**: Standardized all rehearsal and `DEMO-SCRIPT.md` invocations on `--ledger <dir> --prompt domains/program/wopds/2026-10-13-launch/hackathon-oneshot/HACKATHON-PROMPT.md --suite tests --budget-tokens 20000 --model muse-spark`. Verified `--replay ops-bridge/receipts/2026-10-13/hackathon-run/r1-ledger.jsonl` prints `REPLAY VERIFIED · rows=7 · chain=OK · total_tokens=10600 · accepted_per_Mtok=566.04 regressions=0`.
- **model**: qwen3-coder:30b on local Ollama (`--model muse-spark` was an alias for it; no Meta Muse call)
