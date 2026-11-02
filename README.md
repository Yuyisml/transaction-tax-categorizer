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
- **Data handling:** Pandas (read CSV into a DataFrame, clean, group and sum)
- **Matching rules:** keyword / regex matching
- **Output formatting:** tabulate or Pandas
- **Output files:** CSV / Excel

## System Diagram

![System Diagram](docs/system-diagram.png)

## Eisenhower Matrix

[docs/eisenhower-matrix.pdf](docs/eisenhower-matrix.pdf)

## Repository Structure

```
transaction-tax-categorizer/
├── README.md
├── src/      # Python source code
├── tests/    # tests
├── data/     # sample/testing CSV data
└── docs/     # system diagram and Eisenhower Matrix
```
