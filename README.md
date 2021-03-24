
## Use Case Description
This use case is intended to simulate the workload of an inventory management database. The schema contains the following tables:

- Product category
- Product data
- Orders
- Suppliers
- Customers
- Reviews

This is a read-heavy workload, with reads accounting for about 96% of the transactions and writes accounting for 4%. This use case is intended to be tested on AWS, with a Cassandra database cluster. Each database instance is backed by an f1.2xl instance running the rENIAC Row Cache product.

This test creates about 90GB of data on a database node. When queries are accelerated by rENIAC Row Cache, the throughput goes up to almost 7x the throughput vs baseline (i.e. when rENIAC Row Cache is not enabled). The latency also goes down significantly - by about 7x for mean to about 15x for 95th percentile. 

Click **[here](https://www.reniac.com/wp-content/uploads/2021/03/inv_mgmt.tar "Download the tar file")** to download the required files.

**Contact

**rENIAC Support - for technical help or discounts on pricing

support@reniac.com


