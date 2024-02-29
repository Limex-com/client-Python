# limeX: Datahub integration using Python

### Intro
limex is a package for interaction with alternative data, trading API of different exchanges and brokers. Package provides access to market data for storage, analysis, algorithmic trading, strategy backtesting. Also this is data downloader from different data sources starting from close price to order book and tradelog.

### Installation

```r
pip install limex
```
### Getting Started

It is possible to import data from a variety of sources with one rusquant
function: `get_symbols()` and datasource (as example gigapack). For example:

``` r
from limex.services import lx
df0 = lx.get_symbols(symbols=['AAPL', 'AMZN'], fake=True, type_data='candles')
df1 = lx.get_symbols(symbols=['AAPL', 'AMZN'], fake=False, type_data='candles')
df2 = lx.get_symbols(symbols=['AAPL', 'AMZN'], fake=True, type_data='tech')
df3 = lx.get_symbols(symbols=['AAPL', 'AMZN'], fake=False, type_data='tech')
```
