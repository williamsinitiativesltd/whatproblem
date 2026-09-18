# Commands

Every command, what stopping applies to, and what the bot does without being asked:

**[whatproblem.dev/commands](https://whatproblem.dev/commands)**

That page is the one the bot itself links to from every comment it posts, so it is the
version that gets kept right. This file used to hold a second copy and the two drifted:
it described a 24 hour timer that does not exist (nothing happens at the 24 hour mark;
the next comment on the issue is what checks), and it said commands are never read on
issues opened by bots, when in fact a person can call the bot onto one of those issues
and it will answer.

The short version, if you only need the two commands:

| Command | What it does |
|---|---|
| `!whatproblem analyze` | Read this issue now and ask what is missing. Also brings the bot back to an issue it has stopped on, or already finished with. |
| `!whatproblem stop` | Leave this issue alone. Applies to that issue only, not the repository or the account. |
