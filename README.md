# Scheduler

A simple daily planner: one row per hour, with tasks that can span several hours, tags, recurring commitments and suggestions. You choose the start and end of each day.

## Download

**[Apple Silicon (M1, M2, M3, M4)](https://github.com/simone-nicholas/Scheduler/releases/latest/download/Scheduler-1.0.0-arm64.dmg)**

Open the `.dmg` and drag Scheduler into Applications. On first launch, right-click the app and choose _Open_.

Intel Macs are not supported yet.

## Features

- **Hour-by-hour plan.** Each day has its own start and end hour.
- **Multi-hour tasks.** Set a task to last 1 to N hours. The rows below it show as one block.
- **Tags.** Add tags to a task. Tags appear only while the task row is selected.
- **Suggestions.** One editable list, used both as tasks and as tags. Tap one to add it to the first free hour.
- **Recurring commitments.** Set an hour and a name once. They fill in automatically at the start of each new day.
- **Day navigation.** Move between days, or jump back to today.
- **Language and theme.** English or Italiano, with Light, Dark or System theme.
- **Local storage.** Everything is saved on your device. No account and no internet connection needed.

## Run in the browser

Open `index.html` in any modern browser.

## Run as a macOS app

Requires [Node.js](https://nodejs.org/) (LTS).

```bash
npm install
npm run start   # open the app for testing
npm run dist    # build a .dmg in the dist folder
```

The app is built with [Electron](https://www.electronjs.org/) and is not signed. On first launch, right-click the app and choose _Open_.

## Project structure

- `index.html`: the whole interface (HTML, CSS and JavaScript in one file).
- `main.js`: starts the Electron window.
- `package.json`: project settings and build configuration.

## Data

Data is stored in the browser or app storage on the device where you use it. Data from the browser is not shared with the macOS app, and vice versa.