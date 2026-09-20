# Todo Schedule

A lightweight personal daily planner built with HTML, CSS, and vanilla JavaScript.

## Features

- Daily schedule with a clear timed-task timeline
- Seven-day date navigation and a quick Today action
- Start and end times with validation
- Unscheduled and overdue task sections
- Daily completion progress
- Low, medium, and high priority
- Search, status filters, and sorting
- Add, edit, duplicate, complete, and delete tasks
- LocalStorage persistence with safe legacy-data normalization
- JSON import and export
- Responsive dark interface

## Live Demo

https://tranvanquyet04.github.io/todo-list/

## Run locally

From the project directory, run:

```bash
python -m http.server 4173
```

Then open `http://127.0.0.1:4173/`.

## Data migration

Existing tasks saved under `todo.v1.items` are normalized automatically. Legacy fields such as `text`, `done`, `due`, and `dueDate` are mapped to the new schedule model while existing IDs are preserved. Before the first migrated save, the original payload is backed up once under `todo.v1.items.legacyBackup`.

LocalStorage is scoped to each browser origin. Data saved while opening the app with `file://` cannot automatically appear on the HTTPS live site. Use Export in the old app, then Import on the live site to move those tasks.
