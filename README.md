Interactive Study Plan Dashboard

A generic, single-page application (SPA) to track study progress across Physics, Organic Chemistry, and Inorganic Chemistry. It features dynamic charts, a customizable schedule, and cloud data persistence.

🚀 Quick Start (How to host on GitHub Pages)

1. Create the Repository

Create a new repository on GitHub.

Upload interactive_study_plan.html to the repository (rename it to index.html if you want it to be the home page).

2. Set up the Database (Firebase)

Since this app saves data, you need a free backend.

Go to Firebase Console.

Click Add Project and give it a name.

Once created, go to Build > Firestore Database and click Create Database.

Start in Test Mode (allows reading/writing for 30 days, easiest for personal projects).

Go to Build > Authentication.

Click Get Started.

Select Anonymous provider and enable it. (This allows the app to identify you without a login screen).

3. Connect the Code

In your Firebase Project Overview (Project settings), look for the </> icon to register a web app.

Copy the firebaseConfig object (it looks like a list of keys: apiKey, authDomain, etc.).

Open your index.html (or interactive_study_plan.html) file.

Scroll down to the script section (around line 320) and replace the placeholder values with your actual keys:

firebaseConfig = {
    apiKey: "AIzaSy...",
    authDomain: "your-project.firebaseapp.com",
    projectId: "your-project",
    ...
};


Commit/Save the changes to GitHub.

4. Enable GitHub Pages

Go to your GitHub Repository Settings.

Click on Pages in the left sidebar.

Under Branch, select main (or master) and save.

GitHub will give you a URL (e.g., https://yourusername.github.io/repo-name/).

🛠️ Features

Dynamic Charts: Visualizes lecture breakdown using Chart.js.

Edit Mode: Modify lecture counts and chapter names directly in the browser.

Cloud Save: Your progress is saved automatically to Firestore.

Responsive Design: Works on mobile and desktop.

📝 License

Free to use for personal study tracking.
