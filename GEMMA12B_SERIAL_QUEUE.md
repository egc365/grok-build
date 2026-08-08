# Gemma 12B Serial Experiment and Test Queue

Status: queued; owner interactive test pending.

Run exactly one item at a time. Record the model digest, input locator,
commands, output hash, measured result, and pass/fail receipt before advancing.
Stop the queue on failure. Do not promote generated work from this queue.

- [ ] **Q01 — Owner interactive smoke test.** Select `gemma4-12b:latest` and
  confirm Grok exposes its native tool catalog.
- [ ] **Q02 — Native read/search test.** Locate repository instructions and one
  exact source file without mutation.
- [ ] **Q03 — Native terminal test.** Run one bounded read-only command and
  capture its exit status.
- [ ] **Q04 — Scratch write test.** Create and revise one explicitly disposable
  file; verify path enforcement and cleanup.
- [ ] **Q05 — Qwen retrieval test.** Call `/wiki/gemma-search` through Grok's
  terminal tooling and verify compact cited results.
- [ ] **Q06 — Full SQLite search experiment.** Inventory allowed tables, define
  row grains, and test Qwen-boosted retrieval on a read-only snapshot.
- [ ] **Q07 — Report double-check experiment.** Extract claims, retrieve
  evidence, check arithmetic, paths, and hashes, and emit a contradiction table.
- [ ] **Q08 — Tunable parser experiment.** Run one versioned JSON Schema
  extraction profile and measure validity plus field accuracy.
- [ ] **Q09 — Controlled write experiment.** Draft with Gemma, validate
  deterministically, and submit only an owner-gated candidate.
- [ ] **Q10 — Grok comparison.** Compare native Grok against Grok driven by
  local Gemma 12B on the same bounded task set.
- [ ] **Q11 — Claude Code adapter experiment.** Enforce the same router through
  permissions and pre-tool hooks.
- [ ] **Q12 — Google Gemini CLI adapter experiment.** Enforce the same router
  through sandbox, policy, and hooks.
- [ ] **Q13 — Final replay.** Rerun all passing cases from cold processes and
  publish the evidence matrix for owner review.
