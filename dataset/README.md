## Input Source Data
Take LA dataset as an example below.
```
2 1073727 2
6032.63 5585.62
6033.83 5585.80
6026.04 5580.84
......
```
The first line of source data contains three numbers to represent the data dimension, the number of objects, and the distance function, respectively. Each line that starts from the second line represents a detailed record/object. Every dimension data is separated by the blank.

Note That, we utilize numbers to represent distance functions, as we adopt the Lp-norm here. The number denots the p value.

| Number  |  Measurement |
| :------------: | :------------: |
|1  | Manhattan Distance  |
| 2 |  Euclidean distance |
| 5 |  Minkowski Distance |
|   other| Chebyshev Distance |

<font color=#dc3545>If you want to run codes on other datasets. Please make sure that the data format is the same. In addition, other data types and distance metrics can be also used by modifying the object class.</font>

## Input Query Data
For the main-memory indexes, we use the data id to perform the queires. However, for the disk-based indexes, we use the detailed data records to do the queries. Take LA Query Data as an example. We have two types of query data file `LA_query.txt` and `LA_query_id.txt`.
- In `LA_query.txt`, each line represents a query object/record.
- In `LA_query_id.txt`, each line represents the id of a query object in the source data file.

## Input Pivot Data
Similar as Query Data, the Pivot Data can also use both id and detailed records. Take LA Pivot Data as an example. We have two different types of pivot file `pivot_all_LA.txt` and `pivot_all_LA_id.txt`.
- In `pivot_all_LA.txt`, each line represents a pivot, i.e., a detailed object information.
- In `pivot_all_LA_id.txt`, each line represents the id of pivot in source data file.

Note that, the pivots are used for pivot-based methods and hybrid methods, which are selected by pivot selection methods. Here, we use HFI to select pivots. However, various pivot selection methods exit. Latter, we will also release all the codes of various pivot selection methods.

## Output Cost Data
For the index construction, we provide four preformace metrics: `index build time`, `the number of distance computations`, `the size of index`, `IO times`. For query, we give the following performance metrics:
- query time: the average query time for each query
- distance computed: the average number of distances computed for each query
- IO times: the average number of page access for each query (only for disk-based index)
- radius: the average k-the nearest neighbour distance for each query (only for KNN Query)
- obj: the average number of result objects for each query (only for Range Query)
