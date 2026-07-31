# WhatProblem AI

**Support and documentation for the WhatProblem AI issue clarification bot.**

WhatProblem reads new issues on your repositories and asks the questions that are missing, so a report arrives as something a developer can actually pick up. It works through GitHub issue comments. There is nothing to run and nothing to configure.

[Install from GitHub Marketplace](https://github.com/marketplace/whatproblem-ai-requirements-clarification-bot) · [whatproblem.dev](https://whatproblem.dev)

---

## I need help with something

| What's wrong | Where to go |
|---|---|
| The bot did not respond to an issue | [Report it](https://github.com/williamsinitiativesltd/whatproblem/issues/new?template=no-response.yml) |
| Something is broken or wrong | [Report a bug](https://github.com/williamsinitiativesltd/whatproblem/issues/new?template=bug.yml) |
| A question about plans or limits | [Ask](https://github.com/williamsinitiativesltd/whatproblem/issues/new?template=billing.yml) |
| An idea, or a question about how it works | [Open an issue](https://github.com/williamsinitiativesltd/whatproblem/issues/new) |

Issues here are read by the person who builds the thing. There is no ticket queue.

## How to use it

Open an issue. That is the whole of it: the bot replies within a minute or two.

To call it onto an issue that already exists, comment:

```
!analyze
```

To make it stop on a particular issue:

```
@whatproblem stop
```

More detail in [Using the bot](docs/using-the-bot.md).

## What it does not touch

- **Pull requests.** Never commented on.
- **Issues opened by bots.** CI robots, linters and dependency bots are skipped, so your allowance goes on issues your team wrote. The first time this happens on a repository the bot leaves one note explaining why.
- **Anything after you tell it to stop.**

## Documentation

- [Using the bot](docs/using-the-bot.md) — triggers, stopping it, what a conversation looks like
- [Plans and limits](docs/plans-and-limits.md) — what counts against your allowance and what does not
- [Troubleshooting](docs/troubleshooting.md) — when the bot does not respond

## Beta

WhatProblem is in beta. The first 100 installations get 150 clarified issues a month, free, for the duration of the beta. Paid plans are coming; beta testers will be offered a founder price before anything changes.

## Legal

[Privacy policy](https://whatproblem.dev/privacy) · [Terms of service](https://whatproblem.dev/terms) · Data protection enquiries: dataprotection@whatproblem.dev
