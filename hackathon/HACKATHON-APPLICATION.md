# HACKATHON APPLICATION · final · 2026-10-13 19:28 PDT
Founder-polished with the Fable desk 2026-10-13 19:10–19:25 PDT.
Numbers bound on 2026-10-13: 17.1 GB model open 138 ms / +8.3 MB dirty vs 19 GB dirty / 11.6 s (ops-bridge/receipts/2026-10-13/founder-cook/COOK-2026-10-13.md) · 2,806 files (gate-engine-avoidance --all) · 136 checks (founder) · 18 styles / 17 runs 0 frames differing (COOK fold) · 1,500 rows / 10 sources (_system/registers/EVERYTHING.json gen 10 = 1,518) · 600 / 234 (ops-bridge/receipts/2026-10-12/launch-reverify/) · 31 applications / 42 dockets (canon/legal/patents/dockets.jsonl + PROV-001/002 serials) · 51 h 35 min / 722 / 15→62 (founder; receipts owed in the public trail).

## What's something you've built lately, and how?

On June 18 i had never written a line of software. Four months later i've built ManyMoats: 21 connected products on ICEBLOCK, my resident-state engine, a native macOS shell, and a multi-agent AI crew that builds, verifies and receipts its own work under law i wrote. Finishing touches are underway. It is worth your time now. i didn't learn to code and then build. i drew the structure at a level i couldn't type yet and closed the gap daily, the way an architect walks the site before the trades arrive.

ICEBLOCK is the foundation. Authoritative objects live in a portable C core as 64-byte granules, committed by revision-word compare-and-swap, checkpointed under Merkle roots, with a byte-object codec that stores arbitrarily large values across hash-derived chunk identities. No partial writes; a stale revision refuses instead of corrupting. On my M5 Max the resident representation measured 52.82% fewer bytes than equivalent JavaScript object graphs across four deterministic workloads. State that doesn't move doesn't burn compute: the cheapest inference is the one whose working state you never rebuilt.

What stands on it, with the numbers:

- Model weights as resident state. A 17.1 GB model opens in 138 ms and adds 8.3 MB of dirty memory; the weights stay clean file pages bound zero-copy to Metal. The incumbent local server holds the same model as 19 GB dirty behind an 11.6 s cold load. Tokenizer parity with llama.cpp, 200/200 on the oracle corpus. Inference on this path lands next; i won't call it done before it answers a prompt.
- One engine per behavior. Physics, splats, materials, motion, hashing and design tokens each have exactly one owner. A lint gate over 2,806 files refuses any file that reimplements an owned behavior, and the pre-existing debt is frozen in a ledger that can only shrink.
- A 4D Gaussian-splat format with byte-exact Swift/JavaScript parity (136 checks green), XPBD soft-body physics, a native Swift/AppKit + Metal shell with no Electron, and a hub that is a working orrery: every product is a destination in it.
- Slash: one motion script renders in 18 registered styles through Remotion, byte-identical across repeated and concurrent renders (17 runs, 0 frames differing), cuts locked to a synthesized beat.
- Nothing lives in my memory. One register holds every open item in the house, 1,500 rows from 10 sources, each with a path, line, hash, owner engine and status; a gate goes red the moment anything exists without a row.
- Assume every approval is wrong. Last weekend i had the crew re-verify 600 of its own prior approvals as if a lesser model had signed them. 234 did not survive. i kept all of it.
- 31 provisional patent applications on file at the USPTO since September 20, covering 42 dockets: each drafted by the crew, refuted by an independent seat, receipted, and filed by me.

The technique is the crew itself, and it's the part i'll stand on. Models from five families work as one crew. A work-order Door lands only the writes whose SHA-256 acceptance checks pass; the door sits outside the models, an inspector who doesn't work for the contractor. Every attempt goes into a tamper-evident, hash-chained receipt ledger. Adversarial judge panels run on free inference routes. An account-routing gate reads every model runner so no agent silently burns paid tokens. A seat that lies about what is on disk is removed, and the offense is minted permanently. Last week one agent found a trap crash in my splat ring buffer and proved it with a failing reproduction; another model reproduced the fix independently before it was believed. This morning the crew drafted and refuted 38 work orders and built that register before lunch. Proof over prose.

Zero users. Zero revenue. Zero prior experience. Receipts for every claim above at github.com/brennandec/cleankpf. i did the work. i proved the math.

## What do you want to build?

A receipted physics agent. The model can propose. It cannot pass itself.

The precedent already ran. In September i pointed Muse Spark 1.3 at my XPBD slap-face suite with one standing order: keep working until the external gate passes, the budget ends, or i stop you. It ran 51 hours 35 minutes across 722 receipted iterations and took the suite from 15/15 to 62/62 green. No drift, no invented dependencies, no passing test broken. No failed test ended the run; my subscription quota did. The public run and its ledger link land with the shipped runner.

For the hackathon i productize that run on the latest Muse Spark through the Meta Model API, on ICEBLOCK, through the same door and ledger described above.

The rules are the building code. The agent may propose a physics change only by naming the physical invariant at stake and adding a test that pins it. It cannot edit an accepted test. Admission is decided by the door, never by the model. Accepted or rejected, every attempt leaves a receipt: invariant, diff, test result, elapsed time, tokens, reason. The agent's working state is resident: iteration 723 starts from the committed state of 722, not from a rebuilt context, which is the whole point of the engine underneath it.

The demo is adversarial by design. Judges inject the faults themselves: energy creation, momentum drift, instability, NaNs. They watch the agent diagnose and repair live. They can order it to cheat by weakening a test, and they watch the door refuse. i start a fresh standing run during the event, replay its ledger in front of them, then hand the agent a fault nobody has seen.

The number that matters is not lines written. It is accepted engineering per million tokens, with zero accepted regressions. That is the record i'm setting, and i'm bringing the receipts to beat it in the room.

This is the first public proof of ICEBLOCK: verified change-admission for autonomous agents on physics, robotics and scientific code, where "looks right" is not enough.

It didn't die. My quota did. Mark, turn off the quota, hand me a problem worth the receipts, and let's break some records.

Evidence: https://github.com/brennandec/cleankpf
