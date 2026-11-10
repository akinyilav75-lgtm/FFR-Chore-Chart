# FFR Chore Manager (simple static app)

## What it does
- Add and remove active residents.
- Generate a proposed two-week chore cycle.
- Preview each resident's previous zone before confirming.
- Reduce repeated assignments using each resident's assignment history.
- Confirm before publishing a new cycle.
- Mark current chores complete.
- Print the current resident chart.
- View fairness counts and previous cycles.
- Set a browser reminder.

## Important limitations
This version stores data in the browser's local storage on one device. It does not sync between Jill and other administrators. Export the JSON backup regularly using the button in the app.

Browser notifications are best-effort and require the app to be open around the reminder time. A static GitHub Pages site cannot reliably send push reminders while closed. For a simple reliable reminder, create a recurring calendar event for every other Monday. A future shared version would need a small database and scheduled service.

## Easiest hosting: GitHub Pages
1. Sign in to GitHub and create a new repository, e.g. `ffr-chore-manager`.
2. Upload `FFR_Chore_Manager_v2.html`.
3. Rename the uploaded file to `index.html`.
4. Open the repository's **Settings → Pages**.
5. Under **Build and deployment**, choose **Deploy from a branch**.
6. Select branch `main`, folder `/ (root)`, then Save.
7. GitHub will provide a public website URL. Open it and bookmark it.

Anyone with the link can open the site, but each browser/device has its own separate saved data. Do not put sensitive resident information in this public static app. Use resident first names only if appropriate for your organization's privacy practices.

## Backups
Use **Export backup (JSON)** from the app and store the backup in a secure location. Do not share it publicly; it contains resident names and operational history.
