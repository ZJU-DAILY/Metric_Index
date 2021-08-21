## CPT
Usage:` [dataFile] [pname] [indexFile] [costFile] [queryFile] [blockSize] [pivotNumber]`
Example: `synthetic.txt pivot_id_synthetic.txt CPT_synthetic_index CPT_synthetic_cost.txt synthetic_query.txt 40960 5`
- dataFile: the path of source data file
- pname: the path of pivot file
- indexFile: the path to store the generated index file
- costFile: the path to store the running cost
- queryFile: the path of input query data file
- blockSize: the size of block which store the M-tree node and the unit of size is KB
- pivotNumber: the number of pivots