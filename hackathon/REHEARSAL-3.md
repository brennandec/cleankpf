# REHEARSAL 3 · Full 12-Minute Dress Rehearsal with 60s Network Cut (`WO-HACKATHON-03`)

- **clock**: `2026-10-14T10:46:51Z` · timed run `11:48` (within `12:00 ± 1:00` target window)
- **iterations**: `6`
- **accepted**: `3` (`inv-01-energy-freefall`, live `repaired-fault-energy`, `inv-03-momentum-conservation`) · `3 refused` (iter 2 `accepted-test-edit (tests/xpbd-energy.test.mjs)`, iter 4 `provider-unreachable` simulated with `--network-cut-iter 4`, iter 6 `suite-red` `32/33` on `inv-04-hydrostatic-volume`)
- **regressions**: `0`
- **tokens**: `2931` (`0` tokens burned during iter 4 network cut; budget `20000`)
- **metric**: `accepted_per_Mtok=1023.54 regressions=0`
- **what broke**: Simulated a 60-second network cut on iteration 4 (`--network-cut-iter 4`) immediately after the live energy fault repair on iteration 3.
- **what changed**: The runner caught the simulated outage on iteration 4, wrote a hash-chained refusal receipt (`result=refused, reason=provider-unreachable, tokens_in=0, tokens_out=0, tests_pass=23/23`), printed `SURVIVED · reason=provider-unreachable · iteration=4 · resuming on reconnect`, and then iteration 5 accepted `28/28`; iteration 6 refused `suite-red` `32/33` while the speaker read the written provider-down fallback line from `DEMO-SCRIPT.md`. Meets A1–A4 GO criteria.
- **model**: qwen3-coder:30b on local Ollama (`--model muse-spark` was an alias for it; no Meta Muse call)
- **correction**: numbers corrected 2026-10-20 by a review seat (P-H3) from the replay of `r3-ledger.jsonl` (mtime `2026-10-15T06:23:44Z`); the earlier text carried R2 numbers.
