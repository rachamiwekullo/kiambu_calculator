
## Kiambu Dairy Co-op Payment Calculator

A lightweight Python CLI tool built for dairy co-operatives to calculate daily payout amounts for farmers based on the quantity of milk supplied (in litres) and the current rate per litre.

## Features

- Dynamic Price Configuration: Automatically checks for a price.txt configuration file to set the per-litre price.
- Default Fallback: Defaults to KES 55.00/litre if price.txt is missing.
- Input Validation: Ensures farmer names are provided and that milk volume entries are valid numbers greater than zero.
- Formatted Currency Output: Prints clear receipt summaries formatted with thousands separators and 2 decimal precision.

# Project Structure

- kiambu_cal.py    # Main application script
- price.txt        # Optional configuration file specifying current price per litre
- README.md        # Project documentation


## Installation & Setup

Prerequisites

Python 3.7+ installed on your system.

## Steps

Clone or download the script files into your target directory.

Open your terminal or virtual environment (.venv):

cd "D:\AI DATA ANALYST\WEEK 2"


## Usage

Run the calculator script via terminal:

```bash
python kiambu_cal.py
```


## Example Interactive Output

```text
Kiambu Dairy Co-op Payment Calculator
--------------------------------------
Current buying price: KES 55.00 per litre

Farmer name: Ann
Litres supplied today: 80

Farmer : ann
Litres : 80.0
Price  : KES 55.00/litre
Total  : KES 4,400.00
```


## Configuration (price.txt)

- To update the per-litre buying rate without modifying the code, create or edit price.txt in the same folder as ``` kiambu_cal.py:```
- Create price.txt.
- Enter the numeric price per litre (e.g., 60.0).
- Save the file.
When you execute ```python kiambu_cal.py```, the system will automatically read and apply the updated rate.
