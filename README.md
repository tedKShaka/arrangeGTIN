Arrange GTIN
==============
Provided with Average Sales sheet from quickbooks, this script will pair GTINs with SKUs, sort them by GTIN ascending, and produce new .xlsx with SKU and Quantity sold.

 
 Usage
 --------------
1. Requires [environment](https://docs.python.org/3/tutorial/venv.html) running for Python 3.7 and up, then ```$ pip install -r requirements.txt ```

2. Run python script - provide script(GTINArrange.py) and argument(target excel file) on command line:
```$ python [script] [argument]```

Example: 
```
$ python GTINArrange.py ./testQtys.xlsx

            GTIN      SKU  Quantity
0   843105125366  CLS022X       6.0
0   843105125373  CLS023X       7.0
0   843105125380  CLS024X       5.0
0   843105125397  CLS025X      10.5
0   843105125403   CLS02L       0.0
..           ...      ...       ...
0   843105119259  VNS017X       0.0
0   843105119266   VNS01L     130.0
0   843105119273   VNS01M     121.0
0   843105119280   VNS01S      28.0
0   843105119297  VNS01XL     119.0

[1814 rows x 3 columns]
            GTIN      SKU  Quantity
0   843105114711  MHS012T     124.5
0   843105114728  MHS012X     357.0
0   843105114735  MHS013T     135.0
0   843105114742  MHS013X     266.0
0   843105114759  MHS014T      24.0
..           ...      ...       ...
0   843105147979  FJP253X       3.0
0   843105148006   FJP25L      12.0
0   843105148013   FJP25M      12.0
0   843105148020   FJP25S       6.0
0   843105148037  FJP25XL       6.0

Sorting finished. Saving sheet in folder as sortedQtys.xlsx
```
Resulting file will be sorted, and only has SKU and Quantity column.
