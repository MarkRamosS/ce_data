# Cache estimator data.
This project contains the raw data output by champsim.

This data is collected by running Champsim on the traces of 3rd Data Prefetching Championship (DPC-3) (https://dpc3.compas.cs.stonybrook.edu/champsim-traces/speccpu/) with the addition of rdlru, an lru that's only enabled on the files ending in '_2048.out' and prints the reuse distance histogram every 2 million iterations. The rest of the files have the cache accesses and misses every 2milion iterations. All files are ran for 1.5 billion iterations with 50 million warmup instructions.

The reuse distances and cache miss ratios we'll use for training are retrieved from the raw data via the clear_data.ipynb file.

This project acts as a database to the main project: https://github.com/MarkRamosS/ce_data/edit/main/README.md 
