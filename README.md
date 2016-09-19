# MRPT - Fast approximate nearest neighbor search with random projection
Efficient index structures for fast approximate nearest neighbor queries are required in many applications such as recommendation systems. In high-dimensional spaces, many conventional methods suffer from excessive usage of memory and slow response times. We propose a method where multiple random projection trees are combined by a novel voting scheme. The key idea is to exploit the redundancy in a large number of candidate sets obtained by independently generated random projections in order to reduce the number of expensive exact distance evaluations. The method is straightforward to implement using sparse projections which leads to a reduced memory footprint and fast index construction. Furthermore, it enables grouping of the required computations into big matrix multiplications, which leads to additional savings due to cache effects and low-level parallelization. We demonstrate by extensive experiments on a wide variety of data sets that the method is faster than existing partitioning tree or hashing based approaches, making it the fastest available technique on high accuracy levels.

## More information
See our paper: https://arxiv.org/pdf/1509.06957.pdf
Comparisons to alternative methods including FLANN, FALCONN and KGraph: https://github.com/ejaasaari/mrpt-comparison