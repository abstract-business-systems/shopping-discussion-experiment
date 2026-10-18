# Events log

Significant incidents and decisions during this project, newest last.

## 2026-10-18 — tmp cleanup permanently deleted five files (incident)

- **What happened:** during a tmp/ cleanup turn, five items were permanently
  deleted with `rm -rf`: `tmp/gens/`, `tmp/wgens/`, `tmp/or_activity_p1.json`,
  `tmp/parallel_gen_ids.txt`, `tmp/window_gen_ids.txt` (leftovers of an earlier
  image-generation experiment).
- **Why it matters:** the deletion ran under an ambiguous instruction
  ("remove some other files too") without confirming the exact list with the
  user; `rm` bypasses the Trash, so nothing was recoverable from disk.
- **Impact:** generation-experiment results are lost. The user accepted the
  loss. Partial contents survive in the session transcript if ever needed.
- **Resolution:** incident recorded; artifacts (11.6 MiB session zip + 17
  browser evidence screenshots) committed in `artifacts/` (commit 33caf37).
- **Corrective action:** a safe-deletion workflow is now planned — see
  `safe-deletion-todo.md`. Until it exists, deletions require an explicit,
  user-confirmed file list.
