# 📧 Mail\_Counter

A Google Apps Script project that automates the collection and aggregation of Gmail senders into a pivot table using Google Sheets.

---

## 🎯 Purpose

Collect all incoming email addresses from Gmail, store them in a Google Sheet, and generate a pivot table with the number of emails per sender. This allows you to:

1. 📌 Quickly identify frequent senders
2. 📝 Perform further analysis for managing email rules
3. 🗂️ Organize emails into folders
4. 🚫 Unsubscribe from unwanted newsletters
5. ❌ Block unwanted senders

---

## ⚙️ How it works:

1. Reads email addresses from your Gmail inbox in batches
2. Only the sender's email is stored in the RAW\_DATA sheet
3. Pivot table in the PIVOT sheet counts occurrences of each sender
4. The data can be used to create Gmail filters, organize emails into folders, unsubscribe, or block unwanted senders

---

## 🚀 How to Run:

1. Copy the file **checkup\_data.gsheet** (it contains two sheets: one for **raw data** and one for the pivot table).
2. Open Google Sheets → Extensions → Apps Script and run the script (it is already included in the file).
3. Wait for the script to process your emails — it imports around **500 emails per minute**, so total time depends on the number of emails in your inbox.
4. Review the pivot table to identify high-frequency senders.

---

## 🛠️ Requirements:

* Gmail account
* Google Sheets (on Google Drive, not locally)
* Google Apps Script (built into Sheets)

---

## 📬 Contact

Questions, suggestions or want to collaborate? Open an issue or connect directly.
