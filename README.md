# opensearch-embedding-example
A sample project that shows how to store and retrieve content in an OpenSearch serverless database using embeddings

Note: this solution creates a public OpenSearch serverless instance. You should make this private for production use. 

To start, install the [CloudFormation template](opensearch.yml). You must provide the ARN of the user or role that should have admin access to the OpenSearch serverless cluster. 

Once the CloudFormation template has successfully completed, open the [demo.ipynb](demo.ipyb) notebook. Modify the first cell in the notebook for your region and OpenSearch host name. Note: the OpenSearch host name is available on the **Outputs** tab of the CloudFormation console for this stack.

The notebook walks you through uploading the IMDB top 1000 movies database and shows how you can then perform searches against the "Overview" column, which is also stored as an embedding via Titan Text embeddings.