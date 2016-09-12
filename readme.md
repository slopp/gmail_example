Steps to Recreate Analysis:
1. Go through Pre-reqs
2. Run gmailr_pull.Rmd (Takes a long time)
3. Run gmail_exploration_results.Rmd


Pre-Reqs:

* Pick a project name; referred to as `PROJ-NAME` from now on.
* Register a new project at <https://console.developers.google.com/project>.
* From Overview screen, look at Google Apps APIs and select the Gmail API. Enable it.
* Click "Go to Credentials" or navigate directly to Credentials.
* You want a get a client ID and will need to "Configure consent screen".
  - The email should be pre-filled. Enter `PROJ-NAME` as Product name. Other fields can be left blank.
* Returning to the "client id" process:
  - Application Type: "Other"
  - Enter `PROJ-NAME` again as the name.
  - Click "Create"
* Client id and secret will appear in a pop-up which you can dismiss via "OK". Instead use download icon at far right of your project's listing to download a JSON file with all of this info. Move to an appropriate location and consider renaming as `client-secret.json`.
* Install gmailr: install.packages("gmailr")
* Copy the .Rmd files
