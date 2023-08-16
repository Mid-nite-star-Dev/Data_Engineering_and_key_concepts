

# Assignment: Understanding Data Engineering and key concepts 


**What is Data Engineering?**
  Data engineering is the discipline of collecting, storing, transforming, and analyzing data. Data engineers build the systems that make data accessible and useful for businesses and organizations.

## Why is Data Engineering Important?
   Data is the lifeblood of modern businesses. It is used to make decisions, improve products and services, and drive innovation. Data engineers play a critical role in ensuring that businesses have access to the data they need to succeed.


**Research of the following:**
- compare two popular cloud service providers and their offerings for Data Engineering.
- real world case that exemplifies each of the Big data 5Vs consists of (Volume, Velocity, Variety, Veracity, Value)
- Analyze a real-world business case and propose a hybrid solution that combines OLTP and OLAP.
- Explain the key differences between a traditional relational database, a data warehouse, and a data lake.
- Discuss the advantages and challenges of ETL in the context of data engineering.
   
## Assignment Overview

**Question1:    Research and compare two popular cloud service providers and their offerings for data engineering. Analyze the features, pricing models, and scalability options provided by each platform.**

**Azure by Microsoft Vs Amazon Web Services or (AWS) Comparison**:
Cloud computing refers to the on-demand distribution of computing services over the internet and remote data centers (i.e., the cloud) to drive faster innovation, increase resource provisioning flexibility, and help companies gain from economies of scale. Cloud providers like Microsoft Azure and Amazon Web Services (AWS) have functions and services distributed across multiple data centers. Further, cloud computing relies on two methods to enable standardization and cost efficiency: a resource-sharing model and a “pay-as-you-go” paradigm. In simple words, cloud computing allows users to rent rather than buy their IT infrastructure. Customers choose to access computational power offered by service providers like AWS and Azure over the internet or the cloud and pay for it as they use it, rather than investing extensively in databases, software, and hardware

1. **The approach to computing power provisioning and usage**
The primary issue with computing is scalability. To address this, AWS uses elastic cloud computing (EC2), in which the resource footprint available may increase or shrink on-demand as a result of elastic cloud computing resource provisioning. Local clusters provide just a piece of the resource pool that is accessible to all processes simultaneously. 
While Azure users are given the option of creating a VM from a virtual hard disc (VHD). It uses virtual scale sets to provide scalability and enable load balancing. The main distinction is that EC2 may be customized for various uses, whereas Azure VMs work in tandem with other cloud-deployment tools.

2. **Cloud storage offerings**
Success of cloud deployment depends on having adequate storage. In this aspect, Azure and AWS are almost equally strong — however, their offerings in this regard are different. AWS has services like Amazon simple storage service (S3), elastic block store (EBS), and Glacier, 
whereas Azure Storage Services offers blob storage, disk storage, and standard archive. Using AWS S3, customers can gain from a scalable, secure, and robust storage solution for unstructured and structured data use cases. In contrast, Azure offers data storage in Azure Blogs, Azure Queues, Azure Disks, Azure Tables, and Azure Files. Both offer an infinite number of permissible objects. However, AWS has a 5 TB object size restriction, whereas Azure has a 4.75 TB limit. 

3. **Security and data privacy** 
AWS performs an excellent job of selecting secure alternatives and settings by default, ensuring enhanced privacy. Azure uses Microsoft’s Cloud Defender service for security and data privacy – an artificial intelligence-powered solution that protects against new and emerging threats. However, Azure services may not be 100% secure by default, such as virtual machine instances deployed with all ports open unless otherwise configured. 

4. **Documentation and simplicity of use**
AWS offers greater ease of use and is good for first-time cloud platform adopters. The first is the dashboard, which is both feature-rich and user-friendly. AWS also provides extensive documentation for its cloud services. To host a simple EC2 instance, users can type their queries into the AWS search box and navigate to “Documentation” for a video or written lesson. However, adding users and access rules is more complex in AWS.
 Azure keeps all the user accounts and information in one place, although its documentation and recommendations system is less intuitive and search-friendly.

5. **Database capabilities**
The two solutions offer a wide range of database services to handle both structured and unstructured information or big data. In terms of durability in data management, AWS users can gain from Amazon RDS. 
whereas Azure has the Azure SQL server database option. Amazon’s relational database service (RDS) is compatible with six database engines: MariaDB, Amazon Aurora, MySQL, Microsoft SQL, PostgreSQL, and Oracle.
these services are pretty comparable, offering analytics and big data capabilities. For the same, AWS has Elastic MapReduce (EMR), and Azure offers HD Insights. Further, Azure users can access the Cortana Intelligence Suite, covering Spark, Hadoop, HBase, and Storm. In comparison to Azure, AWS provides a relatively mature environment for big data handling. Both systems are compatible with relational and NoSQL databases. 
6. **Pricing model**
In terms of pricing, AWS and Azure both offer reasonable pricing and a pay-as-you-go pricing model. Moreover, both provide free introductory packages to give users an idea about how their systems can be integrated with on-premise software. AWS is billed on an hourly basis, with instances purchasable:

**On-demand:** Pay only for the resources and services you use
**Spot:** Bid for extra capacity availability
**Reserved:** Reserve an instance for up to three years with an upfront payment
Meanwhile, Azure is billed on a per-minute basis, which means users can gain from a more exact pricing component than AWS. It also allows you to enter short-term commitments to choose from prepaid or monthly charges. Short-term subscription plans on Azure provides more flexibility.
However, when the two are compared, Azure usually turns out to be the more expensive option and can add to a company’s cloud costs. 


**Conclusion**
Azure and AWS offer similar features to their customers, and both cloud products are incredibly comprehensive. Users will be able to host various applications, learn about the cloud offering, use AI and ML, and gain from open-source contributions. However, a few key differences remain, mainly in the pricing model and documentation approach.
Most Azure adopters are influenced by the availability of the larger Microsoft ecosystem, including various productivity tools, business apps, and, of course, Windows. On the other hand, AWS can be more affordable and is often the better choice for first-time adopters.

**Question2:  Select a real-world use case that exemplifies each of the 5Vs (Volume, Velocity, Variety, Veracity, Value) of big data.** 
              **Explain how data engineering techniques can be applied to address the challenges and opportunities associated with each V.**

**Volume:**
Volume refers to the colossal amount of data that inundates organizations. We’re well past the days when companies resourced their data internally and stored it in local servers. Companies of 15 years ago handled terabytes of data.
Today, data has grown to petabytes if not exabytes of bytes (that’s 1,000–1 million TB) that come from sources such as transaction processing systems, emails, social networks, customer databases, website lead captures, monitoring devices and mobile apps.
To handle all of this data, managers use data lakes and warehouses or data management systems. They store it on clouds or use service providers such as Google Cloud.
Example of data volume
Walmart operates approximately 10,500 stores in 24 countries, handling more than 1 million customer transactions every hour. The result? Walmart imports more than 2.5 petabytes of data per hour, storing it internally on what happens to be the world’s biggest private cloud.


**Velocity:**
Big data grows fast. Consider that, according to Zettaspere, there are around 3,400,000 emails, 4,595 SMS, 740,741 WhatsApp messages, almost 69,000 Google searches, 55,000 Facebook posts, and 5,700 tweets made per minute.
Around five years ago, data scientists measured incoming data with computerized batch processing that read large files and generated reports. Today, batch processes are unable to handle the continuous rush of real-time data from a growing number of sources.
Example of data velocity
Using real-time alerting, Walmart sales analysts noted that a particular, rather popular, Halloween novelty cookie was not selling in two stores. A quick investigation showed that, due to a stocking oversight, those cookies hadn’t been put on the shelves. By receiving automated alerts, Walmart was quickly able to rectify the situation and save its sales.


**Variety:**
Variety refers to the different types of digitized data that inundate organizations and how to process and mine these various types of data for insights. At one time, organizations mostly gained their information from structured data that fit into internal databases like Excel.
Today, you also have unstructured information that evades management and comes in diverse forms such as emails, customer comments, SMS, social media posts, sensor data, audio, images, and video. Companies struggle with digesting, processing, and analyzing this type of data and doing so in real time.
Example of data variety
Walmart tracks each one of its 145 million American consumers individually, resulting in accrued data per hour that’s equivalent to 167 times the books in America’s Library of Congress. Most of that is unstructured data that comes from its videos, tweets, Facebook posts, call-center conversations, closed-circuit TV footage, mobile phone calls and texts, and website clicks.


**Veracity:**
Veracity is arguably the most important factor of all the five Vs because it serves as the premise for business success. You can only generate business profit and impact change with thorough and correct information.
Data can only help organizations if it’s clean. That’s if it’s accurate, error-free, reliable, consistent, bias-free, and complete. Contaminating factors include:
•  Statistical data that misrepresents the information of a particular market
•	Bugs in software that produce distorted information
•	Human agents that make mistakes in reading, processing, or analyzing data, resulting in incorrect information
       Example of data veracity
According to Jaya Kolhatkar, vice president of global data for Walmart labs, Walmart’s priority is making sure its data is correct and of high quality. Clean data helps with privacy issues, ensuring sensitive details are encrypted while customer contact information is segregated.


**Value:**
Big data is the new competitive advantage. But, that’s only if you convert your information into useful insight.
Users can capture value from that data through:
•	Making their enterprise information transparent for trust
•	Making better management decisions by collecting more accurate and detailed performance information across their business
•	Developing the next generation of products and services
Example of data value
Walmart uses its big data to make its pharmacies more efficient, help it improve store checkout, personalize its shopping experience, manage its supply chain, and optimize product assortment among other ends.


**Question3: Analyze a real-world business case and propose a hybrid solution that combines OLTP and OLAP systems to meet both transactional and analytical data processing requirements.** 
                **Justify your solution and discuss potential benefits and challenges.**

A mixed workload database is capable of handling both OLAP and OLTP workloads in one system. Which can be describe as a Hybrid Transaction Analytical Processing (HTAP), It has the ability to record data updates through transactions, and at the same time performs large, intensive analytical queries, mixed workload databases were invented to reconcile both worlds.
The most advanced mixed workload databases can process short transactions, long transactions, short queries and complex queries at the same time. No need to wait for a transaction to be committed before starting a new transaction and vice versa. A significant advantage of such a system is that it removes the latency between the transactional environment where data is created, and the analytical environment where data is explored. As a result, users are able to interactively explore data that is updated incrementally in real-time.
A real-world case is a front office risk analytics applications used by traders, where the mixed workload implementation allows traders to analyse their risk exposure at any time across many dimensions (currency, counterparty…) and with various levels of aggregation (at portfolio level or at the most granular level of the trade id). Typically risk intelligence also needs to be propagated at various levels in the organization in real-time. A mixed workload system will allow both the desk manager and the head of trading to see aggregated risk data across all trading desks and all risk class assets with instant updates as market data change.

**Benefits of Hybrid Transaction Analytical Processing (HTAP) For OLTP and OLAP**

•Unifying transactional and analytical data unlocks many new opportunities to extract value from data stores. Although running parallel OLTP and OLAP systems is still common practice for many organizations, the advantages of uniting these two systems has made HTAP an increasingly popular choice. 

•HTAP can minimize the need for creating ETL pipelines to copy data from OLTP to OLAP databases. Moving data can be costly and resource-intensive. Since transactional and analytical data is handled together within the HTAP system, ETL pipelines aren’t necessary to make this data available for analytics.

•With data available for analytical querying as soon as it’s created, an HTAP database allows organizations to capture value from transient opportunities that would be lost in the time needed to transfer data from an OLTP to OLAP database. 

•With only one system to manage, HTAP reduces operational complexity and costs. An HTAP database architecture streamlines data management, freeing IT and data professionals to focus on higher-level, value-added tasks.

**Challenges of Hybrid Transaction Analytical Processing (HTAP) For OLTP and OLAP**

•The main technical challenges for an HTAP database are how to be efficient both for operational (many small transactions with a high fraction of updates) and analytical workloads (large and complex queries traversing large number of rows) on the same database system and how to prevent the interference of the analytical queries over the operational workload. This kind of operational workload is also commonly referred to as Operational Analytical Processing.

•Some challenges for HTAP include limited industry experience and skills, as well as undefined best practices.


**Question4:  Explain the key differences between a traditional relational database, a data warehouse, and a data lake. When would you recommend using each of these storage solutions in a data engineering project?**

A database is used to store, search and report on structured data from a single source. They are the simplest to create and SQL can be used to query and report on the data. There are both open source and proprietary databases, making it widely accessible to install and start using on premise or on the cloud.

A relational database requires schemas and are not a fit for unstructured or semi-structured data. Because of this rigid schema, they are not suited to be the centralized place to store data from multiple sources where the raw data varies in format and structure. However, they are popular for data analysis and monolithic applications.

A data warehouse is used to store large amounts of structured data from multiple sources in a centralized place. The process of creating a data warehouse requires some heavy lifting in the planning and design stage of examining data structures. Data warehouses are preferred by the business and operations decision makers of the company and a good system justifies its often-high costs in proprietary software and storage.

A data lake stores structured, semi-structured and unstructured data, supporting the ability to store raw data from all sources without the need to process or transform it at that time.
Only when the data needs to be retrieved, will some structure need to be applied, which is ideal in the hands of data scientists and data analysis developers who can create new data models on the fly but does not provide the same reporting capabilities and ease of use for business users. Storing data in data lakes is much cheaper than in a data warehouse. Data lakes are very popular in the modern stack because of its flexibility and costs but they are not a replacement for data warehouses or relational databases.

A Data use case:
Shipping Company: They sell gadgets online and outsource fulfillment to others. They use a basic database to track orders and often discard records not long after the orders have been delivered. Their products change frequently and so they feel they have no need for historical data.

A Data warehouse use case:
Banking and finance: A data warehouse is often the best storage model for these sectors, as they allow structured access by the entire company rather than a single data scientist.

A Data Lake use case:
Healthcare: Data warehouses have been used for many years in the healthcare industry. Due to the large amounts of unstructured data in healthcare (i.e. physicians’ notes, clinical data, etc.)
and the need for real-time insights, the use of data lakes allows access to structured and unstructured data, which turns out to be a better fit for healthcare companies.


**Question5: Discuss the advantages and challenges of ETL in the context of data engineering.**
			
**Advantages Of ETL**

ETL allows data engineers to apply consistent and standardized transformations to the data before loading it into the target, ensuring that the data is clean, accurate, and compatible. 

ETL also enables data engineers to enforce data quality rules and validations at the source level, preventing errors and anomalies from propagating downstream. 

ETL can also improve the performance and efficiency of the target system, as the data is already optimized and structured for querying and analysis.

With data governance comes data democracy as well. That means making your corporate data accessible to all team members who need it to conduct the proper analysis necessary for driving insights and building business intelligence.
It does so by creating a single point-of-view so that you can make sense of the data easily. It also lets you put new data sets next to the old ones to give you historical context.
				
**Challenges of ETL**

ETL can be time-consuming and resource-intensive, as the data has to go through multiple stages and systems before reaching the target. 

ETL can also limit the flexibility and agility of data engineering, as any changes or additions to the data sources or transformations require modifying and testing the ETL code or tools.

ETL can also reduce the availability and completeness of the data, as some data may be filtered out or discarded during the transformation process. You may end up with some data loss, corrupted or irrelevant data because some processes in the transformation phase may not have performed correctly. You may also end up dealing with many bottlenecks because of insufficient memory or CPU.
In such cases, you may need to conduct a host of different data transformations. That defeats the whole purpose of ETL.


# Key Concepts in Data Engineering

1. **Data collection**: The process of gathering data from a variety of sources, such as databases, sensors, and social media.
2. **Data storage**: The process of organizing and storing data in a way that is efficient and secure.
3. **Data transformation**: The process of cleaning, transforming, and enriching data so that it is ready for analysis.
4. **Data analysis**: The process of exploring, querying, and modeling data to extract insights.
5. **Data visualization**: The process of presenting data in a way that is easy to understand and interpret.



## Contribution and Feedback

Contributions are welcomed to enhance and extend this Data Engineering and key concepts further. or provide feedback to help improve the Assignment Research.


