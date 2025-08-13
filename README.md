# Competition-analysis
Keyword Scraping and Visualization
📌 Overview
This project scrapes keywords from a given website, retrieves keyword metrics such as Search Volume, CPC (Cost Per Click), and Keyword Difficulty, and visualizes the results using a pie chart.
The stopwords list is restricted to punctuation marks only to avoid removing meaningful words during processing.

🚀 Features
Web scraping of keywords from target URLs.

Removes only punctuation marks, preserving all words.

Fetches keyword metrics (Volume, CPC, Difficulty).

Saves keyword data to an Excel file.

Generates a pie chart visualization for selected metrics.

Saves the visualization as a PNG image.

📂 Project Structure
bash
Copy
Edit
├── main.py                 # Main script for scraping and visualization
├── keywords.xlsx           # Output Excel file with keyword data
├── pie_chart.png           # Generated pie chart visualization
├── README.md               # Project documentation
🛠 Installation
Make sure you have Python 3.x installed. Install required dependencies with:

bash
Copy
Edit
pip install requests beautifulsoup4 pandas matplotlib nltk pytrends openpyxl
⚙️ Usage
Run the script:

bash
Copy
Edit
python main.py
Enter the URL of the website you want to scrape.

Choose the metric for the pie chart (Volume, CPC, or Difficulty).

The program will:

Scrape keywords.

Save data to keywords.xlsx.

Generate a pie chart PNG (pie_chart.png).

📊 Visualization Example
Example pie chart output:

📜 Notes
Stopwords list contains only punctuation marks:

python
Copy
Edit
stopwords = [',', '.', '!', '(', ')', '[', ']', '{', '}', '"', "'"]
No words are removed from the keywords to ensure complete data extraction.

Ensure you have a stable internet connection for web scraping and Google Trends API requests.
