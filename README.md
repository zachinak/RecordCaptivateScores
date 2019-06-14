# RecordCaptivateScores
A Javascript and Google Apps Script project to record scores from captivate training modules to a Google Sheet.

Required apps: Google Sheets and Adobe captivate

A brief summary of usage:
On the Google Sheets side - The Google Sheet "catches" the data sent by Captivate. First, create a new sheet. Go to the script editor. Copy and paste the code from the Google Apps Script file into the script editor. Publish the script as a web app (allowing any required permissions). Drop down the "Run" menu -> Run Function -> click "setup" to run the setup function to properly set up your sheet. After the the setup function has run, go back to the data view of your sheet and create a new sheet within the Google Sheets document called "Emails". On the Emails sheet write "List of Emails to Notify" in A1. In the A column (Starting in A2) list any emails that should receive notifications, one email per row.

On the captivate side - Trigger a javascript action and include the code from the captivate javascript file in the action. Be sure to set the captivate project name and be sure to assign the proper variables so that there is data to send. The variables are listed in the Javascript file. 
