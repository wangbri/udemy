# Section 1
## AWS Setup

AWS for machine learning service is available in US East (N. Virginia) but base application can be connected to it elsewhere.

Amazon S3 is a storage service to store large datasets such as csv files and EC2 is a remote computer running Windows or Linux that can be used to process/train these datasets.

S3 buckets are used for universal file storage. S3 bucket policies can grant bucket access to a user or a service (such as machinelearning.amazonaws.com).

A bucket contains the following contents:
  - csv file containing all training data
  - csv file containing only training inputs for testing the model
  - store predicted model results into an output folder
