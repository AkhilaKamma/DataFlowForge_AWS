# DataFlowForge_AWS

DataFlowForge is a comprehensive data engineering solution that facilitates the seamless management and orchestration of data flow processes from end to end. The project involves the following key steps:

**Responsive Web UI Development:** Utilizing ReactJS, DataFlowForge provides a user-friendly web interface where users can input text and upload files.
Direct Upload to S3: Users can upload files directly to Amazon S3 from their web browsers, ensuring efficient and secure data transfer without intermediaries.
Data Management with DynamoDB: DataFlowForge integrates with DynamoDB to store input text, file paths, and other metadata in a structured manner, using API Gateway and Lambda functions for seamless interaction.
**Automated Script Execution on EC2:** Upon file upload and DynamoDB entry, DataFlowForge triggers the execution of scripts on EC2 instances. This process involves automatic provisioning of EC2 instances, downloading scripts from S3, and executing them.
**Data Processing and Output Generation:** The executed scripts retrieve input data from DynamoDB and files from S3, perform data processing tasks, and generate output files. The output files are then uploaded back to S3.
**Data Persistence and Lifecycle Management:** DataFlowForge ensures the persistence of output data and associated metadata in DynamoDB, enabling easy retrieval and tracking. Additionally, it automates the termination of EC2 instances to optimize resource usage.
