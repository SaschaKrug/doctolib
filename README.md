# doctolib
This is a tiny library to check regular for new appointments in Doctolib.

# Quick Start
1. Clone this project: `git clone https://github.com/SaschaKrug/doctolib.git`
2. Install Python 3.12
3. Install python dependencies: `pip install -r requirements.txt`
4. Install Playwright dependencies `playwright install`
---
1. Go to the Doctolib website (https://doctolib.de).
2. Find and select the medical practice that corresponds to your needs.
3. Once you are on the appointment overview page, open the Developer Tools by pressing F11 on your keyboard.
4. In the Developer Tools, navigate to the Network tab.
5. Refresh the page by reloading it.
6. Look for a file named `availabilities.json` in the Network tab.
7. Click on the `availabilities.json` file to view its details.
8. Extract out of the URL of the file all parameters that are relevant for `main.py`:
  - visit_motive_ids
  - agenda_ids
  - practice_ids
  - telehealth
