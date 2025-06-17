# TASK4-CHROME-EXTENSION-FOR-TIME-TRACKING-AND-PRODUCTIVITY-ANALYTICS

COMPANY:CODETECT IT SOLUTIONS

NAME:MANAL RUWAIDA

INTERN ID:CT04DN861

DOMAIN:FULL STACK

DURATION:4 WEEKS

MENTOR:NEELA SANTHOSH KUMAR

DESCRIPTION ON CHROME-EXTENSION-FOR-TIME-TRACKING-AND-PRODUCTIVITY-ANALYTICS:
The Chrome Extension for Time Tracking and Productivity Analytics is a lightweight yet powerful tool designed to help users understand how they spend their time online. It operates in the background of the browser to monitor user activity, track website usage, and generate productivity insights based on browsing behavior. This tool is especially useful for students, remote workers, freelancers, and anyone seeking to improve time management and reduce digital distractions.

By analyzing the time spent on each website and categorizing them into productive or unproductive tasks, the extension empowers users with meaningful data to make informed decisions about their daily habits.

🧱 Key Components and Their Functions
1. background.js
This script is the backbone of the extension. Running as a background process, it listens to browser events such as tab switching, tab activation, and browser idle states. Key responsibilities include:

Tracking active tabs and the URLs visited.

Recording time spent on each website.

Handling idle detection and pausing tracking when the user is inactive.

Storing and updating usage statistics locally (or sending to a backend for more complex analytics).

Resetting data daily or providing analytics based on custom time ranges.

The script uses Chrome's APIs such as chrome.tabs, chrome.windows, chrome.idle, and chrome.storage to manage and persist tracking data.

2. manifest.json
This file is the metadata blueprint of the extension. It defines how the extension behaves, what permissions it needs, and what scripts to load. Important entries in the manifest include:

"name", "description", and "version": Basic information about the extension.

"background": Specifies background.js as the script to run in the background.

"permissions": Requests necessary permissions like access to tabs, browsing history, and storage.

"icons": Links to the visual assets used in the extension toolbar and Chrome extension management UI.
