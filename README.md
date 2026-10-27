# DevSync — Daily Repository Updates

Automated GitHub repository maintenance using **GitHub Actions** to record scheduled activity, maintain daily logs, and demonstrate continuous workflow automation.

## Overview

DevSync is a lightweight automation project designed to keep a consistent record of repository activity through scheduled GitHub Actions workflows.

The workflow automatically creates or updates a daily Markdown log and commits the changes to the repository. This provides a simple, transparent example of scheduled automation, version control, and CI/CD practices.

## Features

- **Automated updates:** Runs on a predefined schedule using GitHub Actions.
- **Multiple daily runs:** Configured to run four times a day.
- **Daily activity logs:** Records automated maintenance activity in Markdown files.
- **Automatic commits:** Commits and pushes changes to the repository.
- **Manual execution:** Supports manual workflow runs through the GitHub Actions interface.
- **No external services required:** Uses GitHub Actions and Git for automation.

## Tech Stack

| Technology | Purpose |
|---|---|
| GitHub Actions | Workflow scheduling and automation |
| Git | Version control and commit management |
| Markdown | Daily activity logs |
| YAML | Workflow configuration |
| Ubuntu | Automation runner environment |

## Repository Structure

```text
devsync-daily-update/
├── .github/
│   └── workflows/
│       └── daily-commit.yml
├── daily-logs/
│   └── YYYY-MM-DD.md
└── README.md
```

Each daily log contains timestamped entries for automated repository maintenance.

## Automation Schedule

The workflow is configured for four daily runs:

| Time (IST) | Purpose |
|---|---|
| 9:00 AM | Morning update |
| 1:00 PM | Afternoon update |
| 5:00 PM | Evening update |
| 9:00 PM | Night update |

*Note: GitHub Actions scheduled workflows use UTC and may occasionally start later than their scheduled times.*

## Getting Started

### 1. Fork or clone the repository

```bash
git clone https://github.com/debmalyaSanyal/devsync-daily-update.git
cd devsync-daily-update
```

### 2. Enable GitHub Actions

Open the repository on GitHub, navigate to **Actions**, and enable workflows if prompted.

### 3. Check the workflow

Open `.github/workflows/daily-commit.yml` and verify the schedule and workflow permissions.

The workflow needs write permission for repository contents to create and push commits.

### 4. Run manually

If manual execution is enabled, navigate to **Actions → Daily Repository Updates → Run workflow**.

### 5. Monitor executions

Check the Actions tab to review workflow runs, execution logs, and any failures.

## What I Learned

This project provides practical experience with:

- Automating repetitive development tasks.
- Configuring scheduled GitHub Actions workflows.
- Managing repository permissions securely.
- Creating and maintaining structured Markdown logs.
- Automating Git commits and pushes.
- Monitoring workflow execution and troubleshooting failures.

## Future Improvements

- Add workflow failure notifications.
- Generate weekly or monthly activity summaries.
- Add automated validation and repository health checks.
- Track workflow success rates and execution history.

## Author

**Debmalya Sanyal**

- GitHub: [@debmalyaSanyal](https://github.com/debmalyaSanyal)
- LinkedIn: [Connect with me](https://www.linkedin.com/in/debmalya-sanyal-19b0b1248/)

---

If you find this repository useful as a reference for GitHub Actions automation, feel free to explore the workflow and adapt it to your own projects.
