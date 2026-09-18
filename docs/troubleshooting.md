# When the bot does not respond

Work down this list. The first three cover almost everything. Each one says what to check;
[how it works](https://whatproblem.dev/using-the-bot) says why.

### 1. Was the issue opened by a bot?

WhatProblem skips issues from CI robots, linters and dependency bots (`github-actions[bot]`,
`renovate[bot]`, Copilot and similar), so your allowance goes on issues your team wrote. A note
explains it when it happens, at most once a month per repository.

You can still call the bot onto one of those issues yourself: comment `!whatproblem analyze`.

### 2. Is it a pull request?

The bot never comments on pull requests, including the comment threads on them. Nothing you
type there reaches it.

### 3. Is the repository actually included in the installation?

The app can be installed on a subset of repositories. Check
**Settings → Applications → WhatProblem AI → Configure** and confirm the repository is in the list.

### 4. Has someone told it to stop on that issue?

A comment containing `!whatproblem stop` anywhere in the thread ends it for that issue. Scroll
the thread. To undo it, comment `!whatproblem analyze`. Stopping is per issue, so this tells you
nothing about the rest of the repository.
[Every command is on one page.](https://whatproblem.dev/commands)

### 5. Had the thread been quiet for more than 24 hours?

If the last activity on the issue was over a day before your comment, the bot treats the
conversation as finished and your comment gets no reply. Comment `!whatproblem analyze` to pick
it up again, which works whatever the gap.

### 6. Have you used up the month's allowance?

The bot posts a note on the issue when this happens, so check whether one appeared.
[What counts against an allowance.](https://whatproblem.dev/plans-and-limits)

### 7. Still nothing

Then it is us, and we want to know. GitHub does not retry a webhook it has already delivered, so
a response we fail to send is gone: nothing will arrive later, and we are not told it happened.

[Email us.](mailto:support@whatproblem.dev) A link to the issue and the account it is installed on
is enough to start. We look this one up in our own logs, so it goes to us privately rather than
into the public tracker.
