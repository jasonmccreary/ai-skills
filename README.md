# Shift AI
A set of AI skills and commands for managing the entire [Shift](https://laravelshift.com) process. Determine what Shift needs to be run, open a PR, and review it for additional automation all from your AI of choice.

## Installation
There are multiple ways to install these skills and commands.

If you primarily use Claude Code, we recommend installing the plugin. Otherwise, you may install through _Laravel Boost_ or `npx`.

### Claude Code
Add the marketplace and install globally by running:

```
/plugin marketplace add laravel-shift/shift-ai
/plugin install shift@laravel-shift --scope user
```

The `--scope user` flag installs the plugin once for your entire system — no per-project setup needed.

### Laravel Boost
You may also install via [Laravel Boost](https://laravel.com/ai/boost) by running:

```sh
php artisan boost:add-skill laravel/shift-ai --skill shift
```

### NPX Skills
You may also install via [Skills](https://www.skills.sh/) by running:

```sh
npx skills add laravel-shift/shift-ai
```

## Commands
- `/shift:analyze` — analyze your project and determine the next Shift to run
- `/shift:run` — trigger a Shift to run against your current repository
- `/shift:review` — review and process the Shift PR for additional automation
- `/shift:refactor` — run a [Shift Workbench](https://laravelshift.com/workbench) task to refactor your code

## Requirements
The `/shift:run` and `/shift:refactor` commands use the [Shift API](https://laravelshift.com/shift-api). As such, they require a Shift API token. You may sign into [Shift](https://laravelshift.com) to generate one.

The `/shift:review` command interacts with Shift changes through Git. If your repository is hosted with GitHub, the [`gh`](https://cli.github.com) utility is required.
