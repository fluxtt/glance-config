# glance-config

This repository contains a Glance dashboard configuration and a small deployment helper script.

## Contents

- `glance.yml` - Glance dashboard configuration file, defining theme, branding, pages, and widgets.
- `remote_update.bat` - Windows helper script to copy `glance.yml` to a remote server using `scp`.

## Purpose

This repo is used to manage a Glance dashboard setup for a personal homelab and security/dev monitoring view.
The configuration includes widgets for clock, weather, services, Docker containers, bookmarks, Hacker News, and security RSS feeds.

## Usage

### Local edits

1. Edit `glance.yml` to update the dashboard layout, widgets, links, and data sources.
2. Save your changes.

### Deploy to remote Glance instance

Update `remote_update.bat` with the correct remote host, username, and destination path if needed.

Run the script from PowerShell or Command Prompt:

```bat
remote_update.bat
```

This uses `scp` to copy the local `glance.yml` file to the configured remote destination.