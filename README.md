# Todo List

A calm, responsive personal task manager built with HTML, CSS, and vanilla JavaScript.

## Features

- Add, edit, duplicate, complete, and delete tasks
- Due dates and priority levels
- Search and All / Active / Done filters
- Newest, oldest, and due-date sorting
- Bulk toggle and clear-completed actions
- LocalStorage persistence
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

LocalStorage is scoped to each browser origin. Data stored by a `file://` version does not automatically transfer to the deployed HTTPS site. Export tasks from the old version and import the JSON file into the live site when migration is needed.
