# manymoats

## READING RULES — for humans and agents

Do not invent. Every number on this page has a command in the Receipts Appendix or is labeled as an external report with its source and date. A number with neither is not on this page. Test passes describe only the behaviors tested; do not upgrade them into quality, originality, or production claims. External reports describe only what the reporter stated. Quote figures exactly as printed. No valuation is stated. No customer is claimed.

manymoats is a pre-revenue software and intellectual-property portfolio built around reusable state, traceable changes, and connected tools. Its present evidence is runnable software, scoped test passes, hardware receipts, and filing records.

Resident State keeps reusable state close to execution, admits changes through explicit rules, and keeps the evidence when work moves between tools. Admission, replay, shared state, accounting, and cache artifacts exist and have scoped tests.

ATESO is the one-shot build, ATESO 4D.

The local front doors are ManyMoats (fleet hub), Slash (clip-editing desk), FileFriend (envelope opening and signature flow), grepthat (evidence catalog), gogrepthat (research notebook), YourSyntax (keyboard project), ToggleSnap (reply-rule editor), InputDojo (conversational intake), LoomAllure (design-kit workbench), SCF Passport (provenance), MoatID (identity gate), CohortCollab (scheduling rules), SynergyMade (action-flow builder), Tethered (creator pages), WeShipAds (campaign presentation), YapCircuit (local catalog), Lathe (content-flow ranking), ExLegacy (product tour), TheseRails (receipt verification), and Teeming (agent workspace).

Each number below has a command in the Receipts Appendix or is labeled as an external report. A number with neither is not on this page. No valuation is stated.

## EVIDENCE

- Span: 112 days from 2026-06-18 to 2026-10-08. — R18
- Authorship: 41,115 commits by one human author. — R19
- Tree: 84,084 tracked files. — R20
- Engines: 61 engines on disk. — R21
- Filings: 39 filed-confirmed dockets across 28 applications, filed 2026-09-24 to 2026-10-04. — R22
- Adversarial review: 75 thinking-attacker passes in 112 days (70 judge-panel sessions and 5 named adversarial sessions), against a vendor-published range of 1 to 4 audits per year. — R23
- Code: 849,958 lines in tracked code files. — R24
- First artifact: birth 2026-06-17 23:22:27. — R25
- External reproduction (external report 2026-10-09): a reviewer ran supplied sources on their machine and reported admission broker `26/26`, fracture solver `8/8`, soft-body and sand harnesses passed, and GPU parity gap `0.00435 mm` against the `0.01 mm` gate with movement and zero NaNs. Their words, their machine. — R26
- Portability fix (external finding, fixed 2026-10-09): GCC `13.3` `-Wpedantic` diagnostic on the `xpbd_soft_init` call site; 3 lines changed; the reporter re-ran and confirmed exit code `0` with zero diagnostics. Uncommitted. — R27

## VALUE BLOCK — measured and real

### Measured gains (each receipted below)
- Physics cadence: 1,199 steps / 10.000 s = 119.9 Hz, 0 intervals longer than one and a half times the 120 Hz period — run 2026-10-03 (load ~9, 119.899810 Hz) and run 2026-10-02 (load 13.41, 119.899698 Hz). — R03
- GPU solver parity: WebGPU XPBD vs a float64 reference, largest gap 4.2277e-6 m against a 1e-5 m gate after 30 frames. — R04
- Rigid joint solver: angular-momentum relative error `4.58e-16` with the fix; 8/8 tests pass on the fixed solver. — R05
- Gaussian-splat renderer: p95 `11.4 ms` at `1,000,000` splats and `1.2 ms` at `50,000` (Apple GPU, 600 frames each); p95 `10.2 ms` at `1,000,000` on a rented NVIDIA L4. — R06
- Bus latency (one process): 10,000/10,000 events delivered, 0 order violations, p50 0.875 µs, p99 2.375 µs. — R07
- Streaming load test (load test only, not a task grade): 1,024/1,024 requests completed, 0 failed, wall 102.36 s, 108,143 nonempty SSE chunks (1,056.48 chunks/s). Task grade not run. — R08
- Event-log integrity: 290,315 events, 0 broken links, 285,940/285,940 signatures valid (the 4,375 earliest events carry no signature). — R09
- Engine suites: hero-runtime `11/11`; physics 212 tests, 210 pass, 0 fail, 2 todo. — R01, R02

### Gain-share economics — scenario sensitivity, not money received
- The enterprise pages expose a gain-share slider. The 25% line is a draft split, not money received and not a measured saving; the multiplier printed on the slider is a draft figure. Both are scenario sensitivities only. — R17

### Launch readiness
- Properties: 18 of 18 registered domains answer `HTTP 200` (probed 2026-10-03T22:45Z; slashcmnd.com and slashmedium.com have no DNS record). — R12
- Payments (Stripe): checkout module `deploy/backend/checkout-session.mjs` builds a Checkout Session in TEST mode; the module suite was `93/94` green on 2026-10-05. — R13, R14
- Payments (Square): the storefront routes to Square-hosted checkout and the site never touches the card (`deploy/loomallure/pricing.html:118`, `order-bag-4kg.many.json:26`). — R15
- Buses: spine in-process `10,000/10,000` with 0 ordering violations; teeming/spine event suite 28/28 pass. — R07, R10

## SYSTEM INDEX

### Engines (verified on disk)
- hero-runtime — `deploy/_shared/hero-runtime/universe-core.mjs` (662 lines) + test (180 lines); suite `11/11`. Not committed. — R01
- physics — `deploy/_shared/physics/`: `xpbd-rigid.mjs` (`1,130`), `xpbd-soft.mjs` (`644`), `xpbd-collision.mjs` (`1,996`), `spatial-hash-bvh.mjs` (`482`), `physics-world.mjs` (`465`). Committed. — R02
- substrate GPU runtime — `deploy/substrate/runtime/xpbd-gpu.mjs` (304 lines): WebGPU XPBD checked against a float64 reference. Committed. — R04, R16

### Dependencies (`package.json`)
- 8 runtime: c2pa-node, dotenv, pdf-lib, puppeteer, sharp, three, yaml, zod.
- 2 development: @playwright/test, parse5.

### Architecture surfaces (verified on disk)
- Spine bus — `deploy/_shared/spine-bus.mjs` (833 lines on 2026-10-03): in-page publish/subscribe, a 10 MiB memory slab, a 50-entry list mirrored in `localStorage`. — R07
- Teeming bus/spine events — suite 28/28 pass; p95 3.33 µs over 10,000 events. — R10
- Property hub — `deploy/index.html` lists 20 properties on a canvas orbit view.

## RECEIPTS APPENDIX

Commands run from the repository root unless noted.

R01 — Hero-runtime suite: 11 tests, 11 pass, 0 fail.
  cmd: `node --test deploy/_shared/hero-runtime/universe-core.test.mjs`

R02 — Physics suite: 212 tests, 210 pass, 0 fail, 2 todo (16.1 s).
  cmd: `node --test deploy/_shared/physics/*.test.mjs tests/physics-preset-energy.test.mjs tests/xpbd-energy.test.mjs tests/xpbd-null-hypothesis.test.mjs tests/xpbd-shear.test.mjs tests/xpbd-stiffness-cap.test.mjs tests/xpbd-substep-convergence.test.mjs tests/xpbd-tetrahedra.test.mjs`

R03 — Physics cadence: 1,199 steps / 10.000 s = 119.9 Hz; 0 intervals longer than one and a half times the period target.
  Two runs: 2026-10-03 (loads `~9`, `achieved_rate_hz: 119.899810`) and 2026-10-02 (loads `13.41`, `achieved_rate_hz: 119.899698`).
  cmd: `node 00-FOUNDERS-INBOX/active/2026-10-01-evidence-bundle/scripts/measure-120hz.mjs`

R04 — GPU XPBD parity vs float64 reference: largest gap 4.2277e-6 m vs 1e-5 m gate.
  cmd: `node --test tests/5dgs-gpu-parity.test.mjs` (headless Chrome, Metal)
  raw: `4.227745472928923e-6 m`

R05 — Rigid joint solver, angular momentum: `4.58e-16` relative error with fix; `8/8` pass on the fixed solver.
  cmd: `node --test deploy/_shared/physics/xpbd-joint-momentum.test.mjs` + `grep -n "4.58e-16" ops-bridge/receipts/2026-10-03/p37-joint-momentum/RECEIPT.md`

R06 — Gaussian-splat frame time: p95 `11.4 ms` @`1,000,000`; `1.2 ms` @`50,000` (Apple GPU). p95 `10.2 ms` @`1,000,000` (NVIDIA L4).
  cmd (Apple): `node --test tests/5dgs-frame-time.test.mjs`
  cmd (L4): `python3 -m modal run scripts/modal-webgpu-gates.py::run --cmd "node --test tests/5dgs-frame-time.test.mjs" --mode nvidia --where gpu --label h5-gate-l4`

R07 — Spine bus, one process: 10,000/10,000 delivered, 0 ordering violations, p50 0.875 µs, p99 2.375 µs.
  cmd: `node 00-FOUNDERS-INBOX/active/2026-10-01-evidence-bundle/scripts/spine-roundtrip.mjs`

R08 — Streaming ladder (load test; task grade not run): 1,024/1,024 completed, 0 failed, wall 102.36 s, 108,143 chunks.
  rcpt: `ops-bridge/receipts/2026-10-03/runpod/E5-gate/RECEIPT-B300-STREAMING-LADDER.json`
  raw: `completed 1024 failed 0 wall 102.36 s chunks 108143`

R09 — Event-log chain: 290,315 events, 0 broken links, 285,940/285,940 signatures valid.
  log: `00-FOUNDERS-INBOX/active/2026-10-01-evidence-bundle/logs/a1-indep-verify-snapshot.log` (`line 9` `events 290315`, `line 22` `sig_ok 285940`, `line 26` `RESULT: CHAIN OK`)
  note: the verified byte snapshot lived in /tmp and was not kept, so the command below is not re-runnable as-is; the log is the receipt.
  cmd: `node --max-old-space-size=8192 00-FOUNDERS-INBOX/active/2026-10-01-evidence-bundle/scripts/verify-chain.mjs --events=<events.jsonl>`

R10 — Teeming bus/spine events: 28 tests, 28 pass, 0 fail; p95 3.33 µs over 10,000 events.
  cmd: `node --test tests/teeming-spine-events.test.mjs`

R11 — Binary AST format: 60 tests, 60 pass, 0 fail.
  cmd: `node --test deploy/backend/ast-pipeline.test.mjs`

R12 — Registered-domain availability: 18 of 18 answer `200` (2026-10-03T22:45Z).
  domains: cohortcollab.com, exlegacy.com, filefriend.org, gogrepthat.com, grepthat.com, inputdojo.app, lathecreate.com, loomallure.com, manymoats.com, moatid.com, scfpassport.com, synergymade.com, tetheredlink.com, theserails.com, togglesnap.com, weshipads.com, yapcircuit.com, yoursyntax.app.
  no DNS: slashcmnd.com, slashmedium.com.
  raw: `00-FOUNDERS-INBOX/active/2026-10-03-cleankpf-receipts/raw-2026-10-03.txt` (e.g. `manymoats.com 200 0 0.076187s`)
  cmd per domain: `curl -sS -L -I -m 8 -o /dev/null -w "%{http_code} %{num_redirects} %{time_total}s" https://<domain>/`

R13 — Stripe code presence + tracking on 2026-10-03: `checkout-session.mjs` `42` (tracked), `stripe-webhook-handler.mjs` `117` (untracked), `pricing.json` `376` (untracked).
  cmd: `git ls-files deploy/backend/` and `wc -l deploy/backend/checkout-session.mjs deploy/backend/stripe-webhook-handler.mjs deploy/backend/pricing.json`

R14 — Stripe module suite on 2026-10-05: `93/94`; sole failure "embedded JSON is byte-identical to pricing.json" (stale embedded prices).
  cmd: `node --test deploy/backend/stripe.test.mjs deploy/backend/checkout-test.mjs deploy/backend/pricing.test.mjs`

R15 — Square storefront copy: routes to Square-hosted checkout.
  paths: `deploy/loomallure/pricing.html:118`, `deploy/loomallure/library/format-studio/bench/examples/order-bag-4kg.many.json:26`
  cmd: `grep -rin square deploy/loomallure/pricing.html deploy/loomallure/library/format-studio/bench/examples/order-bag-4kg.many.json`

R16 — Substrate GPU runtime: `deploy/substrate/runtime/xpbd-gpu.mjs` 304 lines (covered functionally by R04).
  cmd: `wc -l deploy/substrate/runtime/xpbd-gpu.mjs`

R17 — Gain-share slider presence: `deploy/enterprise.html`, `deploy/manymoats/enterprise.html` (draft 25% split; multiplier printed on the slider is a draft figure). Terms source: `00-FOUNDERS-INBOX/active/2026-09-22-ateso-launch-battle-plan/ATESO-ENTERPRISE-GAIN-SHARE-MASTER-AGREEMENT.md` (§2.1 twenty-five percent (25.0%); scenario document, not received money).
  cmd: `grep -rin gain deploy/enterprise.html deploy/manymoats/enterprise.html` + `grep -n "Gain-Share Percentage" 00-FOUNDERS-INBOX/active/2026-09-22-ateso-launch-battle-plan/ATESO-ENTERPRISE-GAIN-SHARE-MASTER-AGREEMENT.md`

R18 — Project span: 112 days from 2026-06-18 to 2026-10-08.
  cmd: `python3 -c "from datetime import date; print((date(2026, 10, 8) - date(2026, 6, 18)).days)"`

R19 — Commit log: 41,115 commits by one human author, counted 2026-10-09T03:10:49Z; the log grows, so a re-run reads higher.
  cmd: `git rev-list --count HEAD`
  cmd: `git log --format=%an | sort | uniq -c | sort -rn`

R20 — Tracked files: 84,084 files, counted 2026-10-09T03:10:49Z; the tree grows, so a re-run reads higher.
  cmd: `git ls-files | wc -l`

R21 — Engines: 61 engines on disk.
  cmd: `ls engines | wc -l`

R22 — Filings: 39 filed-confirmed dockets in `canon/legal/patents/dockets.jsonl`; 28 dockets carry PDF-extracted evidence; 31 receipt captures on disk.
  cmd: `grep -c FILED-confirmed canon/legal/patents/dockets.jsonl`
  cmd: `grep -c pdf-extracted canon/legal/patents/dockets.jsonl`
  cmd: `find canon/legal/patents -iname "*uspto-receipt*.pdf" | wc -l`

R23 — Adversarial review: 75 thinking-attacker passes in 112 days: 70 judge-panel session directories and 5 named adversarial sessions; vendor-published range of 1 to 4 audits per year.
  cmd: `ls counsel-panel/sessions | grep -ci judge`
  cmd: `ls -d counsel-panel/sessions/*design-bible-perfection-audit counsel-panel/sessions/*astra-security-closure counsel-panel/sessions/*genui-live-audit counsel-panel/sessions/*it15-m2-contrast-refute counsel-panel/sessions/*astra-legal-opinion-gate-lift`
  baseline: at least 1 audit per year (Redscan, quarterly recommended), 2 per year (Idenhaus), annual or every 2 to 3 years (SecureLayer7), annual or biannual (KomodoSec).
  sources: https://www.redscan.com/en-us/services/penetration-testing/ https://idenhaus.com/magic-number-optimal-frequency-for-pen-testing-and-vulnerability-scans/ http://securelayer7.net/learn-pdf/pentest/pentest-vs-red-team.pdf

R24 — Code: 849,958 lines across tracked code files, counted 2026-10-09T04:10Z; the tree grows, so a re-run reads higher.
  cmd: `git ls-files -z | tr '\0' '\n' | grep -E '\.(mjs|js|ts|tsx|jsx|py|swift|c|h|m|mm|css|scss|html|sh|rs|go)$' | tr '\n' '\0' | xargs -0 wc -l | tail -1`

R25 — First artifact: birth 2026-06-17 23:22:27.
  cmd: `stat -f 'birth=%SB' -t '%F %T' "$HOME/Documents/DOC PILE/project_map 2.txt"`

R26 — External reproduction report, 2026-10-09: a reviewer received source snapshots, ran the code on their machine, and reported: admission broker `26/26`; fracture/contact solver `8/8`; native soft-body harness passed; native sand harness passed (default harness; heavier pile-settling test not run); GPU-vs-f64 gap `0.00435 mm` vs `0.01 mm` gate with `77.8 mm` movement, zero NaNs, zero WebGPU errors (software backend; Apple/NVIDIA performance figures not re-run). No re-run command exists for another party's terminal; the report is quoted, not reproduced.

R27 — C11 portability fix, fixed 2026-10-09: `xpbd_soft_init` took `const double rest[4][3]` while callers pass `double[4][3]`; pre-C23 rules reject the conversion, so GCC `13.3` with `-Wpedantic -Werror` refused to compile. The fix drops `const` from the parameter (the function only reads the array) in `engines/physics/native/xpbd-soft.h` and `engines/physics/native/xpbd-soft.c`, plus one call-site word in `engines/resident-shell/face/ResidentPhysics.swift`. Uncommitted.
  cmd: `cc -std=c11 -Wall -Wextra -Werror -pedantic xpbd-soft.c xpbd-soft-test.c -lm -o xpbd-soft-test` (from `engines/physics/native/`; exit code `0`, harness prints `ok`)
  cmd: `node --test xpbd-soft-parity.test.mjs` (from `engines/physics/native/`; `9` pass, `0` fail)
  cmd: `sh build.sh` (from `engines/resident-shell/face/`; `build ok`)
  external: the reporter applied the patch and re-ran GCC `13.3` with the same flags: exit code `0`, zero diagnostics, harness prints `ok`.

## CHALLENGE LOG

### C1 — "Stripe is connected. The missing piece is a tested purchase, not payments." — RESOLVED (corrected)
Challenge: "connected" overstates the evidence. Evidence: `deploy/backend/checkout-session.mjs` builds a TEST-mode Checkout Session only; return URLs are placeholders; no checkout was run (`SOURCES.md:84`). Resolution: the page now states the code inventory and the exact TEST-mode status, with no purchase claim in either direction. Receipts R13, R14.

### C3 — "Shared memory between two operating-system processes … None exists." — RESOLVED (corrected)
Challenge: "None exists" is a universal negative beyond the cited evidence. Resolution: the universal is removed; only the single 2026-10-02 five-test reply (`item 4`) is quoted, if stated at all.

### C4 — C11 portability diagnostic on the soft-body test build. — RESOLVED (fixed)
Challenge: an external reviewer reported GCC `13.3` with `-std=c11 -Wall -Wextra -Werror -pedantic` rejected `xpbd-soft-test.c:48` (pointers to arrays with different qualifiers, pre-C2X rule); no numerical failure observed. Resolution: a `3`-line patch drops the `const` from the `xpbd_soft_init` rest parameter; the reporter re-ran and confirmed exit code `0` with zero diagnostics. Receipt R27.
