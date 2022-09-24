[Architecture]

1. Minumun Cluster Size
 - Druid: 1 Master 


2. Data Tier
 - Understood each tier has a separte configuration to serve data with use-cases. How many tiers typically used in the field (2, 3?)

3. Deep Storage
 - In field, when user says 'we don't use Deep Storage', it means using only 'LOCAL DEEP STORAGE' without S3 or HDFS extension?
 - If so, what happens when data excceeds the diskspace?


azure-instances.tf
gcp-instances.tf

12 vcpu: license part
 - 2vcpu imply manager
 - 2vcpu master + zk 
 - 2vcpu data
 - 2vcpu query
 - 1 rds mysql metadata Storage
 - s3

