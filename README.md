# Analysis of FY26 Discretionary Funds data set — 04/2026

This repository contains data, analytic code, and findings that support portions of the article, “[Why is the City Using Discretionary Funds to Foster Support for the Israeli Army?](https://docs.google.com/document/d/1xXB_RtWTBaHzg9gpdQsZC84ZQzgMnTKxamxeO6SCz9I/edit?),” published April 17, 2026. Please read that article, which contains important context and details, before proceeding.

## Data

This analysis uses one spreadsheet of all the available discretionary funds set aside by the New York City Council for Fiscal Year 2026.

The spreadsheets come from the following sources:

- Name of source:
  - `Funded Disclosure FY2026.xlsx`: Raw data of all the discretionary funding set aside by the City Council for FY2026.

Each of the spreadsheets contain, among others, the following columns relevant to the analysis:

- `Legal Name` — The name of the nonprofit to which discretionary funds are available. 
- `Amount` — The amount of funds available to any given nonprofit.
- `Purpose of Funds` — The official purpose of the funding.

## Methodology

The notebook [`FY26-notebook.ipynb`](notebooks/FY26-notebook.ipynb) performs the following analyses:

##### Part 1: Find nonprofits that focus on supporting Zionism and the Israeli army

- First, I combed through the list of nonprofits receiving discretionary funds from the city. I noticed a number with "Israel" in their name, and began researching the focus of these nonprofits. Using information from their websites, I gained an understanding of which nonprofits specifically focus on fostering support for Zionism and the Israeli army.

##### Part 2: Pair down the list

- Next, I paired down the full spreadsheet to only include a list of the specific nonprofits that foster support for Zionism and the Israeli army. 


## Outputs

The notebooks output this spreadsheet which contains a list of specific nonprofits and the amount of City Council funding each received: [`israel_funds.csv`](israel_funds.csv).

## Running the analysis yourself

You can run the analysis yourself. To do so, you'll need the following installed on your computer:

- Python 3
- The Python libraries specified in [`requirements.txt`](requirements.txt)

## Licensing

All code in this repository is available under the [MIT License](https://opensource.org/licenses/MIT). The data file in the output/ directory is available under the [Creative Commons Attribution 4.0 International](https://creativecommons.org/licenses/by/4.0/) (CC BY 4.0) license. All files in the data/ directory are released into the public domain.

## Feedback / Questions?

Contact Sohini Desai at sohini.desai74@journalism.cuny.edu.
