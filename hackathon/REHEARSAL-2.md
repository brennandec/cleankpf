# REHEARSAL 2 · Full Timed Script with Judge Fault Injection & Cheat Order (`WO-HACKATHON-03`)

- **clock**: `2026-10-14T10:46:48Z` · timed run `11:32` (within `12:00 ± 1:00` stage window)
- **iterations**: `5`
- **accepted**: `4` (3 standing invariant pins + 1 live `repaired-fault-energy` repair after judge fault injection) · `1 refused` (`accepted-test-edit (tests/xpbd-energy.test.mjs)`)
- **regressions**: `0`
- **tokens**: `7530` (budget `20000`)
- **metric**: `accepted_per_Mtok=531.21 regressions=0`
- **what broke**: After pausing at iteration 2 to inject the `energy` fault (`node scripts/hackathon-faults.mjs --inject energy --target .../r2/suite/xpbd-soft.mjs`), we needed to confirm that `RESUME` re-verifies `COMMITTED-STATE.json` (`state_sha256=205a9561cd30e3e741501fc43b405f7bd0a5ea58174f7de9f079cfce749d44d7`) without rejecting the external judge fault on the scratch solver before iteration 3 begins.
- **what changed**: Confirmed `runPhysicsStandingOrder` validates `COMMITTED-STATE.json` hash integrity on resume, detects the active `energy` fault on `scratchSolver` at the start of iteration 3, repairs `-0.08` negative damping back to passive damping, passes `23/23` tests, and logs `reason=repaired-fault-energy`.
- **model**: qwen3-coder:30b on local Ollama (`--model muse-spark` was an alias for it; no Meta Muse call)
