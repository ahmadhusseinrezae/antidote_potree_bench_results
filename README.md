# antidote_potree_bench_results

AntidoteDB was deployed in a riak ring with varying numbers of vnodes for the sake of this performance evaluation. It was deployed on a system with 20 CPU cores and 80 GB of RAM. During the benchmark, the load generator was deployed and running on the same machine as AntidoteDB. Since riak ring's vnodes were on the same machine, network latency was insignificant.
The load generator issued three distinct types of operations: put, get, and get-range. In AntidoteDB, put was an update operation. get-range is a range query operation, whereas get was a read operation. Depending on the experiment, a varying number of concurrent workers generated the load.
