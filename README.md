# Azure-Data-Factory---Data-Engineering-With-Real-Time-Project-Notes
This Repository contains my Notes of "Azure Data Factory - Data Engineering With Real Time Project" Course from Udemy

**I) Introduction**

**A) Data Analytics And Data Engineering Introduction**

**B) Azure Data Analytical Services Introduction**

**C) Azure Cloud Fundamentals Introduction**

**D) Free Azure Account for Students**

**E) Free Azure Account for All**




# **I) Introduction**

# **A) Data Analytics And Data Engineering Introduction**

The data analytics domain has experienced exceptional growth in the software industry over the past ten years, and this trend is expected to continue. This growth has created numerous job opportunities, particularly in emerging technologies. One such in-demand role is that of an Azure Data Engineer. Understanding the day-to-day responsibilities of a data engineer is crucial to grasp how data analytics projects are developed and executed.

A practical example of a data analytics project involves analyzing product pricing data across multiple markets in India. For instance, examining the pricing of onions across 547 markets on a given day can reveal significant insights, such as identifying markets where onions can be purchased cheaply and sold at a much higher price elsewhere. These insights, derived from the data, can lead to substantial monetary benefits, and the operations performed on the data—like filtering and aggregation—are collectively called data transformation. Data engineers are responsible for performing these transformations to extract valuable information from raw data.

Before transforming the data, it is essential to understand its origin. Most data for analytics projects comes from enterprise software systems that support day-to-day business operations, such as e-commerce websites in retail. These systems, known as Online Transactional Processing (OLTP) systems, capture transactional data, which can then be used for analytics. Additionally, open-source data has emerged as a significant contributor to data analytics, allowing solutions to be developed independently of any specific business.

Data comes in various formats, broadly classified as structured, semi-structured, and unstructured. Structured data includes delimited text files, Excel sheets, and database tables, where the format and column names are consistent. Semi-structured data, like JSON or XML, allows each row to have its own schema, using key-value pairs. Unstructured data, such as zip files, videos, audio files, and certain binary formats like NetCDF, lacks a predefined structure and can contain diverse content.

The primary tasks of a data engineer can be summarized into three steps: ingest, transform, and publish. First, the data engineer ingests raw data from various source systems into a centralized analytics platform. Next, the data is transformed through filtering, aggregations, and other operations to derive useful insights. Finally, the transformed data is published, storing it permanently for use by other roles, such as data analysts and machine learning engineers, in Online Analytical Processing (OLAP) systems. In data warehousing terminology, this entire process is often referred to as ETL (Extract, Transform, Load).

In summary, the data engineer plays a pivotal role in developing data analytics projects. They are responsible for identifying source systems and data formats, ingesting raw data into an analytical platform, transforming it to extract insights, and storing the results permanently for further use. These core operations enable businesses and analysts to leverage data effectively for decision-making and creating value.

# **B) Azure Data Analytical Services Introduction**

In our previous introduction lesson, we identified the role of a Data Engineer in building a data analytics project. A Data Engineer’s day-to-day tasks primarily revolve around three layers: the ingest layer, the transform & integrate layer, and the model & publish layer. The ingest layer is responsible for extracting data from various source systems and loading it into the analytics platform. The transform & integrate layer processes the raw data, integrating multiple datasets to extract meaningful information. Finally, the model & publish layer applies data modeling techniques and stores the transformed insights for reporting and analytical purposes.

There are three main types of source systems from which data is extracted. First, web services provide delimited files, which often contain transactional or pricing information. Second, OLTP databases provide structured tabular data such as master data and market information. Third, third-party APIs provide JSON-formatted data, including open-source datasets like weather information and country profiles (for example, GDP growth rates). Collectively, these datasets form the raw inputs for building the analytics platform.

To build the ingest layer, we use Azure Data Factory (ADF). ADF has inbuilt connectors for more than 100 source systems, making it ideal for extracting data in multiple formats. Although ADF handles data processing, it cannot store data internally, which is why we use Azure Data Lake Storage Gen2. This storage service can store any type of data in its original format, including CSV, JSON, compressed files, binary files, and video files. Even table data from OLTP databases is converted into files during ingestion, ensuring consistent storage for all source data.

For the transform and integrate layer, Azure Data Factory again plays a central role. ADF supports a wide range of transformations such as joins, unions, lookups, derived columns, aggregations, ranking, and pivot/unpivot operations. Using these features, we can transform raw data and integrate datasets from multiple sources into a consolidated view. This layer prepares data for final modeling and analytics while maintaining high processing efficiency.

The model and publish layer stores the transformed data in a format suitable for reporting or analytics. We use Azure SQL Database for structured, tabular data to support reporting needs. For large or semi-structured datasets, such as JSON data from APIs, we continue to use Azure Data Lake Storage Gen2. This layer often employs dimensional data modeling techniques for reporting and the medallion architecture (bronze, silver, and gold tables) for building the data lake. These techniques ensure that the analytics platform is structured, flexible, and scalable for both reporting and machine learning purposes.

The data analytics platform supports two types of users. Reporting users build reports to understand organizational operations and trends, relying on tools like Power BI. For reporting purposes, the pricing data, master data, market data, and country profiles are integrated into dimension and fact tables using dimensional modeling techniques. These tables are populated daily through automated pipelines, which include delta records processing (only processing new or changed data) and scheduled transformations for continuous updates.

On the other hand, artificial intelligence and machine learning users require additional data to build predictive models. This includes population data per market, weather information within market regions, and country profile data for import/export potential. These datasets are processed and integrated into the data lake using semi-structured data processing techniques and Azure Data Factory pipelines. The resulting bronze, silver, and gold tables provide a consolidated, structured view for machine learning models to predict future trends, such as pricing changes.

Beyond data processing, the platform also includes security, operational support, and code management. Microsoft Entra and Key Vault are used to secure the platform, while Azure Monitor and Log Analytics Workspace provide operational monitoring and alerting. Code management involves a development environment, followed by testing and deployment to production using Git repositories and CI/CD pipelines. This ensures smooth, controlled delivery of analytics workflows and daily operations for end users.

Overall, the course covers the complete lifecycle of a data analytics project: from extracting data from multiple sources, transforming and integrating it, modeling for reporting and ML, to securing, operationalizing, and managing the code. Each layer and operation is supported by specific Azure services, providing a robust, scalable, and enterprise-ready analytics platform.

# **C) Azure Cloud Fundamentals Introduction**

Before we start using Azure Data Analytical services to build our data analytics platform, it is important to understand the basics of cloud computing. To do that, we first look at a non-cloud environment. For example, the laptop you are using is a non-cloud environment because all software and hardware components exist locally on your machine. Any software application development in this environment requires certain mandatory hardware and software components.

The first essential component is the processor, which executes all operations, such as opening applications or processing data. Next is memory, which stores data during processing. There are two types of memory: virtual memory, used by the operating system while loading and processing data, and physical memory, where data is physically stored. On top of this, the operating system is necessary to make the hardware available for software applications. Finally, networking is required to provide access to the applications for other users. These are the core components of a non-cloud setup.

In the cloud environment, all these components—processors, memory, operating systems, and networking—are available remotely through data centers. Cloud providers like Microsoft Azure have built multiple data centers across the globe; for example, Azure has over 300 physical data centers. Each data center contains networked computer servers equipped with all the hardware and software components needed for software development. These data centers are interconnected using Microsoft-owned network cables to ensure global connectivity.

To access and use these cloud resources, Azure provides a browser-based front-end interface called the Azure Portal (portal.azure.com). Through this portal, users can create an Azure account, log in, and provision resources directly in the cloud. Azure accounts require credit card information because charges are based on the resources consumed. Once logged in, users can create virtual machines, storage, databases, and other cloud resources and start developing software applications entirely in the cloud without needing physical hardware locally.

For beginners, Azure also provides a free account, typically valid for 30 days, allowing users to explore most of the services needed for development. This free account is ideal for following along with this course and practicing the creation of cloud resources. Understanding this cloud infrastructure and interface is sufficient to start building your data analytics platform using Azure services.

In the next lesson, we will go step by step to create a free Azure account and begin using these cloud resources for application development and data analytics.

# **D) Free Azure Account for Students**

If you are a student and have a university or college email ID, you can create a free Azure student account without providing any credit card information. To do this, simply search for “Azure Free Student Account”, which will take you directly to the student account signup page. This account provides free access for one year with a $100 credit that you can use for Azure services throughout the year.

To get started, click on “Start Free”. You will need to fill in some basic details, including your first name, surname, country, school name, date of birth, and your student email address. Once you submit these details, a verification code will be sent to your student email. Enter this code on the portal and complete the quick puzzle or captcha if prompted.

After verification, your student Azure account will be activated for 12 months. You can then use your student email ID to log in at any time and start accessing your free credit to explore Azure services. This setup allows students to experiment and learn on Azure without worrying about charges or providing a credit card.

# **E) Free Azure Account for All**

If you are not a student, you can still set up a free Azure account. First, go to Outlook.com and create a new email ID for yourself. Even if you already have an Outlook email ID, it’s recommended not to use the existing one for setting up a free Azure account. In some cases, free Azure accounts are refused for existing emails because they might have been used previously to create a free account. So, always create a new Outlook email ID for this purpose.

Once you have created your new email ID, log in to portal.azure.com using that email. You may be prompted to take a short tour, but you can skip it. You will see the option to “Start with Azure Free Trial”—click the start button. The portal will ask you to re-enter your details. Most details are automatically taken from your email account, but make sure to provide accurate information, as this will be linked to your credit card for verification.

Enter your mobile number (with the correct country code) and then proceed to receive a verification code via SMS. Enter the code to verify your phone number. Next, provide your address details and check all required boxes to continue.

The portal will then ask for your credit card details. Don’t worry about charges—Microsoft will only validate your credit card, and no actual billing occurs unless you switch to a pay-as-you-go subscription. Usually, a small temporary authorization (up to $1) is applied to verify your card. Once entered, click Sign Up to complete the process.

After your account is successfully created, go back to portal.azure.com and log in with your new credentials. In the portal, search for “Subscriptions” using the search bar and click on it. You should see “Azure Subscription 1”, indicating that your free Azure tenant has been successfully set up. This confirms that your account is ready to start creating and managing Azure resources.
