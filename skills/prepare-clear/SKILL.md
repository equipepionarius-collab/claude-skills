---
name: prepare-clear
description: When the user types /clear, "clear" or "let's start over" in any conversation - save everything to a state file first so the work can resume after the reset.
---

# Prepare a reset (/clear)

Claude cannot clear the conversation itself: only the user can type /clear. This skill makes sure nothing useful is lost after /clear and that a new conversation can pick the work back up.

Works for any conversation (code, sales, website, content, case files).

## Steps

1. Find the conversation's tracking file (dated list, state, plan) in the project or repo. If there is none, create one: `state-<topic>.md`.
2. Write a complete, self-contained resume state in it:
   - **Rules and instructions** given by the user (all of them, including the "don'ts").
   - **Current state**: what is done, delivered, scheduled, in progress, with useful links, IDs and paths (files, branches, campaigns, documents).
   - **Remaining dated actions**, nearest first.
   - **Waiting on**: replies, approvals.
   - **How to resume**: the exact sentence to say in a new conversation (e.g. "read state-<topic>.md then do what's next").
3. If the file already existed, archive the old version (dated copy), then save the new one.
4. Re-read the saved file and check that no instruction or deadline disappeared.
5. Reply in three lines: where the state is saved, the resume sentence, then "You can type /clear."

## Rules

- No external action (sending, publishing, deleting) during this skill.
- Never summarize an instruction to the point of changing its meaning.
- Short sentences, in the user's language.
