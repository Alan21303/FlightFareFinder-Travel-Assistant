# FlightFareFinder - Travel Assistant

<p align="center">
  <img src="https://img.shields.io/badge/UiPath-Studio-blueviolet?style=for-the-badge&logo=uipath" />
  <img src="https://img.shields.io/badge/Microsoft-Excel-1D6F42?style=for-the-badge&logo=microsoft-excel" />
</p>

An intelligent RPA bot designed to automate the tedious process of searching for flight fares. This assistant navigates [MakeMyTrip.com](https://www.makemytrip.com), scrapes flight data based on user input, compiles it into a structured Excel report, and delivers it directly to your inbox.

---

### About The Project

Manually checking websites for the best flight prices is time-consuming and repetitive. This project solves that problem by deploying a UiPath robot to act as a personal travel assistant. It provides a hands-free way to gather and compare flight information, saving you valuable time and effort.

The core of this automation lies in its ability to:

- Interact with a user to get travel requirements.
- Perform robust web automation on a dynamic website.
- Extract structured data from complex web layouts.
- Generate a clean, usable report.
- Communicate the results via email.

---

### Key Features

- **Dynamic User Input:** Prompts for travel details like source, destination, and date.
- **Automated Web Navigation:** Launches MakeMyTrip.com and performs the search automatically.
- **Intelligent Data Scraping:** Extracts crucial flight details including airline, timings, and price.
- **Structured Reporting:** Organizes all scraped data into a clean, easy-to-read Excel file.
- **Secure Email Notifications:** Automatically sends the Excel report using securely stored SMTP credentials.

---

### How It Works

1.  **Collects Input:** The robot starts by asking the user for the source, destination, travel date, and recipient email.
2.  **Launches Browser:** It opens MakeMyTrip.com in a web browser.
3.  **Performs Search:** The bot enters the user-provided details into the search form and initiates the search.
4.  **Scrapes Data:** Once the results page loads, it systematically extracts the flight data into a structured table.
5.  **Generates Report:** The scraped data is written to an Excel file, which is named dynamically based on the search query.
6.  **Sends Email:** The robot retrieves securely stored sender credentials, composes an email, attaches the report, and sends it to the user.

---

### Built With

| Tool / Technology          | Purpose                                                |
| -------------------------- | ------------------------------------------------------ |
| UiPath Studio              | RPA workflow development                               |
| MakeMyTrip.com             | Data source for flight fares                           |
| Data Scraping              | To extract structured flight data from the web.        |
| Excel Activities           | For writing and organizing data in `.xlsx` files.      |
| SMTP Mail Activity         | To send automated emails with the report.              |
| Windows Credential Manager | For securely storing and retrieving email credentials. |

---

### Getting Started

To get a local copy up and running, follow these simple steps.

**Prerequisites**

- **UiPath Studio** (Community or Enterprise)
- **Microsoft Excel**

**Installation & Configuration**

1.  **Clone the repository:**
    ```sh
    git clone https://github.com/Alan21303/FlightFareFinder-Travel-Assistant.git
    ```
2.  **Open the project** in UiPath Studio by opening the `project.json` file.

3.  **Set up SMTP Credentials:**
    This bot uses the Windows Credential Manager to securely handle the sender's email credentials.

    - Open **Control Panel** -> **Credential Manager** -> **Windows Credentials**.
    - Click **"Add a generic credential"**.
    - Enter the following details:
      - **Internet or network address:** `FlightFareFinder_SMTP_Credentials`
      - **User name:** Your sender's Gmail address (e.g., `your.email@gmail.com`)
      - **Password:** Your 16-character Google App Password.

4.  **Run the Robot:**
    - Open `Main.xaml` in UiPath Studio.
    - Click the **"Run"** button.
    - Follow the prompts to enter your travel details.

---

### Author

- **Alan03** - Alan21303

---

### Roadmap

- [ ] Expand to multiple travel websites (e.g., Expedia, Goibibo).
- [ ] Add support for advanced filters (non-stop, preferred airlines).
- [ ] Integrate hotel and cab booking data.
- [ ] Develop a user interface or chatbot for a more interactive experience.

- Expand to multiple travel websites (Goibibo, Expedia)
- Add filters (non-stop, preferred airline, price range)
- Integrate hotel/cab data scraping
- Build a dashboard for trend monitoring
- Add chatbot interface for input and output

---
