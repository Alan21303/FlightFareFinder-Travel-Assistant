# ✈️ Flight Fare Finder Bot using UiPath

This project is a Robotic Process Automation (RPA) bot developed using **UiPath Studio**. It automates the process of searching and comparing flight fares from [MakeMyTrip](https://www.makemytrip.com), extracts the required data, stores it in an Excel file, and sends it to the user via email — saving both time and effort.

---

## ✍️ Author

- **Alan03** - [Alan21303](https://github.com/Alan21303)

---

## 📌 Features

- ✅ Accepts source, destination, travel date, and recipient email as inputs
- 🌐 Launches MakeMyTrip and performs automated search
- 📊 Extracts airline name, departure/arrival times, and fare
- 📝 Stores the data in a formatted Excel file
- 📧 Sends the result file to the user using SMTP

---

## 🛠️ Tools & Technologies

| Tool / Technology    | Purpose                                       |
| -------------------- | --------------------------------------------- |
| UiPath Studio        | RPA workflow development                      |
| MakeMyTrip.com       | Data source for flight fares                  |
| Data Scraping Wizard | To extract structured flight data             |
| Excel Activities     | For writing and formatting data in Excel      |
| SMTP Mail Activity   | To send automated emails with attachments     |
| Input Dialog Boxes   | To accept user inputs dynamically             |
| Try-Catch & Delays   | For error handling and timing synchronization |

---

## 🧩 Challenges Faced

| Problem                   | Solution Implemented                                     |
| ------------------------- | -------------------------------------------------------- |
| Dynamic Web Elements      | Used stable selectors with Anchor Base and UI Explorer   |
| Page Load Timing          | Added `Element Exists` checks and appropriate delays     |
| Incomplete Data Scraping  | Adjusted scraping regions and validated DataTable output |
| SMTP Configuration Issues | Used port 587 with TLS and correct credentials           |

---

## 🌍 Real-World Use Cases

- Used by travel agents for quick fare analysis
- Corporate travel planners can automate cost comparisons
- Frequent travelers can schedule periodic fare checks

---

## 🔮 Future Enhancements

- Expand to multiple travel websites (Goibibo, Expedia)
- Add filters (non-stop, preferred airline, price range)
- Integrate hotel/cab data scraping
- Build a dashboard for trend monitoring
- Add chatbot interface for input and output

---
