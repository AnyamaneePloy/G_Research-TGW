# Unleash GenAI with AWS Serverless

## Agenda
1. **Modern Applications Overview**
: An Intro to building evolvable architecturesusing serverless and other cloud native building blocks, the best practices andbenefits.
2. **Hands-on Lab**
: You will learn to build your very own Intelligent DocumentProcessing App using serverless architecture.
3. **Observability for GenAI**
: Gain real-time insights into model performance,resource utilization, and output quality. Enhance reliability, optimize costs, andensure compliance.
4. **Accelerate development with Amazon Q Developer**
: Learn how GenAIassistant can help at every software development lifecycle and improvedeveloper’s productivity.


## Introduction to Serverless GenAI

Serverless computing is increasingly popular for deploying Generative AI (GenAI) systems due to its scalability, cost efficiency, and reduced infrastructure management. Here's a summary of the pros and how serverless can be applied to GenAI:

### Pros of Serverless for GenAI

1. **Scalability**: Serverless platforms like AWS Lambda and Azure Functions automatically scale to handle sudden spikes in traffic, making them ideal for GenAI applications with irregular workflows[^1][^3].
2. **Cost Efficiency**: Pay-per-use pricing models ensure that you only pay for the compute resources used, reducing costs significantly compared to traditional setups[^1][^3].
3. **Reduced Infrastructure Management**: Developers can focus on building AI models rather than managing servers, which simplifies deployment and maintenance[^1][^4].
4. **Event-Driven Architecture**: Serverless functions execute on-demand in response to events, aligning well with the dynamic nature of GenAI applications[^3].



## Modern Applications Overview
Building modern applications on AWS involves leveraging a range of services and best practices to enhance innovation, scalability, reliability, and cost efficiency. Here's a comprehensive guide to help you build modern applications on AWS:

1. **Culture of Ownership**: Encourage teams to take ownership of their components.
2. **Microservices Architecture**: Modular design for easier scaling and development.
3. **Serverless Computing**: Use AWS Lambda for event-driven, scalable applications.
4. **Decoupled Data Management**: Employ purpose-built databases like DynamoDB.
5. **Developer Agility**: Implement abstraction, automation, and standardization.
6. **Operational Model**: Adopt a serverless-first approach.
7. **Management \& Governance**: Leverage programmatic guardrails for security and compliance[^1][^2].

### AWS Services for Modern Applications

- **Compute Services**:
    - **AWS Lambda**: Serverless computing for event-driven applications.
- **Data Services**:
    - **Amazon S3**: Object storage for data lakes and static content.
    - **Amazon DynamoDB**: NoSQL database for fast data access.
- **Integration Services**:
    - **Amazon SQS**: Message queuing for decoupling components.
    - **Amazon EventBridge**: Event bus for managing event-driven workflows.
- **Security and Governance**:
    - **AWS IAM**: Identity and access management for secure access.
    - **AWS CloudWatch**: Monitoring and logging for operational insights.

### Best Practices for Building Modern Applications

1. **Adopt a Modular Architecture**: Use microservices to increase agility and reduce risk[^2][^3].
2. **Leverage Serverless**: Focus on writing code rather than managing infrastructure[^3][^4].
3. **Implement Continuous Integration/Continuous Deployment (CI/CD)**: Use AWS CodePipeline for automated build and deployment workflows[^1].
4. **Monitor and Optimize**: Use AWS CloudWatch and AWS X-Ray for performance monitoring and optimization[^1].



### Applications and Use Cases

- **RAG (Retrieval-Augmented Generation)**: This architecture can be implemented using serverless functions to manage complex workflows efficiently[^8].
- **Multi-Modal Processing**: Serverless can handle diverse data types and processing needs, making it suitable for multi-modal AI applications.
- **Agent-Based Systems**: Agents can identify user needs and trigger serverless functions to process requests efficiently.


### Example Use Case: 
- **UK Government Application**

    1. **Customer Uploads Image to S3**: The user uploads an image to an Amazon S3 bucket.
    2. **Trigger Lambda Function**: S3 triggers a Lambda function upon upload.
    3. **Image Analysis with Amazon Rekognition**: The Lambda function uses Amazon Rekognition to analyze the image.
    4. **Store Results in Another S3 Bucket**: The analysis results are stored in a separate S3 bucket.

### Technical Implementation

- **SQS for Queueing Requests**: Use Amazon SQS to manage a queue of requests before invoking Lambda functions.
- **Multiple Models**: Employ multiple AI models in a workflow, each triggered by a queue system.
- **EventBridge for Event Handling**: Leverage EventBridge for managing event-driven workflows.


## Hands-on Lab
#### 1. Chatbot
<img src="image\image.png" alt="alt text" width="600" height="315">

#### 2. Document Summarization

<img src="image\image-1.png" alt="alt text" width="600" height="350">

**Testing the RAG Inference**

<img src="image\image-2.png" alt="alt text" width="600" height="350">


**Service in Model**

1. **Amazon S3**: Object storage built to retrieve any amount of data from anywhere.
2. **AWS Step Functions**: Visual workfl ows for distributed applications.
3. **AWS Lambda**: Serverless compute service; Run code without thinking about servers orclusters.
4. **Amazon Bedrock**: The easiest way to build and scale generative AI applications withfoundation models.
5. **Amazon OpenSearch**: Securely unlock real-time search, monitoring, and analysis ofbusiness and operational data.
6. **AWS AppSync**: Connect apps to data and events with secure, serverless, and performantGraphQL and Pub/Sub APIs.


**Summary**

In this module, you learned how to build a custom knowledge base using the OpenSearchServerless database. You explored how to create a Retrieval-Augmented Generation (RAG)pipeline for processing thousands of documents using AWS Step Functions distributedmap, Lambda functions, and LLamaIndex. Additionally, you learned how to managepipeline failures during processing and how to control concurrency to prevent downstreamservices, such as Amazon Bedrock, from being overwhelmed by excessive requests.

---

#### 3. Document extraction and summarization

[Open Data Summarization Notebook](code\02-idp-genai-classify-summarize.ipynb)
[Open Data Extraction Notebook](code\03-idp-genai-data-extraction.ipynb)

<img src="image\image-3.png" alt="alt text" width="600" height="350">

<img src="image\image-4.png" alt="alt text" width="600" height="350">


<div style="text-align: center">⁂</div>

[^1]: https://pages.awscloud.com/rs/112-TZM-766/images/AWS_Modern_Applications_eBook.pdf

[^2]: https://aws.amazon.com/campaigns/modern-application-development-emea/

[^3]: https://d1.awsstatic.com/psc-digital/2023/gc-300/build-mod-apps/build-modern-applications-on-aws.pdf

[^4]: https://aws.amazon.com/modern-apps/

[^5]: https://aws.amazon.com/partners/featured/modern-application-development/

[^6]: https://docs.aws.amazon.com/whitepapers/latest/modern-application-development-on-aws/welcome.html

[^7]: https://pages.awscloud.com/global-ln-gc-300-build-mod-apps-ebook-learn

[^8]: https://www.youtube.com/watch?v=OJD3UMuU8Zk






