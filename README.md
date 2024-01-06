# financial-statement
\f0\fs24 \cf0 # financial_statement\
\
[![License](https://img.shields.io/badge/license-MIT-blue.svg)](https://opensource.org/licenses/MIT)\
\
# Overview\
\
financial_statement is a Python package that allows you to read the financial statements of listed companies.\
\
## Installation\
\
```bash\
pip install financial_statement
```
}
## Usage
```python
import financial_statement as fs
# get annual income statement
ticket = "AAPL"
year = "2023" # it is string
income_statement = income_statement(ticket,year)

# get balance sheet
balance_sheet = balance_sheet(ticket,year)

# get cash flow statement
cash_flow_statement = cash_flow_statement(ticket,year)

# get dividend from company
dividend = get_dividend(ticket)
# if you want get annual received dividend
annual_dividend = get_dividend(ticket,YTM=True)

# get shareholder list
shareholder = shareholder(ticket)
```

## Source

The library extracts data from discounting cash flows and Yahoo Finance. Developers are not tasked with accumulating the data, and the library automatically goes offline in the case of an interest conflict.

