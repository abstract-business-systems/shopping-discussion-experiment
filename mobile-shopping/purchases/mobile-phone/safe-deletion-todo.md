# Safe-deletion to-do — prevent permanent-loss deletions

Created: 2026-10-18 (after the tmp cleanup incident — see events.md)

Goal: every future deletion inside project and tmp areas must move files to the
Trash instead of permanently removing them.

## Tasks

- [ ] Verify `gio trash` works for both the project directory and `tmp/`
      (GNOME/GIO is present on this desktop; confirm it creates
      `~/.local/share/Trash/files` entries with restore info).
- [ ] Create a small `safe-delete` helper (script or shell function) that:
      - takes one or more paths,
      - calls `gio trash` on each,
      - prints exactly what was trashed,
      - refuses to run without an explicit file list (no globs silently expanded).
- [ ] Adopt the convention in this workspace: **no bare `rm -rf` on user files**;
      only `safe-delete` (or `gio trash`) for anything not generated this turn.
- [ ] For machine-generated scratch that is safe to remove (e.g. logs created
      in the same turn), still prefer trashing, or state explicitly in the reply
      what is being permanently removed and get a one-word confirmation.
- [ ] Record the helper location here once created, and add it to the
      project README so future sessions discover it.
- [ ] Periodically empty the Trash only after confirming nothing trashed in
      the last 30 days is needed.

## Not in scope

- Reconstructing the five deleted tmp files (user accepted the loss; partial
  contents remain in the session transcript if ever needed).
