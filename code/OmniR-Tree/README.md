## OmniR-Tree
Usage: `[dataFile] [pname] [indexFile] [costFile] [queryFile] [pivotNumber]`
Example: `synthetic.txt pivot_all_synthetic.txt R-synthetic-index R-synthetic-cost.txt synthetic_query.txt 5`
- dataFile: the path of source data file
- pname: the path of pivot file
- indexFile: the path to store the generated index file
- costFile: the path to store the running cost
- queryFile: the path of input query data file
- pivotNumber: the number of pivots

The implementation of OmniR-tree by the authors themselves can be found in [OmniTree project](http://www.cs.cmu.edu/~christos/SRC/OmniUsrKit.tar.gz "OmniTree project").