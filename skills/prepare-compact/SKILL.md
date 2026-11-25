---
name: prepare-compact
description: When the user types /compact, "compact" or "clean up" in any conversation - tidy the tracking file, archive what is done and keep only what matters before they run /compact.
---

# Prepare a compaction (/compact)

Claude cannot run /compact itself: only the user can type the command. This skill tidies the conversation's tracking so compaction loses nothing useful.

Works for any conversation.

## Steps

1. Read the conversation's tracking file in the project or repo (dated list, state, plan).
2. Archive the full version before any change (local copy or dated `...-archive-YYYY-MM-DD` file).
3. Rewrite the list in four blocks:
   - **Standing rules**: every instruction still valid, duplicates merged.
   - **Today's state**: what is in progress or scheduled, with the useful IDs.
   - **Dated actions**: only what remains to do.
   - **Waiting on**.
   Remove: reports already done, finished tasks, outdated technical details.
4. Put the update date and the archive name at the top, then save.
5. Compare with the archive: no instruction and no future deadline may be missing.
6. Reply in three lines: what was archived, what was kept, then "You can type /compact, nothing useful will be lost."

## Rules

- Never delete a user instruction or a future deadline.
- No external action during the cleanup.
