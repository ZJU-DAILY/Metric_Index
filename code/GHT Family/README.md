## GHT
Usage: `[dataFile]  [queryFile]  [costFile]`
Example: `synthetic.txt synthetic_query_id.txt GHT-synthetic-cost.txt`
- dataFile: the path of source data file
- queryFile: the path of input query data file
- costFile: the path to store the running cost

## GNAT
Usage: `[dataFile]  [queryFile]  [costFile]  [height]`
Example: `synthetic.txt synthetic_query_id.txt GNAT-synthetic-cost.txt 9`
- dataFile: the path of source data file
- queryFile: the path of input query data file
- costFile: the path to store the running cost
- height: the height of the tree (we limit the tree-height for fair comparison, which is not necessary for normal use.)

## EGNAT
Usage: `[dataFile]  [queryFile]  [costFile]  [blockSize]`
Example:` LA.txt LA_query.txt EGNAT-LA-cost.txt 4096`
- dataFile: the path of source data file
- queryFile: the path of input query data file
- costFile: the path to store the running cost
- blockSize: the size of block to store the EGNAT node and the unit of size is KB