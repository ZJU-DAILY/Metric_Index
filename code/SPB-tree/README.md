## SPB-Tree
Usage: `[dataFile] [pname] [indexFile] [costFile] [maxDistance] [pivotNumber] [blockSize] [queryFile]`
Example:` LA.txt pivot_all_LA.txt spb-index-file spb-cost.txt 25000 5 4096 LA_query.txt`
- dataFile: the path of source data file
- pname: the path of pivot file
- indexFile: the path to store the generated index file
- costFile: the path to store the running cost
- maxDistance: the max distance between objects in source data
- pivotNumber: the number of pivots
- blockSize: the size of block that stores the node of B+-Tree and the unit of size is KB
- queryFile: the path of input query data file