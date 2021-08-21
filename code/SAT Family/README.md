## SAT
Usage:` [dataFile] [indexFile] [costFile] [queryFile] [height]`
Example: `synthetic.txt synthetic_index.txt synthetic_cost.txt synthetic_query.txt 9`
- dataFile: the path of source data file
- indexFile: the path to store the generated index file
- costFile: the path to store the running cost
- queryFile: the path of input query data file
- height: the height of the tree (we limit the tree-height for fair comparison, which is not necessary for normal use.)

## DSACLT
Usage:` [dataFile] [indexFile] [costFile] [queryFile] [maxArity] [blockSize]`
Example: `synthetic.txt synthetic_index.txt synthetic_cost.txt synthetic_query.txt 5 4096`
- dataFile: the path of source data file
- indexFile: the path to store the generated index file
- costFile: the path to store the running cost
- queryFile: the path of input query data file
- maxArity: the max arity of DSACLT
- blockSize: the size of block which store the node of DSACLT and the unit of size is KB