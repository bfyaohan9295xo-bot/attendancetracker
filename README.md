# Class Attendance Tracker

A lightweight, no-build attendance tracker that runs as a static web page. The repository contains fictional demo students so it can be shared publicly without publishing a real class roster.

## Features

- Weekly attendance by subject, with Present (P), Tardy (T), Absent (A), Excused (E), Holiday (H), and Suspension (S) statuses.
- Monthly and quarterly tardy and absence summaries.
- A behavioral observation log.
- CSV export and print-to-PDF controls.
- Browser `localStorage` persistence; no server or external library is required.

## Run locally

Open `index.html` in a modern browser. There is no build step or dependency installation. For a local web server, run `python -m http.server 8000` from this directory and visit `http://localhost:8000`.

## Publish with GitHub Pages

1. Create a GitHub repository and add these files at the repository root.
2. In **Settings → Pages**, choose **Deploy from a branch**, select `main` and `/ (root)`, then save.
3. Open the Pages URL GitHub provides.

## Customize

- Edit the `students` array near the top of the script in `index.html`. Replace the demo names and sex values with the roster you are authorized to use.
- Edit the `schedule` object to match the school days and subject names. JavaScript day numbers use Sunday = `0`, Monday = `1`, through Saturday = `6`.
- Adjust the quarter date ranges in `quarter()` and the action thresholds in `action()` if your reporting rules differ.

## Data and privacy

Attendance and behavior entries are stored in the browser's `localStorage` on the device and browser where the page is opened. They are not synchronized between users or devices. Clearing browser site data can remove saved entries. This page has no sign-in, access controls, or server-side backup. Do not put real student names or records in a public repository or publish the hosted page for public access. Keep any real roster and records in a private, access-controlled copy and follow your school's data-protection procedures.

## License

No license is included. Add a license only after deciding how you want others to use and distribute the project.
