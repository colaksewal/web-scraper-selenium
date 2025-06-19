# Web Scraper with Selenium & Regex

This project is a comprehensive web scraping tool built with **Python**, utilizing **Selenium**, **BeautifulSoup**, and **Regular Expressions** to automatically extract **email addresses**, **URLs**, and **phone numbers** from any web page. It also features GUI support via **tkinter**, data analysis via **pandas**, and visualization using **matplotlib**.

---

## 🚀 Features

- 🌐 Navigate to a web page automatically using Selenium
- 🧠 Extract full page content and parse it with BeautifulSoup
- 📧 Detect email addresses using regex
- 🔗 Detect URLs from the content
- 📞 Identify phone numbers using the `phonenumbers` library
- 🧮 Analyze and tabulate the results using pandas
- 📊 Visualize findings with matplotlib
- 🪟 GUI-based file selection with tkinter
- ⚡ Multi-threaded execution for performance using ThreadPoolExecutor

---

## 🧰 Technologies Used

- Python 3.x
- Selenium (web automation)
- BeautifulSoup (HTML parsing)
- Regex (`re` module)
- phonenumbers
- pandas
- matplotlib
- tkinter (GUI)
- concurrent.futures (for multithreading)
- webdriver-manager (for automatic ChromeDriver handling)

---

## 📦 Installation

Install required Python packages:

```bash
pip install selenium beautifulsoup4 pandas matplotlib phonenumbers webdriver-manager
```

> Make sure you have Google Chrome installed. `webdriver-manager` will auto-download the correct driver.

---

## ⚙️ How to Run

1. Clone this repository or download the `advancedWebDataExtractor.ipynb` file.
2. Install the dependencies listed above.
3. Launch the notebook:

```bash
jupyter notebook advancedWebDataExtractor.ipynb
```

4. The script will:
   - Launch Chrome browser and navigate to a specified URL
   - Scrape the entire HTML source of the page
   - Use regular expressions and `phonenumbers` to extract:
     - Emails → `[\w.+-]+@[\w-]+\.[\w.-]+`
     - URLs → `https?://(?:[-\w.]|(?:%[\da-fA-F]{2}))+`
     - Phone numbers → via `phonenumbers.PhoneNumberMatcher`

5. Results are:
   - Displayed in lists
   - Exported as a DataFrame using `pandas`
   - Visualized with `matplotlib`


