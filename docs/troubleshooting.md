# When the bot does not respond

Work down this list. The first three cover almost everything.

### 1. Was the issue opened by a bot?

WhatProblem skips issues from CI robots, linters and dependency bots (`github-actions[bot]`, `renovate[bot]`, Copilot and similar). This is deliberate: it keeps your allowance for issues your team wrote.

The first time it happens on a repository, the bot leaves one note saying so, then stays quiet about it.

### 2. Is it a pull request?

The bot never comments on pull requests, including the comment threads on them.

### 3. Is the repository actually included in the installation?

The app can be installed on a subset of repositories. Check **Settings → Applications → WhatProblem AI → Configure** and confirm the repository is in the list.

### 4. Has someone told it to stop on that issue?

A comment like `!whatproblem stop` anywhere in the thread ends it for that issue. Scroll the thread. To undo it, comment `!whatproblem analyze`.

### 5. Is the conversation older than 24 hours?

Conversations close themselves after a day of silence, so a reply to a two-day-old thread will not wake it. Comment `!whatproblem analyze` to start again.

### 6. Have you used up the month's allowance?

The bot posts a note on the issue when this happens, so check whether one appeared. See [Plans and limits](plans-and-limits.md).

### 7. Still nothing

Then it is us, and we want to know. GitHub does not retry a webhook it has already delivered, so a response we fail to send is gone: nothing will arrive later, and we are not told it happened.

[Email us.](mailto:support@whatproblem.dev) A link to the issue and the account it is installed on is enough to start. We look this one up in our own logs, so it goes to us privately rather than into the public tracker.
