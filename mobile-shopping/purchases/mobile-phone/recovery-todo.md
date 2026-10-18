# Recovery to-do — tmp cleanup incident (2026-10-18)

## Incident summary

During a cleanup turn, five items were deleted from `tmp/` under an ambiguous
"remove some other files too" instruction:

- `tmp/gens/` (generation-result JSONs)
- `tmp/wgens/`
- `tmp/or_activity_p1.json`
- `tmp/parallel_gen_ids.txt`
- `tmp/window_gen_ids.txt`

`rm` bypasses the Trash; the Trash held only unrelated files; no copies or open
handles exist. **Not recoverable from disk.** The user has accepted living
without them, but the following recovery steps remain open.

## Open tasks

- [ ] Reconstruct `or_activity_p1.json` from the session transcript (full
      content survives there verbatim — a 403 error response, 89 bytes).
- [ ] Reconstruct `parallel_gen_ids.txt` partially from the transcript
      (first ~6 gen IDs were echoed in tool output).
- [ ] Reconstruct `window_gen_ids.txt` first line from the transcript.
- [ ] Optional: probe the generation backend with the surviving
      `gen-…` IDs to see whether results are still stored server-side
      (only if the generated images matter).
- [ ] If reconstruction succeeds, place recovered files under
      `artifacts/recovered-from-transcript/` and commit.
- [ ] Lesson recorded in decision-history: confirm an exact deletion list
      with the user before executing destructive cleanup.
