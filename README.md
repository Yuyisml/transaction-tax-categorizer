# Transaction Tax Categorizer

## Project Goal

A lightweight Python tool that ingests raw bank transaction CSVs, automatically categorizes expenses into tax deduction buckets using custom matching rules, and exports a clean summary report.

## MVP Scope

The MVP covers the "Do" quadrant of the Eisenhower Matrix:

- Define data parsing (Pandas)
- Map out tax categories and rules
- Set up testing data (CSV)

## Future Plans

Planned for V2.0+ (the "Schedule" quadrant):

- Build a categorization engine
- Export a clean and concise output
- Handle edge cases

Handled with libraries/tools ("Delegate"): generating mock data through AI, formatting tables through tabulate or Pandas, and standardizing CSV header mapping across bank formats.

Out of scope ("Delete"): relying on live API banking data, creating an entire GUI, and inputting other tax files (e.g. W2, W9, 1095-A).

## Tech Stack

- **Language:** Python
- **Libraries:** Pandas, RE (regular expressions), OpenPyXL
- **Version control:** Git / GitHub

Possible additions in future versions: Rich, Matplotlib, SQLite, FastAPI, and the Plaid API.

## System Diagram

![System Diagram](docs/Flowchart%20System%20Diagram.drawio.png)

The diagram was made in draw.io; the `.drawio.png` file contains the editable draw.io source and can be opened directly in draw.io.

## Eisenhower Matrix

[Eisenhower Matrix (PDF)](docs/Eisenhower%20Matrix%20Diagram-2.pdf)

## Repository Structure

```
transaction-tax-categorizer/
├── README.md
├── src/      # Python source code
├── tests/    # tests
├── data/     # sample/testing CSV data
└── docs/     # system diagram and Eisenhower Matrix
```
