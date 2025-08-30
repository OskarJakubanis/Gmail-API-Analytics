# 📧 Gmail Sender Analytics

A Google Apps Script project that leverages the Gmail API within **Google Workspace** to automate the collection and aggregation of email senders into a pivot table using Google Sheets.  
This solution has already been tested by several of my friends, and they are very satisfied with the results. 🎉


## 🎯 Purpose

Collect all incoming email addresses from Gmail, store them in a Google Sheet, and generate a pivot table with the number of emails per sender. This allows you to:

1. 📌 Quickly identify frequent senders
2. 📝 Perform further analysis for managing email rules
3. 🗂️ Organize emails into folders
4. 🚫 Unsubscribe from unwanted newsletters
5. ❌ Block unwanted senders

## ⚙️ How it works:

1. Google Apps Script reads the sender emails from your Gmail inbox in batches and stores them in the **RAW\_DATA** sheet.
2. A pivot table in the **PIVOT** sheet counts occurrences of each sender.
3. The data is ready for analysis by you or your team.

## 💡 Notes

* The script shows a warning when you run it and requires you to accept access; however, it is safe and only counts the sender emails.
* Processes around **536 emails per minute**.
* Maximum execution time is **6 minutes**, so the script uses **batch processing with triggers** to continue automatically in JavaScript.

## 🚀 How to Run:

1. Open this link and copy the file to your own drive (it contains two sheets: one for **raw data** and one for the pivot table):  
https://docs.google.com/spreadsheets/d/1-xg-B5SdTGIaWgvkJ9Qu7cRGGpNMuOqSuDG-Dd--Zgg/edit?usp=sharing
2. Open the copied Google Sheet → Extensions → Apps Script and click **Run**.
3. Give access to Apps Script to access your Gmail account 
4. Wait for the script to process your emails — it imports around **500 emails per minute**, so total time depends on the number of emails in your inbox.
5. Check the pivot sheet once the process is completed to review high-frequency senders.

## 🛠️ Requirements:

* Gmail account
* Google Sheets (on Google Drive, not locally)
* Google Apps Script (built into Sheets)

## 📬 Contact

Questions, suggestions or want to collaborate? Open an issue or connect directly.
