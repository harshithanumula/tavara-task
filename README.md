What This Workflow Does
Trigger

Runs every time a push occurs to the dev branch.

 Merge Logic

Checks out main

Fetches branch dev

Runs git merge dev

If merge fails → abort and exit with clear log

If merge succeeds → commits and pushes

Provides messages for:

Successful merge

Merge conflict

Push status

Auto-resolve trivial conflicts

Multiple branch merge chains (e.g., feature → dev → staging → main)
