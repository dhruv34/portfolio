+++
date = '2024-05-03T16:58:26-05:00'
title = 'John Deere | MLOps Engineer'
sub = 'November 2023 - May 2024'
featured_image = '/johndeere.png'
+++

**Java, Python, AWS, APIs, SQL, Databricks**

* Built a scalable data pipeline architecture leveraging AWS CloudFormation, SNS queues, and S3 buckets.
* Developed REST APIs to provide analytics insights for data science teams using Java and Python.
* Enhanced customer request management using Databricks and distributed computing.
* Led testing efforts for MLOps products, creating and executing 200+ unit tests with Pytest-mock.

For most of my junior year, I took a reduced courseload and decided to get some more industry experience before graduating. So, I worked as a part-time engineer in the MLOps team at John Deere, working 10-15 hours per week alongside classes. 

The first two months of my time was spent working on the CI/CD pipeline of the MLOps team I was placed in. I learned how to use GitHub Workflows and created checks on pull requests before allowing developers to push their code such as checking unit test coverage. 

I then stepped in to work alongside team members on multiple tasks. This included a data science project using Databricks for distributed computing and building and testing APIs with Postman and Swagger.

In the final 2 months, I worked on a larger project: creating an AWS architecture for data science teams to easily engage with a large database. The problem was that developers didn't know when data was updated so they had to repeatedly pull the database whenever they began working. This process would take 30 to 40 minutes and would drain valuable time. 

To address this, I used AWS CloudFormation to create a system that notifies developers when data was updated. Specifically, I used an API to poll the data source ever so often and when it detects a change, it would send information about that change to a SNS Queue. I then added data science teams' Microsoft Teams chats as subscribers to the SNS queue so they receive messages when data is updated. I also used EC2 Instances to process and transform the incoming data changes for efficient consumption and S3 buckets to store data about past updates.