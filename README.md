# NBA GOAT Machine

This project is designed to create an automated, data-driven system to rank the greatest NBA players of all time based on advanced metrics, conceptual adjustments, and contextual awards.

## Project Folder Structure
```
NBA-GOAT-Machine/
│
├── data/
│   ├── raw/            # Unprocessed scraped data
│   └── processed/      # Cleaned and transformed data
│
├── notebooks/          # Jupyter notebooks for exploration and analysis
│
├── scripts/            # Python scripts for data scraping and processing
│
├── outputs/            # Final outputs like visualizations and reports
│
├── .gitignore          # Specifies files and directories to be ignored by Git
└── README.md           # Project overview and setup instructions
```

## Setup Instructions
1. **Clone the Repository:**  
   ```bash
   git clone https://github.com/astefanidis1/NBA-GOAT-Machine.git
   cd NBA-GOAT-Machine
   ```

2. **Create and Activate Virtual Environment:**  
   ```bash
   python -m venv venv
   .\venv\Scripts\activate  # Windows
   ```

3. **Install Required Packages:**  
   ```bash
   pip install requests beautifulsoup4 pandas openpyxl gspread oauth2client
   ```

4. **Setup .gitignore:**  
   ```bash
   echo venv/ > .gitignore
   echo __pycache__/ >> .gitignore
   echo *.pyc >> .gitignore
   ```

5. **Push Initial Setup to GitHub:**  
   ```bash
   git add .
   git commit -m "Initial project setup with virtual environment and folders"
   git push origin main
   ```

## Key Tasks
- **Data Scraping & Automation:**
  - Scrape advanced stats and awards from Basketball Reference.
  - Automate updates to an Excel or Google Sheet file.

- **Metrics & Weighting:**
  - Apply weightings to key stats: BPM, OBPM, DBPM, TS%, AST/TO, WS/48, VORP, and PER.
  - Fine-tune the impact of each metric on player rankings.

- **Award Integration:**
  - Incorporate awards like MVPs, Finals MVPs, DPOYs, All-NBA, and All-Defensive Team selections.
  - Apply minor boosts for All-Star selections and Rookie of the Year.

- **Conceptual Adjustments:**
  - Add longevity, consistency, peak vs. career splits, playoff multipliers, and era adjustments.
  - Include a tiered bonus for game-changing players (e.g., Curry, Jordan, Russell).

- **Final Rankings & Analysis:**
  - Generate final rankings, normalize to a 2K-style rating out of 99, and analyze outliers.
  - Adjust as necessary based on anomalies in the results.

## Files
- **NBA_GOAT_Template.xlsx**  
  Template spreadsheet where scraped data and metrics will be populated. Contains pre-set columns for stats, awards, and final ratings.

- **NBA_GOAT_Full_Plan.docx**  
  Detailed step-by-step plan outlining metrics, conceptual adjustments, award weightings, and data scraping processes.

