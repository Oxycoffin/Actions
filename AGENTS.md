# Project Notes

This repository stores GitHub Actions used to automate daily tasks for the Nautica application.  The workflows live under `.github/workflows`.

Workflows included:
- `daily-reminders.yml` triggers reminder jobs each day at 16:00 UTC and can be run manually.
- `daily-report.yml` runs the daily report each day at 16:15 UTC and can be triggered manually.
- `daily-db-backup.yml` runs the database backup every day at 02:00 UTC and uploads the response log.
- `ping-main.yml` pings the main website every minute to keep the service awake.

Local development with `pnpm dev` will fail because the MongoDB server is not available in this environment, so do not attempt to run it here.
