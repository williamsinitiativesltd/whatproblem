# Commands

Comment any of these on an issue. They work anywhere in the comment, and the case does not matter.

| Command | What it does |
|---|---|
| `!whatproblem analyze` | Read this issue now and ask what is missing. Also brings the bot back to an issue it has stopped on, or already finished with. |
| `!whatproblem stop` | Leave this issue alone. |

## Commands apply to one issue

Stopping is per issue. It is not per repository and not per account, so stopping on issue #12
changes nothing about #13.

To stop it everywhere, remove repositories from the installation or uninstall from
**Settings → Applications → WhatProblem AI**.

## Bringing it back

`!whatproblem analyze` on an issue the bot has stopped on, or has already summarised, starts a
fresh pass: the round count goes back to zero and it picks the issue up as if for the first time.

This costs nothing extra. An issue counts once against your monthly allowance however many times
it is picked up. See [plans and limits](plans-and-limits.md).

## What it does without being asked

- Reads any new issue within a minute or two and asks what is missing.
- Carries on for at most **five rounds** on one issue.
- Ends by posting a summary of the clarified requirement.
- Closes a conversation that has gone quiet for **24 hours**, so it will not resurface days later.
- Bows out early and posts the summary if the issue is already clear enough, or if the
  conversation has plainly run its course.

## Where commands do nothing

- **Pull requests.** The bot never comments on them, so nothing you type there reaches it.
- **Issues opened by bots.** Skipped before any command is read.

## Older forms

These still work, because people learned them and comments outlive documentation:

`!analyze` · `!whatproblem` · `@whatproblem analyze` · `@bot stop` · `stop analyzing this issue`

One word on the `@whatproblem` forms: **`@whatproblem` is an unrelated GitHub user's account.**
Typing it in a public repository sends that person a notification and has never been how the bot
hears you, so please use the `!` forms. `@bot stop` is generic enough that it can silence us when
you meant a different bot.
