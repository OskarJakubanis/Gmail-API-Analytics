## **Google Apps Script (JavaScript)**

* **`SpreadsheetApp.getActiveSpreadsheet()`** – Returns the currently active Google Sheet file.
* **`getSheetByName("RAW_DATA")`** – Returns the sheet named `"RAW_DATA"` in the spreadsheet.
* **`GmailApp.getInboxThreads(start, batchSize)`** – Fetches a batch of threads from the Gmail inbox starting at index `start`.
* **`thread.getMessages()`** – Returns all messages in a Gmail thread.
* **`msg.getFrom()`** – Gets the full sender string (name + email) from a Gmail message.
* **`string.match(/<(.+)>/)`** – Uses regex to extract only the email address from the sender string.
* **`sheet.getRange(startRow, 1, rows.length, 1).setValues(rows)`** – Writes a 2D array `rows` to the sheet starting from `startRow` in the first column.
* **`PropertiesService.getScriptProperties()`** – Accesses script-wide properties for storing small persistent data (like last processed thread index).
* **`props.setProperty(key, value)` / `props.getProperty(key)`** – Stores and retrieves persistent key-value pairs.
* **`ScriptApp.newTrigger("importEmailsBatch").timeBased().after(1000).create()`** – Creates a time-based trigger to automatically run the function again after 1 second.
* **`props.deleteProperty("lastStart")`** – Deletes the stored property once all threads are processed.
