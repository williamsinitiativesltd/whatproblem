# Using the bot

## The normal case

Open an issue. WhatProblem reads it and replies within a minute or two with the questions it needs answered before the issue is actionable, along with a rough clarity score.

You do not have to answer. If the issue was already clear, the bot says so and leaves it alone.

## Calling it onto an existing issue

Comment any of these on an issue the bot has not already handled:

```
!whatproblem analyze
```

## Making it stop

Comment any of these and it will leave that issue alone:

```
!whatproblem stop
```

Stopping applies to that issue only. To bring the bot back to it later, comment `!whatproblem analyze`. Older command forms still work: see [Commands](commands.md).

To stop it everywhere, uninstall the app from **Settings → Applications → WhatProblem AI**, or remove individual repositories from the installation.

## What a conversation looks like

1. You open an issue.
2. The bot asks what is missing.
3. You reply.
4. The bot either asks a follow-up or decides it has enough.
5. When it has enough, it posts a summary of the clarified requirement.

It will not go past **five rounds** on one issue. If a conversation goes quiet for **24 hours** it closes itself, so it will not resurface days later.

## What it will not comment on

- **Pull requests.** Ever.
- **Issues opened by bots.** CI failures, lint reports, dependency updates. These are usually already actionable, and answering them would spend your allowance on issues no person is going to read. The first time a bot files an issue on one of your repositories, WhatProblem leaves a single note explaining this, then stays quiet.
- **Issues you have told it to stop on.**

## The clarity score

Each response carries a rough percentage. It is the bot's own estimate of how ready the issue is for someone to pick up, not a grade on your writing. A low score on a first pass usually means context that is obvious to you has not made it into the text.
