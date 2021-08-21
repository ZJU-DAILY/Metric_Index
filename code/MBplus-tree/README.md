## MB<sup>+</sup>-tree
Usage: `[dataFile] [indexFile] [costFile] [blockSize] [queryFile] [maxDistance]`
Example: `synthetic.txt MBTree-synthetic-index MBTree-cost.txt 4096 synthetic_query.txt 10000`
- dataFile: the path of source data file
- indexFile: the path to store the generated index file
- costFile: the path to store the running cost
- blockSize: the size of block which store the node of B+-Tree and the unit of size is KB
- queryFile: the path of input query data file
- maxDistance: the max distance between objects in the source data