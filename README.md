# ExpenseFlow – Personal Expense Tracker (Offline First)

A lightweight, privacy-focused personal daily ledger built with Vanilla HTML, CSS and JavaScript. Designed to track daily spend on Indian payment modes with Zero backend servers. Optional Single file Google Drive cloud backup.


**Live App:** [https://mdnihalaalum.github.io/ExpenseFlow](https://mdnihalaalum.github.io/ExpenseFlow)

--- ## Main Features


- **Offline-First Local Storage:** Stores all budgets and expenses instantly in browser `localStorage`—no internet or sign-in required.

- **Payment Tracking in multiple modes**: Separate tracking of expenses in **Cash, UPI Lite and UPI Bank Account**.

- **Smart Monthly Budgets & Rollover:** Set a `Set / Replace` base limit, `Reset Budget` and allows for mid-month `+ Add Funds`, automatically rolling over unspent balances or deficits from prior months.
**Category Breakdown & Filters:** Live search with filtering by month, category and payment channel with visual percentage bars for each category.

- **Optional Google Drive Sync (`drive.file`):** Connects to your Google Drive using Google Identity Services (OAuth 2.0) and syncs a single, compact `expense.json` file. No other files in your Drive are touched.
- **Light & Dark Themes + CSV Export:** Defaults to a clean Light Mode with a persistent Dark Mode toggle and one-click `.csv` export.
--- 

## Architecture & Privacy

- **No-Server Architecture:** No database or third-party analytics back end. Your financial records stay on your device unless you manually connect to Google Drive.
- **Least-Privilege Drive Isolation:** Uses the `https://www.googleapis.com/auth/drive.file` scope, restricting the app to read/update only the one `expense.json` file it creates.
- **Compact Storage:** Reduces transaction JSON keys to single letters to keep cloud backups small (~60% smaller)

---

## Technology Stack
- **Frontend:** HTML5, CSS3 (CSS Custom Properties, CSS Grid/Flexbox), Vanilla JS (ES6+)
- **Authentication & Cloud Storage:** Google Identity Services (OAuth 2.0), Google Drive REST API v3- **Hosted by:** Github Pages

--- 

## About the Author

Developed by **Muhammed Nihal Aalum**  
GitHub: [@mdnihalaalum](https://github.com/mdnihalaalum)(https://github.com/mdnihalaalum)
