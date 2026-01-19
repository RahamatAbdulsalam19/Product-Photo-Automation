# Product Photo Automation
## Project Overview

This project was delivered to automate your product image enhancement workflow and eliminate the repetitive, time-consuming process of manually cleaning up product photos.

The system is fully integrated with Google Drive and Remove.bg via the Make (Integromat) automation platform. It automatically processes every new image uploaded to your designated folder, enhances it, and saves the final version with clean naming conventions. A structured log is also maintained in Google Sheets for easy tracking, performance monitoring, and accountability.

The goal: faster uploads, consistent visuals, and less manual editing.

## How the System Works

Trigger – When new images are added to the Input Google Drive folder, the automation is triggered automatically.

Enhancement – Each image is sent to the Remove.bg API for background removal and light cleanup. (Can be extended to styled prompts or additional background variations if needed.)

Upload – Enhanced images are saved to the Output folder with a standardized, timestamped file naming structure.

Logging – Every processed image is logged in a Google Sheet with:

Timestamp

Source file name

Output file name

Enhancer used

Status (Success/Error)

Drive link to the enhanced file

## Tools & Integrations

Google Drive – File storage, input and output folders

Remove.bg API – Automated background removal and image enhancement

Make (Integromat) – Orchestration and workflow automation

Google Sheets – Logging and reporting layer

## Key Features Delivered

Hands-free processing — No manual uploads or editing required after initial setup.

Consistent file quality — All enhanced images follow the same background and format standard.

Clean file structure — Automatic timestamped naming ensures zero filename conflicts.

Full tracking — A Google Sheet captures every run, including failures, for transparency and easy troubleshooting.

Failure handling — If an image fails to process (e.g., unsupported file type), it’s logged separately and can be retried.

## Maintenance Notes

To add new team members, simply grant them access to the Input and Output Drive folders.

API key is securely stored in Make and not visible in the workflow interface.

Any failed image processing events will be flagged in the Google Sheet with a red Error status.

Optional: You can add Slack or email notifications later if you want real-time alerts.
