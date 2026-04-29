# Federal Reserve Speech Complexity Dashboard
A Power BI dashboard created as a fun visualization project based on one of my dissertation research.

# Overview
This dashboard is a lightweight, exploratory visualization project built in Power BI. It’s not meant to be a rigorous academic output, instead, it’s something I thought would be fun and visually interesting to create using a subset of the data from my doctoral research on Federal Reserve communication.

The goal is simply to showcase:

- how linguistic complexity in Fed speeches evolves over time
- how different roles and districts compare
- how topics differ in readability and cognitive strain
- how Power BI can be used to tell a clean, intuitive data story

This project focuses on visual storytelling, not formal econometric analysis. I will also limit to just 3 measures of complexity due to the paper space constraint.

# Dashboard Pages
Page 1. Complexity Over Time:
Long‑run trends in abstractness, readability, and cognitive strain.

Page 2. Roles & Speakers' Backgrounds:
Differences in speech complexity across roles and some FOMC Members' characteristics.

Page 3. Financial Variables and Macroeconomic Indicators:
Correlations between complexity measures versus financial variables and macroeconomic figures.

Page 4. Additional Visuals
A filled map of Federal Reserve districts and topics' proportion over time.

# Data Sources
The dataset used here is derived from my doctoral thesis project, where I constructed a corpus of FOMC speeches and computed linguistic complexity metrics using Python.

Because the underlying codebase is part of a much larger research pipeline---involving multiple datasets, heavy preprocessing, and ongoing cleanup---the full code is not included in this repository.

The data files provided here are the cleaned, analysis‑ready outputs used directly in Power BI.

If you’re curious about the methodology, feel free to reach out. However, here I would like to cite the datasources:
## FOMC Speeches (1986–2025)
- Core dataset extends Campiglio, E., Deyris, J., Romelli, D., & Scalisi, G. (2025), which covers FOMC member speeches from Jan 1986–Dec 2023.
- Updated through web scraping of: (1) Federal Reserve Board website, (2) All 12 Federal Reserve Bank websites
- Additional archival material for missing years (e.g., William Poole, 1998–2008) obtained from the FRASER digital archive.
- Only publicly available speeches are included.
- Video transcripts (e.g., YouTube‑based materials) are excluded to maintain consistency with Campiglio’s original dataset

## Speaker Background Information
Biographical and career information for FOMC members compiled from:
- Federal Reserve Board and regional bank official biographies
- Conti‑Brown & Nygaard Federal Reserve Bank Boards of Directors Biographical Database
- Background dataset from Riboni, A., & Ruge‑Murcia, F. (2025)
Variables include: gender, race, degree major, terminal degree, pre‑Fed career, institutional role, saltwater/freshwater classification, age, and tenure

## Daily Financial Market Data
- Daily equity and Treasury market variables obtained via the Yahoo Finance API.
- Used to construct volatility, return, and volume‑based measures aligned with speech dates

## Intraday Financial Market Data (2010–2023)
- High‑frequency (15‑minute) price and volume data sourced from the Bloomberg Terminal.
- Intraday sample restricted to regular U.S. trading hours (09:00–16:30 ET).
- Speech timestamps sourced from the FRASER FOMC Speak Archive (2010–2023)

## Macroeconomic Data
Public macroeconomic indicators retrieved from:
- FRED (Federal Reserve Economic Data)
- ALFRED (archival vintages)
- Additional real‑time macroeconomic conditions taken from the Greenbook/Tealbook (where publicly accessible)


# References (for Data Sources)
Campiglio, E., Deyris, J., Romelli, D., & Scalisi, G. (2025). Warning words in a warming world: Central bank communication and climate change. European Economic Review, 178, 105101. https://doi.org/10.1016/j.euroecorev.2025.105101

Riboni, A., & Ruge‑Murcia, F. (2025). Membership Turnover and Policy Disagreement at the FOMC. HAL Working Paper hal‑05229751. https://ideas.repec.org/p/hal/wpaper/hal-05229751.html
