# Section 4
## AWS Linear Regression example
*using (ml_linear_examples.ipynb)*

Place training sets in CSV file and then upload to AWS S3. Training data can also be pulled from a SQL database from AWS Redshift.

AWS services > Analytics > Machine Learning: In the dashboard, you can create the datasource, create a ML model, evaluate an existing model that you have, or conduct batch prediction with an existing working model.

- Create the datasource
  - specify the location of your CSV file in the S3 bucket
  - check the schema to see if AWS ML processed the data correctly
  - AWS ML automatically selects the appropriate ML model to train the data
  - optional row identifiers are a pass-through column and identifies each row with a unique key, not used to train the model

While the datasource is being created, you can start building the model as the dependencies should already exist and won't execute until the datasource has been created. The datasource provides visualization (histograms and box plots) and a statistical summary of the data (strength of correlation between attributes and the target).
