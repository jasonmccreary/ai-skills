# Shift - Commands for AI
A set of Claude Code commands for automating the entire [Shift](https://laravelshift.com) process. Determine what needs to be run, open a PR, and review it for additional automation.

## Installation
To use these commands, you may add the marketplace and install globally with Claude Code:

```
/plugin marketplace add jasonmccreary/ai-skills
/plugin install laravel-shift@laravel-shift --scope user
```

The `--scope user` flag installs the commands once for your entire system — no per-project setup needed.

## Commands
- `/shift-analyze` — analyze your project and determine the next Shift to run
- `/shift-run` — trigger a Shift to run against your current repository
- `/shift-review` — review and process the Shift PR for additional automation
- `/shift-workbench` — run a [Shift Workbench](https://laravelshift.com/workbench) task to refactor your code

**Note:** These commands are being beta tested. As such, the `/shift-run` command is currently limited to subscribers of a [Shifty Plan](https://laravelshift.com/shifty-plans). Once tested, these commands will be made available to all Shift users.
