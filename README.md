# Finsight - Equity Research, Simplified 
Team: John Luke Lim Kang & Jermaine  Khor | Orbital 2026 | Apollo 11 | Team 7666
Proposed level of acheievement: Apollo 11

# Motivation behind the project
Investors and students in Singapore face a fragmanted research experience. To screen stocks by fundamental metrics, view price history and assess financial health, a student analyst has to jump between multiple platforms. Most of which are either paywalled, US-centric or poorly suited to SGX-listed equities. This process has too many hoops, which unecessarily complicates investing.

Professional tools like Bloomberg termainals and FactSet are inaccessible to most undergraduates. Free alternatives like Yahoo Finance lack the clean, focused interface that a student analyst actually needs. This fragmentation is a real barrier to making informed decisions during investment

FinSight is built to close that gap, and our goal is a simple unified platform that brings together stock screening, fundamental data, price history, and a quantitative financial health indicator. This allows for users, specifically student analysts to develop rigorous, data-driven approches to equity research without needing access to professional or pay-walled tools. 

# Aim
FinSight is a web application for students to research stocks listed on the Singapore Exchange (SGX) and US markets. Users can search for stocks, view clean price charts, and use a colour-coded Financial Health Score to assess whether a company is financially stable. Logged-in users can also maintain a personal watchlist to track stocks they are interested in.

# Features

- Stock Screener | Users can filter SGX and US-listed stocks by exchange, sector, P/E ratio and market capitalisation. Data is fetched live via the yfinance API. This is the primary entry point for users who want to discover stocks matching specific criteria.
- Stock Detail Page | Each stock has a dedicated page showing its current price, price to earnings ratio, earnings per share (EPS), market cap, dividend yield, and 52-week high and low. Every metric has an explanation, making the platform accessible to beginners. Data will be fetched in real time via yfinance (Yahoo! Finance API)
  
- Personal Watchlist | Authenticated users can save stocks to a personal watchlist, add annotations and remove stocks. Watchlist data is a stored in a database.

- Finacial Health Score | A colour-coded risk indicatior (Low, Medium and High) calculated from three financial ratios: debt-to-equity, current ratio and interest coverage ratio. The score is then computed.

# Extension Features 

- Interactive Price Charts | Hostorical closing prices rendered using Chart.js over 1M, 3M and 1Y windows, where users are given the option to toggle between them.

- Stock search | A search bar that suggests stock tickers and company names, using live data

- Watchlist CSV Export | Logged-in users can download their watchlist as a CSV file for use in Excel and other tools.

# Timeline and Development Plan

| S/N | Tasks | Description | In-Charge | Date |
| --- | --- | --- | --- | --- |
| **1** | Finalise ideas | Design user interface layouts in Canva, sketch application features and core user flows. | Jermaine | 11 May - 15 May |
| | | Draft Liftoff presentation slides, compile the video script, and complete recording. | John | | 
| **2** | Preliminary research | Learn how Flask routing works and set up coding environment. | John <br> Jermaine | 16 May - 23 May |
| | | Test pulling live stock data from the yfinance API | John | |
| **3** | Database Initialization | Create the local SQLite database tables to store user profiles. | Jermaine | 24 May - 28 May |
| | | Code the database setup script to test saving and loading user data. | John | |
| **4** | UI & Code Integration | Connect the live yfinance data to our styled HTML frontend pages. | John <br> Jermaine | 29 May - 31 May |
| | | **Evaluation Milestone 1:** <br> - Ideation <br> - Proof-of-concept: <br> &nbsp;&nbsp;&nbsp;&nbsp; - 1 hardcoded stock successfully pulling live market numbers. <br> &nbsp;&nbsp;&nbsp;&nbsp; - Local database file verifying it can save and load a test user profile. <br> &nbsp;&nbsp;&nbsp;&nbsp; - Clean web page showing our core design layouts and live price data | | **1 June** |
| **5** | Dynamic Stock Search | Build a search bar that lets users look up any SGX or US stock ticker. | Jermaine | 2 June - 5 June |
| | | Add checks so typing a wrong symbol or lowercase letters doesn't crash the app. | Jermaine | |
| **6** | Personal Watchlist | Create a database table so users can save their favorite stocks. | John | 6 June - 12 June |
| | | Code buttons to easily add, view notes on, or delete stocks from the list. | John | |
| **7** | User Authentication | Create secure registration and login pages for user accounts. | Jermaine | 13 June - 21 June |
| | | Use password hashing so user passwords aren't stored in plain text. | Jermaine | |
| **8** | Interactive Charts | Add a visual section for charts on the stock detail page. | Jermaine | 22 June - 28 June |
| | | Connect **Chart.js** to show 1-month, 3-month, and 1-year historical price graphs. | John | |
| | | **Evaluation Milestone 2:** <br> - First Working Prototype <br> - Core Features Operational: <br> &nbsp;&nbsp;&nbsp;&nbsp; - Working stock search bar and user account login sessions. <br> &nbsp;&nbsp;&nbsp;&nbsp; - Personal watchlists that save data permanently to the database. <br> &nbsp;&nbsp;&nbsp;&nbsp; - Interactive price charts displaying stock performance over time. | | **29 June** |
| **9** | Financial Health Engine | Write the math formulas to pull key financial numbers from company reports. | Jermaine | 30 June - 5 July |
| | | Set up thresholds for Debt-to-Equity, Current, and Interest Coverage ratios. | John | |
| **10** | Stock Screener | Build an interactive table page for users to discover new stocks. | Jermaine | 6 July - 10 July |
| | | Allow users to filter the table by sector, exchange, P/E ratio, and market cap. | John | |
| **11** | CSV Export Extension | Write code to turn a user's watchlist into an Excel-friendly format. | Jermaine | 11 July - 17 July |
| | | Add a download button so users can save their watchlist as a `.csv` file. | Jermaine | |
| **12** | System Audits & Polish | Fix any loading lag and clean up database query speeds. | John <br> Jermaine | 18 July - 26 July |
| | | Run final testing to catch and fix any bugs before the official deployment. | John <br> Jermaine | |
| | | **Evaluation Milestone 3:** <br> - Complete Minimum Viable Product (MVP) <br> - Final App Release: <br> &nbsp;&nbsp;&nbsp;&nbsp; - Working automated Financial Health Score (Low/Medium/High risk). <br> &nbsp;&nbsp;&nbsp;&nbsp; - Fully operational stock screener with advanced sorting filters. <br> &nbsp;&nbsp;&nbsp;&nbsp; - Watchlist export-to-CSV utility tool and finalized user interface. | | **27 July** |


  
