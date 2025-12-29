# Azure-Data-Factory---Data-Engineering-With-Real-Time-Project-Notes
This Repository contains my Notes of "Azure Data Factory - Data Engineering With Real Time Project" Course from Udemy

**I) Introduction**

**A) Data Analytics And Data Engineering Introduction**

**B) Azure Data Analytical Services Introduction**

**C) Azure Cloud Fundamentals Introduction**

**D) Free Azure Account for Students**

**E) Free Azure Account for All**

**II) Azure Portal Overview and Create Data Analytical Resources**

**A) Please Watch - Using Support Files Under Resources For Hands On**

**B) Azure Portal Overview and Setup Resource Group**

**C) Setup Azure Data Factory**

**D) Setup Azure Data Lake Storage Gen2**

**E) Summary**

**III) Azure Data Factory Introduction**

**A) Azure Data Factory Studio Overview**

**B) Azure Data Factory Pipeline Overview**

**C) Copy Data Activity - Configure Source Dataset**

**D) Copy Data Activity - Configure Sink Dataset**

**E) Debug Pipeline**

**F) Recap Data Factory Components**

**G) Recap Copy Data Activity - Load JSON Data**

**H) Azure Data Factory Components Summary**

**IV) Data Ingestion Pipeline - HTTP Source**

**A) Data Ingestion Pipeline Requirement**

**B) Pipeline Expression Builder & Dataset Parameters Overview**

**C) Creating & Configuring Dataset Parameters**

**D) Pipeline Parameters Overview**

**E) Creating & Configuring Pipeline Parameters**

**F) Debugging & Dynamically Passing Parameter Values**

**G) Recap Dataset and Pipeline Parameters**

**H) Identify Static and Dynamic Parameter Values**

**I) Configure Static Pipeline Parameter Values**

**J) Dynamic Pipeline Expressions Using Pipeline Parameters & ADF Functions**

**K) Data factory DATETIME format overview & Error Handling in Ingestion Pipeline**

**L) Formatting DATETIME Values Using Advanced Expressions and Date Functions**

**M) Configuring Pipeline Variables and SET VARIABLE Activity**

**N) ADF Triggers Overview**

**O) Create & Configure Tumbling Window Trigger**

**P) Passing Tumbling Window Trigger System Variables To Pipeline Parameters**

**Q) Monitor Automated Pipeline Runs Via Tumbling Window Trigger**

**V) Metadata Driven Data Ingestion Pipeline - HTTP Source**

**A) Metadata Driven Ingestion Pipeline Overview**

**B) Metadata Driven Ingestion Pipeline Requirement**

**C) Create Metadata File**

**D) Upload Metadata File and LOOKUP Activity Overview**

**E) Configure LOOKUP Activity - Read Metadata File**

**F) Configure LOOKUP Activity Settings & Read Metadata File Values as Array**

**G) Configure FOR EACH Activity to Loop Through LOOKUP Output Value Array**

**H) Configure FOREACH Activity To Pass Metadata Values to Dataset Parameters**

**I) Debugging Metadata Driven Ingestion Pipeline & Error Handling**

**J) Organising Folder Structure in ADF**

**K) End To End Metadata Driven Ingestion Pipeline - Create Metadata File**

**L) End To End Metadata Driven Ingestion Pipeline - Create Datasets**

**M) End To End Metadata Driven Ingestion Pipeline - Create Pipeline Part 1**

**N) End To End Metadata Driven Ingestion Pipeline - Create Pipeline Part 2**

**O) End To End Metadata Driven Ingestion Pipeline - Debugging And Error Handling**

**P) End To End Metadata Driven Ingestion Pipeline - Create Tumbling Window Trigger**

**Q) Data Ingestion From HTTP Web Server - Summary**

**VI) Reporting Database Design - Dimensional Data Modelling ( Star Schema )**

**A) Dimensional Data Modelling Overview**

**B) Dimensional Data Modelling - Source Data Overview**

**C) Identify Business Description(Dimension) and Business Measures(Fact) Columns**

**D) Identify Business Description(Dimension) Column Groups Having 1-1 Relationship**

**E) Logical Data Modelling - Designing Dimension Tables**

**F) Logical Data Modelling - Designing Fact Tables**

**G) Physical Data Modelling Overview**

**H) Physical Data Modelling - Identifying Data Types**

**I) Physical Data Modelling - Applying Naming Conventions**

**J) Physical Data Modelling - Including Audit Columns and Define Database Schema**

**K) Setup AZURE SQL DATABASE - Overview**

**L) Azure SQL Database Query Editor Overview**

**M) SQL Server Management Studio Overview**

**VII) Dimension Tables Load - ADF DATAFLOW Overview**

**A) Dimension Table Load Overview**

**B) Dimension Table Load - Data Transformations Overview**

**C) Dimension Table Load - Configure Source Dataset**

**D) Dimension Table Load - Configure SQL Database Linked Services and Sink Dataset**

**E) Dimension Table Load - COPYDATA Limitations and Usage Requirement for DATAFLOW**

**F) Dimension Table Load - DATAFLOW Overview**

**G) Dimension Table Load - DATAFLOW SELECT Transformation**

**H) Dimension Table Load - DATAFLOW AGGREGATE Transformation**

**I) Dimension Table Load - DATAFLOW EXPRESSION BUILDER Overview**

**J) Dimension Table Load - DATAFLOW SURROGATE KEY Transformation**

**K) Dimension Table Load - DATAFLOW DERIVED COLUMN and SINK Transformation**

**L) Dimension Table Load - Recap DATAFLOW Transformations & Debugging DATAFLOW**

**M) Dimension Table Load - Change Data Capture (CDC) Overview**

**N) Dimension Table Load - Change Data Capture Add Sink Data Into Source Stream**

**O) Dimension Table Load - Change Data Capture LOOKUP Transformation**

**P) Dimension Table Load - Change Data Capture FILTER Transformation**

**Q) Dimension Table Load - Change Data Capture SURROGATE KEY Limitation**

**R) Dimension Table Load - Change Data Capture Get Max SURROGATE KEY Using Query**

**S) Dimension Table Load - Merge Max SK with Source Using JOINER Transformation**

**T) Dimension Table Load - Merge Max SK JOINER Transformation Custom Join Condition**

**VIII) Reusable DATAFLOW Design For Loading Dimension Tables**

**A) Reusable DATAFLOW Design - Create Source and Sink Datasets**

**B) Reusable DATAFLOW Design - Configure Source Transformation**

**C) Reusable DATAFLOW Design - Generate Dynamic SQL Query Using Dataflow Parameter**

**D) Reusable DATAFLOW Design - Dynamic SQL Query Import Projection**

**E) Reusable DATAFLOW Design - Dynamic SQL Query For Max Surrogate Key Value**

**F) Reusable DATAFLOW Design - Configure SELECT , AGGREGATOR and LOOKUP**

**G) Reusable DATAFLOW Design - Configure FILTER , JOINER and DERIVED COLUMN**

**H) Reusable DATAFLOW Design - Configure SINK & Pipeline To Automate Run**

**I) Reusable DATAFLOW Design - Debugging**

**J) Reusable DATAFLOW Design -Produce Dimension and Fact Tables CREATE SQL Scripts**

**K) Reusable DATAFLOW Design - Reusing to Populate DIM_MARKET Dimension Table**

**L) Reusable DATAFLOW Design - Reusing to Populate DIM_PRODUCT Dimension Table**

**M) Reusable DATAFLOW Design - Reusing to Populate DIM_VARIETY Dimension Table**

**N) Reusable DATAFLOW Design - Debugging Run Of Loading All Dimension Tables**

**IX) Incremental Load ( Delta Records Processing ) - Dimension Tables Load**

**A) Incremental Load Overview**

**B) Incremental Load - GET METADATA Activity Overview**

**C) Incremental Load - GET METADATA Activity Filter Metadata Between Dates**

**D) Incremental Load - IF CONDITION Activity Overview**

**E) Incremental Load - IF CONDITION Activity For EXCEPTION Handling**

**F) Incremental Load - ADF Single Pipeline Limitations & Workaround(Multi Pipeline)**

**G) Incremental Load - Calling and Passing Values Between Parameters**

**H) Incremental Load - Designing Reporting Tables Load Master Pipeline**

**I) Incremental Load - Calling Reporting Dimension Load From Master Pipeline**

**J) Incremental Load - Using Master Pipeline GET METADATA output in Child Pipeline**

**K) Incremental Load - Debugging Dimension Tables Load Part 1**

**L) Incremental Load - Debugging Dimension Tables Load Part 2**

**M) Incremental Load - Configure Tumbling Window Trigger**

**N) Incremental Load - Test Tumbling Window Trigger Run**

**O) Incremental Load - Fixing Data Quality Error on DIM_VARIETY Table Load**

**P) Loading DIM_DATE Dimension Table - Using INSERT STATEMENTS**

**Q) Data Ingestion Pipeline - HTTP Source Full Load Using Tumbling Window Trigger**

**X) Fact Table Load DATAFLOW Design**

**A) Fact Table Load Transformation Overview**

**B) Fact Table Load DATAFLOW - Configure Source File**

**C) Fact Table Load DATAFLOW - Configure Dimension Table Source & LOOKUP SurrogateID**

**D) Fact Table Load DATAFLOW - Configure All Dimension Tables & LOOKUP SurrogateIDs**

**E) Fact Table Load DATAFLOW - Configure DATE Dimension Table & LOOKUP SurrogateID**

**F) Fact Table Load DATAFLOW Debugging and Fixing Data Issues**

**G) Fact Table Load DATAFLOW - Configure SINK Transformation**

**H) Fact Table Load DATAFLOW Testing Part 1**

**I) Fact Table Load DATAFLOW - Add Tumbling Window Trigger**

**J) Fact Table Load DATAFLOW - Testing End to End Reporting Database Load**

**XI) Data Lake Design - Medallion Architecture**

**A) Data Lake Design Overview**

**B) Data Lake Design - Setup Container and Folder Structure**

**C) Data Lake Design - Additional Source Data Requirements**

**D) Data Lake Design - Additional Source Data Format Overview**

**XII) Data Lake Bronze Layer Data Ingestion - Demographics Data REST API**

**A) Demographics Data Ingestion Overview**

**B) HTTP Request Vs REST API REQUEST RESPONSE Overview**

**C) Demographics Data Ingestion - Configure Linked Service**

**D) Demographics Data Ingestion - Configure Source and Sink Datasets**

**E) Demographics Data Ingestion - Create Ingestion Pipeline**

**F) Demographics Data Ingestion - Configure Pipeline Parameters**

**G) Demographics Data Ingestion - Create and Upload Metadata File**

**H) Demographics Data Ingestion - Configure LOOKUP and FOREACH Activity**

**I) Demographics Data Ingestion - Pass Dataset Parameter Values From Metadata File**

**J) Demographics Data Ingestion - Identifying and Fixing The Errors**

**K) Demographics Data Ingestion - Identifying and Fixing User Errors**

**XIII) Data Lake Bronze Layer Data Ingestion - Weather Data REST API**

**A) Weather Data Ingestion Overview**

**B) Weather Data Ingestion - Dynamic Metadata File Creation Configure Source**

**C) Weather Data Ingestion - Dynamic Metadata File Creation Configure Source Schema**

**D) Weather Data Ingestion - Dynamic Metadata File Creation FLATTEN Complex JSON**

**E) Weather Data Ingestion - Dynamic Metadata File Config Additional Params and SINK**

**F) Weather Data Ingestion - Dynamic Metadata File Creation & DATAFLOW Partitioning**

**G) Weather Data Ingestion - Configure Source and Sink Datasets**

**H) Weather Data Ingestion - Configure LOOKUP and FOREACH Activity**

**I) Weather_Data_Ingestion-Configure_Pipeline_Parameters_and_Variables**

**J) Weather Data Ingestion - Pass Dataset Parameter Values Using Pipeline Expression**

**K) Weather Data Ingestion - Configure Dynamic Subfolder Creation in Sink Storage**

**L) Weather Data Ingestion - Pipeline Debugging and Known Error on Activity Name**

**M) Weather Data Ingestion - Additional Source Column on COPYDATA and Setup Trigger**

**XIV) Data Lake Silver Layer Data Transformation - Demographics Data**

**A) Demographics Data Transformation - Configure Source and Sink Datasets**

**B) Demographics Data Transformation DATAFLOW Source Wildcard Paths Configuration**

**C) Demographics Data Transformation DATAFLOW - FLATTEN Complex JSON Structure**

**D) Demographics Data Transformation DATAFLOW - Naming Conventions & Configure SINK**

**E) Demographics Data Transformation DATAFLOW - Configure Pipeline & Pass Parameters**

**F) Demographics Data Transformation DATAFLOW Pipeline Debugging And Testing**

**XV) Data Lake Silver Layer Data Transformation - Weather Data**

**A) Weather Data Transformation - Configure Source and Sink Datasets & DATAFLOW**

**B) Weather Data Transformation - FLATTEN Nested JSON ARRAY Values Level1**

**C) Weather Data Transformation - FLATTEN Nested JSON ARRAY Values Level2**

**D) Weather Data Transformation - Remove Duplicates and Create Transform Pipeline**

**E) Weather Data Transformation - Removing Unwanted Source Columns & Set Parameters**

**F) Weather Data Transformation - Dynamic DATAFLOW Parameter Passing From Pipeline**

**G) Weather Data Transformation - Identifying and Fixing User Errors**



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

# **II) Azure Portal Overview and Create Data Analytical Resources**

# **A) Please Watch - Using Support Files Under Resources For Hands On**

We’re going to be doing a lot of hands-on work in this portal — starting from creating resources, to using those resources while developing the code that will make your life much easier.

Under the Resources section of this course, I’ve included supporting documents for each of the hands-on exercises you’ll be working on. You can go to the Resources section for each hands-on video, download the corresponding document, and follow along. Inside each supporting document, you’ll find step-by-step instructions that guide you through creating resources or developing the required code.

This will make your work a lot easier because you won’t need to constantly refer back to the video whenever you get stuck with a particular property or configuration option.

I’ve also included naming conventions for all the resources we create and have followed the same pattern in the code as well, so you can quickly reuse them and maintain consistency.

For example, when creating a Resource Group, I’ve given it a specific name in the document — and you’ll also see a small hint suggesting that you can replace part of that name with your initials. This ensures that each resource you create remains uniquely identifiable while still following the same logical naming pattern.

So, as you go through each hands-on activity in the Azure Portal, make sure to download the supporting documents from the Resources section, refer to them while working, and follow the naming conventions provided. This will keep your setup organized, consistent, and easy to navigate throughout the course.

# **B) Azure Portal Overview and Setup Resource Group**

Now we have set up our free Azure account. We can log in to the Azure portal by typing portal.azure.com in the browser. I would like you to memorize this URL because we are going to create resources inside this portal, develop our code within this portal, and deploy that developed code into other infrastructures that also exist within the Azure portal. So please remember this URL — portal.azure.com.

When you type this address, it will take you to the sign-in page. Enter the email ID that you used while setting up your free account, provide your password, and you will be logged into the home page of the Azure portal. As I mentioned earlier, we are going to use this portal for all our development and deployment activities. Therefore, it’s important for us to understand the various options available within the portal.

There are many options available here. However, rather than giving a high-level overview of every option right now, we will learn about each one gradually as we start using them. This approach ensures that you not only understand what each option does but also remember when and where to use it effectively.

Okay, now let’s quickly recall the data analytical project architecture that we designed previously. We are going to build three different layers in our project, and in each of these layers, we’ll be using specific sets of technologies. Using those technologies, we will perform the necessary setup operations for each layer.

We will first focus on our Connect and Ingest layer. For logical reference, I have named it Connect and Ingest. However, in real-time projects, this layer is typically called the Landing, Raw, or Bronze layer. These are standard terminologies used in data analytics projects.

The term Landing means this is the first layer in the analytical project where the source data lands. That’s why we call it the Landing Layer. Some projects refer to it as the Raw Layer because the source data is copied here in its original, unprocessed form — the raw format.

The Bronze Layer terminology comes from a data lake architecture known as the Medallion Architecture, which consists of three layers — Bronze, Silver, and Gold. In that architecture, the first set of data that lands into the data lake is stored in the Bronze layer.

In our project, we are going to refer to it as the Landing Layer because that is more relevant for our context. From now on, I will not refer to it as the Connect and Ingest layer anymore — we will simply call it the Landing Layer.

To build the Landing Layer, we need two key technologies in Azure Cloud — Azure Data Factory and Azure Data Lake Storage Gen2. We need to create these resources inside the Azure Cloud Portal. The process of creating resources in the cloud is known as Provisioning. So, provisioning resources simply means creating the required cloud services within Azure. Don’t worry too much about this terminology for now — we’ll revisit it as we progress.

Now, the first step for us is to create the required resources in this portal. Since we are already logged in, let’s understand how Azure organizes everything. Any resource that we create in the Microsoft Azure portal must follow a standard hierarchy.

The topmost hierarchy is called a Management Group or Azure Tenant. In our case, our Azure account itself is the topmost level — either the Tenant or the Management Group. Inside a Tenant, you can have one or more Subscriptions. For our setup, we currently have only one subscription.

However, in real-time projects, there are usually multiple subscriptions because in a corporate environment, different departments use different sets of Azure services. For example, the web development team might use certain services that differ from what the data analytics team uses. Hence, each department often has its own subscription and its own set of resources.

This is the second level in the hierarchy. So, under a Management Group, you can have one or more Subscriptions. Inside each Subscription, the third level in the hierarchy is the Resource Group.

A Resource Group is essentially a logical container that can hold all resources related to a single project or environment. This hierarchy must always be followed when creating any resource in Azure.

When you create new resources, your Tenant is usually selected by default (since we only have one), and your Subscription will also be preselected. But in real-world projects, you’ll often need to choose the appropriate subscription manually — the one allocated to your project or team.

At the moment, we haven’t created any Resource Groups yet. We only have a Subscription. So, for our project, we’re going to create a new Resource Group shortly.

Another important property that’s required when creating any resource in Azure is the Data Center Region. The data center represents the physical location where your resources are actually hosted. The Azure portal is just the interface that lets us communicate with this physical infrastructure.

So, when creating any resource, you must specify the Region — which is a mandatory field. Without selecting a region, you won’t be able to create a resource in the Azure portal.

Now, let’s go ahead and create our first Resource Group. Without it, we won’t be able to create the two resources needed for our analytical project — Azure Data Factory and Azure Data Lake Storage.

Let’s start by navigating back to the Home page. From here, I’ll guide you using directions like left, middle, and right on the screen. Let’s agree on a common understanding — when I say left, I mean the beginning of the screen (top left or bottom left area). When I say right, it refers to the other side of the screen (top right or bottom right). And when I say center, I’m referring to the middle area of the screen — usually where the search bar is located.

So, now, look at the top left corner — you’ll see three horizontal lines. Click on that. This is one of the options available to create resources in Azure. Microsoft provides multiple ways to perform the same action in its interfaces, just like Windows does.

One way to create a resource is from this menu, and another commonly used way is through the Home button, which brings you to the portal’s home page.

Now, we’re going to explore the Create a Resource option. Click on Create a Resource. You’ll see a list of all the services available in Azure, organized by category.

Categories are like folders. For example, if you click on the Databases category, you’ll see all the database-related services available in Azure Cloud. You can then select and start creating a specific database from there.

If you’re not sure which category your resource belongs to, don’t worry. You can simply type the name of the resource you want to create in the search box.

In this case, we’re going to create a Resource Group. Technically, a Resource Group is not a software or a functional resource — it’s just a logical container. But without it, we cannot create or manage other resources.

Click Create Resource Group. As discussed earlier, it will automatically select the Subscription you’re working under, since this resource itself is a Resource Group — that’s why it doesn’t ask for a Resource Group name again.

Next, we must choose the Region, which determines where this Resource Group will physically reside. Usually, we select a region that is geographically closer to where the end users or the business operations are located. For example, if your business operates primarily in India, you might choose a region such as South India or Central India, depending on which one is closer to your operations.

Now, for the Resource Group name — we’re going to name it in a specific format. This particular Resource Group will be used for our Development Environment. The first three letters stand for Resource Group (RG), followed by a unique signature (for example, UDA), which I personally use for identification. You can create your own signature — don’t worry about it for now. I’ll provide instructions on this naming convention at the end of the video. The suffix DEV represents that this is a development environment.

Since the region closest to me is UK South, I’m selecting UK South as the region for this Resource Group.

Now that we’ve filled in all the required details, you’ll notice a few other tabs that provide additional configuration options. We’ll explore those later. For now, let’s focus only on the basic details required to create the Resource Group.

After entering the details, click on the Review + Create button. You’ll see the same option available in multiple places on the page. When you click this, Azure will perform a validation check to ensure that all the mandatory details have been filled correctly. It’s not creating the resource yet — just validating your input.

Once the validation passes successfully, click the Create button to create the actual Resource Group.

After clicking Create, you might notice the window disappears and returns to the Create Resource page. You may wonder if the resource was actually created. Don’t worry — even if you accidentally close the window during creation, you can always check the status of your operation.

Go to the top right corner of the screen — look for the bell icon, which represents Notifications. Every operation you perform in the portal is captured here.

You’ll see an entry showing the action you just performed, along with a confirmation that your Resource Group has been created successfully.

If you click on that notification, it will take you directly to the Resource Group you just created. Every resource you create comes with its own set of configuration options. As I mentioned earlier, we’ll explore each of these configurations step by step as we proceed, rather than covering them all at once.

Now, we’ve successfully created our first Resource Group. We still need to create the two resources required for our analytical project — Azure Data Factory and Azure Data Lake Storage Gen2 — and we’ll do that in the next lesson.

# **C) Setup Azure Data Factory**

In the previous lesson, we created our Resource Group using the Create Resource option inside the Azure Portal. We searched for the Resource Group service, entered all the required parameters, and successfully created our first resource. That was one method of creating resources in Azure. Now, in this lesson, we’ll explore another way to create resources — this time using the Global Search bar available at the top of the portal.

Before we begin creating the next resource, let’s understand the difference between the two search options available in the Azure Portal. The first search option, which appears under the Create a Resource page, will only display the Azure services that are available for you to create. It won’t show any of the resources that you have already created. On the other hand, the Global Search bar, which you can see at the very top of the portal, is more powerful. It shows both the resources you’ve already created as well as the Azure services that are available for you to create as new ones. In simple terms, if you’re looking for a specific resource that you’ve created or if you want to create a new one, you can do both from this global search option.

Let’s take an example to understand this better. Suppose we want to create a Data Factory resource. We can go to the global search bar and type “Data Factory.” You’ll notice that the Azure Portal displays the Data Factory service in the results. Click on it, and since we haven’t created any Data Factory yet, the screen will show an option to create one. Click on Create or Create Data Factory, and it will take you to the setup screen for this resource. As I mentioned earlier, there are multiple ways to create resources inside the Azure Portal, and this is another convenient way to do it.

Now, as soon as the Create Data Factory page opens, you’ll notice that the options here are slightly different from what we saw when creating the Resource Group. That’s because the configuration options depend on the type of resource you’re creating. However, there are a few parameters that are common across all Azure resources. These are the Subscription, the Resource Group, and the Region. These three are mandatory for creating any resource inside Azure.

Let’s go through the setup step by step. The Subscription will be automatically selected as your active one — in our case, the Free Trial Subscription. Next, we have the Resource Group. Since we already created a resource group in the previous lesson, we can select that one here. But if you want to create a new resource group, Azure gives you the flexibility to do that directly from this screen as well. Azure provides multiple ways to create the same type of resource, so it’s entirely up to you which method you prefer to use. After that, you need to provide a Name for your Data Factory. Then, select the Region where you want the Data Factory to be hosted. The region determines where your Data Factory will be physically deployed within Microsoft’s global data centers. In my case, the closest region is UK South, so I’m selecting that.

You’ll also notice that the version is already set to V2, as that’s the only one available at the moment. Some of the other configuration options can be left as they are for now; we’ll discuss those additional settings later in the course when they become relevant to specific requirements. Once you’ve entered all the required information, click on Review + Create. Azure will now validate the details you’ve provided to make sure everything is correct and complete. After the validation passes successfully, click Create, and Azure will begin provisioning your new Data Factory resource.

It’s important to note that the Create Data Factory page actually opens as a sub-window on top of your main Azure Home Page. This means that if you close this window by clicking the “X” icon on the top-right corner, you won’t lose anything — it will simply take you back to your main portal view. So, don’t worry if you accidentally close some windows while working in Azure. Every action you perform inside the portal — whether creating, updating, or deleting a resource — is automatically captured in the Notifications Panel, which is represented by the bell icon at the top-right corner of the page. This feature helps you track all your recent activities and confirm whether your resource creation was successful.

Once the Data Factory has been successfully created, you’ll receive a notification in the panel. You can click that notification to go directly to your new Data Factory. Alternatively, you can use the global search option again to find it. Simply type “Data Factory” in the global search bar, and you’ll see your newly created Data Factory listed under the “Resources” section.

Remember, this Data Factory is also contained within the Resource Group we created earlier. So, another way to access it is by searching for your Resource Group. Type “Resource Group” in the global search bar, open the group you created in the previous lesson, and you’ll see your Data Factory listed under it. This is how you can view all the resources that belong to a particular project or environment.

So far, we’ve learned two different ways to create resources in the Azure Portal. In the first method, we used the Create Resource option to create a Resource Group. In the second method, we used the Global Search bar to create a Data Factory. We’ve also learned how to track our actions using the notification panel and how to find existing resources that we’ve already created. Step by step, we’re getting more comfortable navigating the Azure Portal, understanding its layout, and managing multiple resource windows efficiently.

Now that we’ve successfully created our Azure Data Factory, we’re ready to move on to the next step. In the upcoming lesson, we’ll create our Data Lake Storage Gen2 account, which will serve as the second core component of our Landing Layer in the data analytics architecture. This will complete the first stage of our Azure environment setup.

# **D) Setup Azure Data Lake Storage Gen2**

We are now slowly getting familiar with the Azure Portal. By this point, you already know how to create resources using the top-left Create Resource option. And whenever you want to return to the home window, all you need to do is click the Home button at the top of the portal, which will take you back to the Azure home screen.

We’ve also learned how to create resources using the Global Search option. This search bar not only displays all the available Azure services that you can create, but it also shows the resources that you have already created. This means you can use the global search to either create a new resource or find an existing one quickly and easily.

Now, we’re going to look at the third option for creating resources inside the Azure Portal. You’ve already created your Resource Group, and all the resources you create are available inside that group. From within the Resource Group itself, you can create new resources directly. This is another convenient method provided by Azure for resource creation.

The last resource we need to complete our Landing Layer is the Azure Data Lake Storage Account. To create this, we’ll go inside the Resource Group we created earlier. Once inside, click the Create button. This will open the Search Marketplace window.

In the search box, type Storage Account. From the results, select Storage Account. This option allows us to create our Azure Data Lake Storage Gen2 account.

Now, as we begin filling out the required details, you’ll notice that Azure has started to automatically pick up some of the information from our previous actions. Earlier, it only auto-selected our Subscription. But now, since we’ve repeatedly used the same Resource Group, Azure automatically fills that in for us too. This makes the process faster and more intuitive over time.

Next, we need to provide a name for our Data Lake Storage Account. The name is a mandatory parameter. Following the naming convention, we’ll include “adls” for Azure Data Lake Storage, followed by our signature or initials, and finally the environment tag “dev” to indicate that it’s for our development environment.

After that, select your Region. Azure has already started remembering our preferences, so it will automatically pick the same region we used earlier — in my case, UK South. We’ll continue using the same region for consistency.

Then, we move on to the Performance and Redundancy options. For redundancy, select Locally Redundant Storage (LRS). This setting determines how your data is replicated across Azure data centers. Azure has multiple main data centers and their corresponding paired (secondary) data centers. In a redundant configuration, your data would be stored in both the main and paired centers to ensure high availability. However, since we are working with a free account, it’s better to use our resources efficiently and keep costs low. Therefore, we’ll go with the Locally Redundant Storage (LRS) option. I’ll explain the redundancy concept in more detail with examples in a later lesson.

Next, you’ll notice another important option called Hierarchical Namespace. This setting is critical when creating a Data Lake Storage Gen2 account. You must enable the Hierarchical Namespace because it allows the storage account to support a folder-based structure — meaning you can create multiple folders, subfolders, and a nested directory hierarchy within your Data Lake. Without enabling this option, you won’t be able to organize your data into folders and subfolders later on. We’ll revisit this concept again when we start creating and managing folders inside the Data Lake. But for now, make sure that the Hierarchical Namespace option is enabled before proceeding.

Leave all other settings as their default values. Once you’ve verified everything, click Review + Create to validate your configuration. After the validation passes successfully, click Create to begin the deployment of your Azure Data Lake Storage Gen2 account.

You’ll see a deployment in progress message appear on your screen. This indicates that Azure is provisioning your new storage account. You can keep this window open and monitor the deployment process here. Once the resource has been successfully created, it will be displayed in the notifications panel as well.

And that’s it — you’ve now created your Azure Data Lake Storage Gen2 account, completing the setup for your Landing Layer in our analytical project.

# **E) Summary**

We have now completed the initial setup and are ready to begin working with our Azure environment. So far, we logged into the portal.azure.com
 using the free Azure account that we created earlier. From there, we started creating the necessary resources for building the first layer of our data analytics project — the Landing Layer.

Upon logging in again, you’ll notice that the Azure portal displays the most recent resources you have accessed or created. Initially, we could only see the Azure subscription listed under the “Recent” section. But now, since we have successfully created both the Azure Data Factory and the Azure Data Lake Storage Account, they are also appearing under the recent resources list.

We explored multiple ways of creating resources in the Azure portal. You can use the “Create a Resource” option from the top-left corner, search for a service directly using the Global Search bar, or create a resource from within an existing resource group. Each method is flexible and can be used based on your preference. When you open any service, Azure often displays a sub-window. To return to the main page, you can use the Home button at any time.

As a best practice, when working with multiple resources, always try to open each service in a new browser tab rather than navigating back and forth in the same window. This helps prevent confusion and ensures a smoother workflow, especially since we’ll be developing our code directly within the browser environment.

In addition to the basic navigation, Azure provides some useful personalization options for better usability. For instance, if you frequently use Azure Data Factory (ADF), you can add it to your Favorites by clicking the star icon. Once you do this, it will appear under the “Favorite Services” list on the left panel and also on your homepage the next time you log in. Similarly, you can pin any resource to your custom dashboard using the pin icon beside it. This allows you to access your commonly used services directly from the dashboard view.

Personally, I prefer to rely on the “Home” section because it conveniently displays all the most recently used resources. However, it’s completely up to you — you can organize and personalize your workspace in the way that suits you best.

Before we move on to coding, there’s just one important action we need to perform. We’re going to define our Landing Layer clearly within the Data Lake environment. In this setup, the Data Factory will extract data from the web service and store it into the Azure Data Lake Storage. To store this data, we need to create a container inside our Data Lake Storage Account.

Consider the container as the root directory of your storage system — it’s where everything begins. Without creating a container, you won’t be able to store any files or folders. You can have multiple containers inside a single storage account, which is helpful when organizing data across different project layers. For now, we’ll create a container named “landing” to store all the raw source data retrieved from the web service.

Once the container is created, you can also add folders, subfolders, and files within it. This is where the Hierarchical Namespace feature comes into play. When we created the Data Lake Storage Account earlier, we enabled this option. If it wasn’t enabled, the option to create directories (folders) inside the container would not appear, and you would only be able to store flat files.

Now that our storage setup is ready and the container structure is in place, we are fully prepared to begin development. In the next lesson, we’ll start using Azure Data Factory to build and automate our data workflows for the Landing Layer.

# **III) Azure Data Factory Introduction**

# **A) Azure Data Factory Studio Overview**

We are particularly focusing on building the first layer in the data analytics project, which we call the landing layer. We have already created the two resources required to build this layer. Now, we are going to perform specific operations in this layer using these two resources. We will use Azure Data Factory and Azure Data Lake Storage to extract data from a web service and ingest it into the landing layer in our Data Analytics platform.

To start, log in to the Azure portal at portal.azure.com using your user ID, and you will arrive at the home page. The most recently created resources will be displayed since we created them last time. This is the first time we are opening Azure Data Factory. As a best practice, any service you open in the Azure portal should always open in a new tab to ensure that any work you are doing on the current page is not lost.

When you open Data Factory, options will appear on the left-hand side of the screen. Most of these options are common across all Azure resources, including Azure Data Lake Storage accounts. Common options include Overview, Access Control, Alerts, Metrics, and Networking. Depending on the type of resource, there may be additional options as well. These properties are helpful to set security on resources, defining who can access them and through which networks they are available. For example, you can choose whether a resource is accessible via a private or public endpoint. We will configure these security settings later in the course, but for now, we can leave them as they are.

Our main focus is to read data from a web service using Data Factory and ingest it into the Azure Data Lake Storage account. To accomplish this, we need to use the Data Factory Studio, which provides a separate interface for developing all Azure Data Factory code. When you open Data Factory Studio, a window will appear with some notifications about new features. You can close these notifications for now.

Within the studio, five different tabs are available. While the home tab is not essential for our current task, it provides a good opportunity to explain the logical definition of Azure Data Factory. Azure Data Factory allows you to ingest data from any source system into a data analytics platform. It also provides the capability to transform source data into any required format to extract useful information. Additionally, it can orchestrate the code you develop, ensuring it runs automatically on a daily basis to process new data from source systems. Based on these functionalities, Azure Data Factory can be defined as a data integration and orchestration service.

When you click any of the available options in the studio, it enables a template-based interface for developing Data Factory code. While this interface is useful, I prefer to develop code using the Author tab, which provides full control over the code development process. In the next lesson, we will explore the Author tab in detail and review all the components available in Azure Data Factory.

# **B) Azure Data Factory Pipeline Overview**

Just he explained basics about Activities, Parameters, Properties of Pipelines in Azure Data Factory (No Transcript in Video)

# **C) Copy Data Activity - Configure Source Dataset**

We have dragged the Copy Data activity from the Activities section into the pipeline pane. When you click on the Copy Data activity, the configuration settings associated with this activity appear. If you want to view the configuration settings of the pipeline itself, click somewhere outside the activity in the pipeline design page, and the settings will change to reflect the pipeline-specific configurations. To switch back to the activity-specific configuration settings, simply click on the activity again, and the settings for that specific activity will appear. Here, it is asking for a name, and we will give it a logical name, as we are trying to copy the source pricing data. If any specific settings are not explained, you can leave them as default for now.

Next, we move to the Source tab, which asks where our source data exists. According to our design, it exists as a CSV (comma-separated) file on an HTTP web server. Since Azure Data Factory does not inherently know the location of our source data, we create another component called a dataset. This is the third component we are learning in Azure Data Factory, after pipelines and activities. A dataset represents the actual data we are reading or writing, including its format and storage location.

When you start creating a new dataset, it asks where this dataset exists and in which data store it is stored. In our case, it exists on the HTTP website, so we select “HTTP” as the data store. The next option asks for the format of the source data, and since it is a comma-separated file, we select “Delimited Text.” After creating the dataset, we give it a proper logical name.

At this point, we need to configure one more component called a linked service. While the dataset specifies that the data exists on an HTTP web server in delimited file format, it does not specify how to connect to that web server. A linked service is used by Azure Data Factory to establish this connection. Since we do not have a linked service for this web server yet, we create a new one. Clicking “New” prompts for a name, which we give logically as “HTTP Source.” Based on the selected data store, we then provide configuration values, such as the base URL, which is the root URL of the web server.

In real project development, all this information will be provided to us. Here, we only provide the base URL and not the complete file name. This allows the linked service to read multiple files located in different folders within the web server. No specific authentication has been set, so the web server can be accessed without a username or password. We then test the connection, ensuring that our linked service is correctly established.

With the linked service and dataset created, we now configure the dataset-specific properties. These include specifying the relative URL, which indicates the path of the actual file on the web server. While the linked service connects to the base URL, the dataset specifies which specific file to read. The exact parameters required depend on the type of dataset—in our case, an HTTP dataset asks for the relative URL to access the specific file.

After configuring the source, the next step is to configure the sink, which represents the destination in Azure Data Factory. The sink configuration will be covered in the next lesson.

# **D) Copy Data Activity - Configure Sink Dataset**

We are working on creating an Azure Data Factory pipeline to ingest data from an HTTP web server into the Data Lake Storage landing layer. In the previous lesson, we configured the HTTP web server dataset and linked service. Now, we are going to configure the dataset for our sink.

Returning to our pipeline in the Copy Data activity, we have already configured the source. If we go to the sink, it asks for the sink dataset type. In Azure Data Factory, the sink represents the destination for the data. While our source was HTTP, the sink in this case is Azure Data Lake Storage Gen2, where we will store the file we read from the HTTP web server. We select Azure Data Lake Storage Gen2 as the data store, and the file type is again a delimited text file, matching the source format. We give a logical name to our dataset, ensuring there are no spaces in the name, as it will not accept them.

Next, we need to create a linked service for the sink, similar to how we created one for the HTTP web server. Since there are no existing linked services for this Data Lake Storage Gen2 dataset, we create a new one. We provide a logical name and select the subscription where our storage account exists. This is the same Data Lake Storage account we created to store all the source files received. After entering the details, we test the connection to ensure it successfully connects to the storage account and then click the Create button.

After creating the linked service, the next step is to specify the file path. Unlike the source dataset, which required a relative URL because it was on the HTTP web server, the sink dataset exists in the Data Lake Storage account. We choose “landing” as the folder path where the files will be stored. For the import schema, we select “None” for now, since we are simply moving files from source to sink without processing individual columns.

With this, the sink dataset has been successfully configured, completing the configuration for the Copy Data activity in our pipeline.

# **E) Debug Pipeline**

Now that we have configured both our source and sink datasets, we can open the source dataset from the pipeline interface to view the properties we have set. The source points to the relative URL, and the base URL is taken from the linked service. It is important to note that each dataset is associated with a linked service because the dataset represents the actual data, which may exist inside or outside Azure. For our source, we created a linked service to connect to the HTTP web server. For our sink, we created a linked service to connect to the Azure Data Lake Storage account we created inside Azure.

At this point, we have configured the necessary parameters to ingest data from the HTTP web server into the landing layer of our data analytics platform. There are additional settings available for the Copy Data activity, which we will cover in the appropriate scenarios later. For now, we can leave them as default. The next important step is to click “Publish All” to store the pipeline code permanently in the Azure Data Factory repository. If we do not publish and close the interface, all development work will be lost. It is good practice to keep clicking “Publish All” as you progress through pipeline development.

Once published, running the pipeline will read the file from the HTTP web server and store it in the Data Lake Storage Gen2 account. To verify, open the Azure Data Lake Storage account and navigate to the container. This is where the landing folder was created. Currently, there may be no files or folders, except for test folders like “labs” if any were created during previous exercises. When the pipeline runs, the source file from the HTTP web server will be copied to the Data Lake Storage account.

To run the pipeline, click the “Debug” button at the top of the pipeline interface. It is important to note that the user interface opens each component in a new tab—for example, opening the source dataset or sink dataset will create new tabs. When multiple pipelines exist, you will need to navigate through these tabs carefully to manage your work. Returning to the pipeline tab, clicking “Debug” brings up the pipeline configuration settings.

Under the Output tab, you can see the run logs for each activity included in the pipeline. The input section displays details of the configuration, such as the mechanism and file type used for reading the source file. The output section shows the Data Lake Storage destination, including the number of records read and written, as well as throughput details. These details provide a quick summary of the source and destination data, helping identify if any data was missed or corrupted. In later lessons, we will explore these logs in detail when performing performance tuning of pipelines.

After a successful pipeline run, refreshing the landing container in the Azure Data Lake Storage account will show that the source file has been copied from the web server. Even though we have not accessed the source file directly, Azure Data Factory reads it from the HTTP web server based on the relative URL specified in the source dataset configuration and loads it into the Data Lake Storage account. Files in the storage account can also be edited directly using the hidden edit button available when selecting a file.

As part of this lesson, we have learned about the various Azure Data Factory components and how to use them to build a pipeline. We will revisit these components in a presentation to reinforce the concepts. Additionally, we will develop another pipeline from scratch to gain further familiarity. These example pipelines are designed purely for learning and do not represent real-time project pipelines. Their purpose is to help you understand the different components involved in Azure Data Factory.

# **F) Recap Data Factory Components**

In the previous lesson, we designed an Azure Data Factory pipeline to ingest data from an HTTP web server into the first layer of our data analytics project, called the landing layer. To support this, we created an Azure Data Lake Storage Gen2 account. To design the pipeline, we set up several Azure Data Factory components.

The first component we created was a Linked Service. Although we created it while configuring the dataset, its main purpose is to establish connectivity between Azure Data Factory and the source or destination data store. We also created a separate linked service to connect to the Azure Data Lake Storage Gen2 account.

Inside the HTTP web server, we have our source file. At this point, Azure Data Factory does not inherently know the name or type of the file. To represent the source or destination data, we use the Azure Data Factory component called a dataset. While creating the dataset, we also created the linked service, which is often easier for first-time setups. Linked services can also be created separately and later mapped to a dataset, but in this case, we created both together.

We planned to store the CSV file in our landing container in the first layer of the data analytics project in delimited text format. Since Azure Data Factory does not know the format of the target data, we created a dataset to represent it as well. Thus, we have two datasets (source and sink) and two linked services (source and destination).

To move data between the source and destination, we used activities in Azure Data Factory. One of the key activities is the Copy Data activity. Within this activity, we specify the source dataset and the target dataset. During pipeline runtime, Azure Data Factory uses the information in the datasets and linked services to connect to the HTTP web server, read the specific source file, and copy it into the landing container in Azure Data Lake Storage. The linked services are responsible for connecting to the actual data stores during execution.

Now, if the source file exists in JSON format instead of CSV, and we want to copy this JSON file into the Data Lake Storage landing layer, we can use the same setup with the same source and destination services. However, some additional steps are required to handle the JSON format correctly in the pipeline. These steps will be covered while developing the pipeline.

# **G) Recap Copy Data Activity - Load JSON Data**

We are going to develop a second pipeline to load a JSON file that exists in a different folder on the HTTP web server. The base URL is the same as our previous pipeline, but the JSON file is located in the labs/lab2 folder instead of labs/lab1. Since the file format is JSON, we need to develop a pipeline to handle it, and we will first go through the theory before creating the actual pipeline.

Because the source file is in JSON format, we cannot reuse the dataset created in the previous step for the delimited text file. We need to create a new dataset in Azure Data Factory to represent this JSON source file. Similarly, we will store this JSON file in the same format in the Azure Data Lake Storage Gen2 account, which requires creating a new dataset for the target as well. However, we can reuse the same Copy Data activity as before. The linked services do not need to change because they are specific to the type of data store rather than the format of the data. One linked service per data store is sufficient to read different file formats. At runtime, Azure Data Factory will use the linked services to read from the source and write to the Data Lake Storage account.

Before starting, it is better to close any open pipelines to avoid confusion. To create the new pipeline, you can either right-click or click the “New Pipeline” button and give it a name. We then use the same Copy Data activity by dragging it into the pipeline design pane. Once added, the settings window changes to display the configuration options.

For the source, we need to create a new dataset because the JSON format is different from the previous CSV dataset. While you can create datasets directly from the pipeline, this time we will explore creating datasets separately and then mapping them in the pipeline. This helps in better organizing resources. The source dataset is located in the HTTP web server, and we give it a specific name, including the lab number for clarity (e.g., HTTP_JSON_Source_Pricing_Lab2). Existing resources and naming conventions can guide these details during hands-on practice.

When configuring the source dataset, the link service for the HTTP source is reused. The relative URL is updated to point to the JSON file in labs/lab2. We do not import the schema since this is a file-to-file copy without column-level transformations. After creating the source dataset, it appears under the datasets folder.

Next, we configure the sink dataset to store the JSON file in Azure Data Lake Storage. We select the data store as Azure Data Lake Storage, the format as JSON, and provide a logical name reflecting Lab2. We reuse the existing link service for the Data Lake Storage account and specify the landing folder as the destination. Once the sink dataset is configured, we map it in the pipeline, ensuring proper naming conventions to match the lab context.

With the pipeline configured, running it will move the JSON file from the HTTP web server into the landing layer of the Data Lake Storage account. The pipeline creates a subfolder lab2 in the landing container and writes the JSON file there. To execute the pipeline, click the “Debug” button. The output window displays pipeline properties, run logs, input configuration (reader/writer details), and output statistics, such as the number of records read and written. After the run completes, refreshing the landing container confirms that the JSON file has been successfully loaded into lab2.

For learning purposes, it is useful to note that not all activities in Azure Data Factory require datasets. Activities like “Set Variable” do not interact with datasets; they only set values used within the pipeline. In contrast, data movement and transformation occur primarily in the Copy Data and Data Flow activities, both of which require datasets. Depending on your requirements, you must identify which datasets are needed and which activity will perform the operation. Supporting activities assist the main data movement and transformation tasks, but do not perform data movement themselves.

# **H) Azure Data Factory Components Summary**

In this section, we got an introduction to Azure Data Factory (ADF) and started using it through the Azure Portal. When opening a Data Factory resource, there are several properties associated with it, although we did not explore all of them. The core development in ADF happens in the Data Factory Studio, where we create pipelines to perform specific operations. We primarily used the Author tab to develop these pipelines. Pipelines are logical arrangements of inbuilt activities available in ADF, allowing us to define workflows for data movement and transformation.

We specifically explored the Copy Data activity to move data from an HTTP web server into the landing area of our data analytics project. The first component we learned about was the pipeline, followed by the activity, which is a unit of work within the pipeline. While configuring activities, we created datasets, which represent the source or sink data. Datasets use linked services to connect to the actual data stores at runtime, enabling reading or writing of data.

We created two source datasets—one for a delimited text (CSV) file and another for a JSON file—and two corresponding sink datasets to store these files in Azure Data Lake Storage Gen2. Using these datasets, we developed two pipelines: one to load the CSV file and another to load the JSON file. The pipeline development process involves identifying the activity required for the operation, determining whether a dataset is needed, creating the dataset, choosing the data store, and configuring the linked service. These components can either be created while building the pipeline or independently before mapping them into the pipeline.

Besides the Author tab, we also explored other tabs in Data Factory Studio. The Monitor tab allows us to track pipeline and activity runs, including run logs, the number of records read and written, and throughput. This tab can display pipeline runs from up to 30 days or for a custom date range. The Manage tab is used to define reusable Data Factory components, such as linked services, datasets, and other objects. Linked services, for instance, can be created here and later mapped to datasets within pipelines.

The Home tab provides quick access to common tools, like ingesting data or initiating data flows. However, for proper development practices, we focused on the Author tab to create pipelines in a structured, developer-oriented approach. It’s important to note that the pipelines we developed in this section are not real-time project pipelines; they were designed to introduce the key ADF components—pipelines, activities, datasets, and linked services. Becoming familiar with these components prepares us to create actual ingestion pipelines for real-time projects, which will be covered in the next section.

# **IV) Data Ingestion Pipeline - HTTP Source**

# **A) Data Ingestion Pipeline Requirement**

We have started developing a Data Factory pipeline to ingest data from our existing source system, which resides on an HTTP web server, into the Azure Data Lake Storage account. In our data analytics project, we are moving these files into the first layer, called the Landing Layer. The pipelines we have developed so far are sufficient to understand the different components involved in Data Factory pipeline development, such as creating datasets, creating linked services, and using activities.

However, these pipelines are not robust enough to handle scenarios that occur in a real-time project. In real-time projects, our source system generates new files on a daily basis to capture changes in product pricing information and product arrival quantities. Let us quickly recap our source data and what we are capturing here. The source data includes the daily arrival quantities of products and the minimum and maximum prices set for those products in different markets across India. This information changes daily. To capture these changes, the source system generates a new set of files daily with different file names.

The pipelines we have developed so far point to a single source file. This approach is insufficient because it cannot automatically handle changing file names in the source system. To address this, we need to modify the pipelines using additional options available in Azure Data Factory so that they can automatically capture changes in source file names daily and copy the data into the Landing Layer.

Let us have a quick look at the pipelines we have developed in the Azure portal. We are all getting familiar with using this portal. If you are not logged in, go to portal.azure.com and log in using the free account we have set up. Once logged in, open Azure Data Factory in a new tab and launch Data Factory Studio to view the pipelines we have developed and to create new ones. This Data Factory Studio has a different interface, and we have explored most of the tabs available here. We no longer use the Home button and primarily use the Author button to develop pipelines and configure their associated components. To create a new pipeline, you can right-click, or if you want to open an existing pipeline, the pipeline design window will open along with the activities.

Activities are the backbone of Azure Data Factory. Any coding in Data Factory involves using and configuring these activities. In this pipeline design pattern, we are specifically working on the Copy Data activity in Lab One. By clicking on this activity, the configuration settings associated with it will open. We have configured our source and sink datasets to move a single file from the HTTP web server into the Landing Layer of our data analytics platform.

If you open the dataset and examine the connection information, it uses a linked service to connect to the HTTP web server. Inside this linked service, we configured the base URL to read a specific file from the web server. We set the relative URL property with a fixed value: labs/lab_one/product_wise_market_wise_daily_report_0101_2023.csv. This value is fixed and cannot pick up new files from the source because it is not dynamic. This is what we are going to change.

We will modify the relative URL property so that its value is derived during runtime. We will make this dynamic content, which means the pipeline will not point to any specific source file during development. Instead, during runtime, it will determine which file to read. For example, if the pipeline runs for January 1st, it will read the January 1st file, and if it runs for January 2nd, it will read the January 2nd file. This is what we will learn in this section. I will see you in the next lesson.

# **B) Pipeline Expression Builder & Dataset Parameters Overview**

We need to change the value of the relative URL setting from a static single file to one that is dynamically derived during runtime. To do this, if you click on the settings box in Azure Data Factory, it gives you the option to either set this value statically in the box or, at the bottom of the box, set the value using dynamic content. By selecting the option to add dynamic content, it will open the Pipeline Expression Builder. Here, you can construct an expression, and the output of that expression will replace the value for this setting.

The options available to build your expression depend on the component you are working on. For example, when working on a dataset, you can build expressions using the parameters and functions available in Azure Data Factory. These functions are always available when you open the dynamic content option on any component, along with the Pipeline Expression Builder. The additional option available based on the component we are working on is the parameter. The output of the expression will replace the value in this setting.

Now, what are parameters? Just like in any programming language such as Python or Java, if you want to pass a value to a program during runtime, you use parameters. Parameters are essentially logical references or pointers to a value. The actual value is decided at runtime, not during development. Parameters act as a reference to the value that will be supplied during runtime. You can create a new parameter here, give it a name, and choose the type of the parameter depending on the value it will hold. In our case, it will be a string. You can also provide a default value. If no value is supplied during runtime, the default value will be used for this setting.

Along with parameters, you can use built-in functions available in Azure Data Factory to derive the value for your configuration setting by building expressions. We will explore these functions with our actual requirement later. For now, we focus on how to use parameters—how to map a parameter to the connection settings and how to pass a value to that parameter during runtime.

We will see this in the next section. I do not want to change any of the existing datasets yet because keeping them intact allows you to incrementally understand the difference between using configuration settings without parameters and using parameterized settings. You will also see the flexibility gained by parameterizing configuration settings. I’ll see you in the next lesson for setting the parameter for our source dataset.

# **C) Creating & Configuring Dataset Parameters**

Transcript not available; Not giving Relative URL while creating dataset; Parameters can be created in "Connection", and as well as in "Parameters"

# **D) Pipeline Parameters Overview**

Transcript not available; Now it is like manually writing file name; We don't need any human intervention; We want it to load on its own; We want to Parametrize in Pipeline Level in "Pipeline Expression Builder"

# **E) Creating & Configuring Pipeline Parameters**

We created Dataset Parameters and later used at Pipeline Parameters

We are using parameterized source and sink datasets inside the pipeline. Since these datasets are in a parameterized state, the pipeline requires values to be passed to them. In the previous lesson, we tried to pass the source file as a static value, but this approach is not suitable for handling real-time scenarios. We are going to change the values passed from the pipeline to dynamic content. As soon as you click on the Dynamic Content option inside the pipeline, the same Pipeline Expression Builder used in the dataset opens, but now with additional options available at the pipeline level.

At the pipeline level, you can map values from a parameter or a system variable. Functions always appear in the Pipeline Expression Builder, regardless of where you open the dynamic content. The remaining options vary depending on the ADF component you are working on. You can also use variables at the pipeline level, including system variables, which we will explore later. For now, we focus on parameters. Parameters are logical pointers or references for values that you pass at runtime, either at the dataset level or pipeline level. During runtime, these parameters take the provided values and replace them wherever they are used.

Parameters at the pipeline level function similarly to those created at the dataset level. By clicking the plus button in the pipeline, you can create a new parameter and assign a value. Instead of using dataset-level parameters directly, we create pipeline-level parameters and pass their values to the dataset parameters at runtime. For example, for the dataset parameter relative URL, we create a corresponding pipeline parameter with the same naming convention and map it to the dataset parameter. This allows the dataset to dynamically receive values from the pipeline during execution.

To view pipeline parameters, click anywhere outside the activities in the pipeline design window. This will take you to the Parameters tab, which shows all configuration settings associated with the pipeline. Here, you can see the parameter we created to pass the value to the source dataset. Similarly, we create three parameters at the pipeline level to pass values to the sink dataset. We use a naming convention to differentiate pipeline parameters from dataset parameters by prefixing them with pipeline_.

Thus, there are two types of parameters in Azure Data Factory: dataset-level parameters and pipeline-level parameters. Dataset parameters are associated with dataset connections, and their values are replaced by the values passed from the pipeline. These values can either be hardcoded or parameterized at the pipeline level. In our case, we are parameterizing at the pipeline level and mapping the pipeline parameters to the dataset parameters. When we debug the pipeline, it becomes clear how pipeline parameters are mapped to dataset parameters and how the runtime values replace the dataset parameter values during execution.

For example, in our pipeline, the dataset parameter sync container name is mapped to the pipeline parameter container name. Similarly, the dataset parameter folder is mapped to the pipeline parameter folder name, and the dataset parameter file name is mapped to the pipeline parameter file name. The difference between the previous pipeline and the current one is that nothing is hardcoded anymore; all values are parameterized. The first level of parameterization occurs at the dataset, which is then used in the connection object. These datasets are then used in the pipeline. Pipeline parameters are created and mapped to dataset parameters for both the source and sink datasets.

Now, anywhere inside the pipeline, the values are not static. During debugging, the pipeline will use the values passed to the pipeline parameters. These values will replace the dataset parameters dynamically, allowing the pipeline to run using the runtime values. In the next lesson, we will debug the pipeline and pass values to these pipeline parameters to see it in action.

# **F) Debugging & Dynamically Passing Parameter Values**

Transcript not available; We just passed file names and storage location names during runtime at pipeline level and not at dataset level

# **G) Recap Dataset and Pipeline Parameters**

Understanding the usage of parameters in Azure Data Factory is the key to advancing your pipeline development skills. We have created parameters both at the dataset level and at the pipeline level. Let’s go through this once more to clearly understand what is happening.

We are trying to load data from an HTTP web server source system into the Landing Layer of our Data Lake Storage account. The source system generates new source files daily, with new file names each day. Therefore, we need to develop a pipeline that can automatically capture changes in source file names from the source system without any user intervention.

To achieve this, we created a parameter at the dataset level — specifically in the source dataset — to capture changes in the source file name. This parameter acts as a logical reference or pointer to a value that we pass at runtime. It does not point to any specific source file during development. We mapped this parameter to the connection object inside the same source dataset, making the dataset generic and not tied to any particular file.

Similarly, in the sink dataset, we created three parameters to capture the container name, the folder name, and the file name. All these parameters are driven by the source file name, since the source file comes from a specific folder and follows a particular naming convention. To capture both the folder and file name, we created two different parameters. The container name parameter is always set to point to the “landing” container in our Data Lake Storage account. Again, we created these parameters at the dataset level and mapped them to the dataset’s connection properties — first for the container name, then the folder name, and finally the file name. These make up our dataset-level parameters.

Until this point, we hadn’t used these datasets in the pipeline. Once we started using the source dataset in the Copy Data activity, Azure Data Factory asked for the parameter values defined at the dataset level. Inside the pipeline, we could have passed specific file names as static values, but that would defeat our goal of making the code fully generic. So, we created another set of parameters at the pipeline level to pass values to these dataset parameters.

These pipeline parameters are designed based on the list of parameters we created at the dataset level. To create them, we navigated to the pipeline parameters — which are not specific to any activity or dataset, but rather belong to the pipeline itself — and defined four parameters: one for the source dataset and three for the sink dataset. We then mapped these pipeline parameters to the dataset parameters inside the pipeline, ensuring that any value passed to the pipeline parameters would automatically flow down to the dataset parameters. The dataset parameter values, in turn, get replaced in the dataset connection properties, allowing the source and sink to dynamically read and write data based on the runtime values.

Now, our code is completely generic. It no longer points to any specific source or sink file. The files are determined dynamically at runtime. When we start the pipeline, it will ask for values for the pipeline parameters. Note that these are pipeline parameters, not dataset parameters, because datasets alone are not executable components — they must be used within a pipeline activity. Pipeline parameters act as root-level parameters and are used to pass values into dataset parameters.

Currently, we are loading two source files from the HTTP web server. For the first run, we pass the first source file path as the relative URL value. The container name remains fixed as “landing,” the sink folder name is derived from the source folder name, and the sink file name is also derived from the source file name. The main driver here is the source relative URL, as it changes daily. This allows the pipeline to read the new source file each day and load it into the landing container without any manual intervention.

When you pass these values during execution, they are replaced inside the pipeline parameters, which then replace the corresponding dataset parameter values. Those values, in turn, are used in the dataset connection properties. For example, when the source reads the product_wise_market_wise_daily_report_0101_2023.csv file, it loads it into the Landing container. In the next run, if you debug again and pass the 0102_2023 file, the same parameter replacement occurs — the new file name is dynamically passed through the parameters and loaded into the Landing container.

So far, this pipeline is highly reusable. We have built a solution that can dynamically load different source files on a daily basis. However, there is still one user intervention required: we have to manually provide the source file name for each run. In the next step, we will automate this part as well, so that the pipeline automatically retrieves these values at runtime and executes multiple runs automatically. We will make these changes in the next lesson.

# **H) Identify Static and Dynamic Parameter Values**

Transcript not available; We clicked on outside of Pipeline and gave "Default Parameters"; Splitted up Relative and Sink Path into 4 Parameters - Folder Name, File Name, File Date (Dynamic), File Type

# **I) Configure Static Pipeline Parameter Values**

Transcript not available; We have to try to concatenate all 4 parameters and pass it to Dataset Parameter; We will use concatenate using "Azure Functions"; We don't need to do any coding; We need to just press on individual Parameters and then it will concatenate

# **J) Dynamic Pipeline Expressions Using Pipeline Parameters & ADF Functions**

Transcript not available; We will use concatenate using "Azure Functions"; We don't need to do any coding; We need to just press on individual Parameters and then it will concatenate

# **K) Data factory DATETIME format overview & Error Handling in Ingestion Pipeline**

We need to find a proper way to automate the URL file date. Currently, the file names take values such as 01012023 and 01022023, representing the files for January 1st and January 2nd, respectively. However, if we continue passing these values manually, we end up running the pipeline twice — once for 01012023 and again for 01022023. This manual repetition is what we want to eliminate.

These date values can actually be derived from the Universal Date Time format. For example, instead of manually entering 01012023, we can represent dates in the universal format, which is much easier to automate inside Azure Data Factory (ADF). The universal date format follows a pattern where the year part comes first, followed by the month, day, time, and finally the timezone information (like GMT, GMT+1, GMT+6, etc.). Since dates are fundamental in almost every software system, ADF — like other platforms — can easily generate and handle date values in this universal format automatically.

So instead of passing a manually typed date like 01012023, I would like to pass the Universal Date Time format value as the file_date parameter in the pipeline. This approach can later be automated within ADF using dynamic expressions. For now, we will manually pass the Universal Date Time value as a parameter and run the pipeline to test it.

Once the new value is passed, we can run the pipeline. At this stage, it’s expected that the pipeline will fail — and that’s intentional. The idea is to debug the failure to understand what needs to be fixed for automation to work properly. So instead of passing the actual file date format (01012023), we’re passing the Universal Date Time format (something like 2023-01-01T00:00:00Z) because this is the format that can be easily generated and manipulated inside ADF. However, our source system currently stores files using the compact format (like 01012023), so there will be a mismatch.

After running the pipeline, as expected, it fails. To check what went wrong, we can click on the information icon next to the failed activity. This opens the detailed error message. It’s usually a good idea to expand this window fully since error details can be long and hard to read.

The error message shows that the HTTP request failed with client error status code 404 (Not Found). This means that the requested file does not exist in the source system. The error also provides a hint: “Please check your activity settings. If you configured base URL that includes a path, make sure it ends with a slash.” This confirms that the problem is not with connectivity but with the file name construction.

When we look at the full URL that ADF generated, we can see that it’s formed by concatenating the four parameter values we passed:

The first parameter (folder name): Labs/Lab3

The second parameter (file name prefix)

The third parameter (file date, in universal format)

The fourth parameter (file type, .csv)

By combining these values, the final URL becomes something like:

https://<base_url>/Labs/Lab3/<file_name>2023-01-01T00:00:00Z.csv

However, the source system does not have a file with that date format. Its files are named in the format 01012023.csv, not 2023-01-01T00:00:00Z.csv. Hence, the system throws a 404 Not Found error — because the file name we constructed does not exist in the source.

To fix this, we need to convert the Universal Date Time format into the specific file date format (ddMMyyyy) that matches the source file naming convention. Fortunately, Azure Data Factory allows us to perform such date transformations using expressions in the Pipeline Expression Builder. There, we can apply a date conversion function to dynamically transform the universal date format into the required format before concatenating it into the final URL.

In the next step, we will focus on how to convert the universal date format into the desired 01012023 format inside ADF, so that the pipeline can automatically generate the correct file names and load the appropriate files without any manual input.

# **L) Formatting DATETIME Values Using Advanced Expressions and Date Functions**

We have passed the source file date parameter in the ACM Universal Date Format, and we have used that universal date format parameter inside the source dataset relative URL. Here, we concatenated the folder name, file name, and file date. When running the pipeline previously, it replaced this file date value with the actual date value that we had passed. However, the source file name does not exist in this universal date format — instead, it exists in the “0101 2023” format. Therefore, we need to convert our pipeline parameter value, specifically this file date value, from the universal date format into this specific format.

That conversion can be done inside Azure Data Factory if you closely monitor it. We are trying to extend the complexity of developing the pipeline and configuring it specifically in the Pipeline Expression Builder. At first, we just mapped individual parameters to single dataset parameters. Then, we concatenated four parameters together and passed them as a single parameter to the source dataset relative URL. Now, we are going to apply a function specifically on one of the parameters in the pipeline to convert from the universal date format into the file-specific date format. So, we need to convert this one format into that format.

Probably, I will copy these values here so that we know what we are trying to achieve — what is our input and what is our expected output. We need to extract the month part first, then the date part next, and then the year part. We need to convert the format coming from the source into this new format. We don’t need to write any custom code for this — there are inbuilt functions available in Azure Data Factory. We just need to know how to use them and how to configure them, just like how we configured the concatenation function earlier.

This time, we are working with a date-specific function. You can look at the Date Functions group, and in fact, the first function there is formatDateTime(). This function will format an input date that comes in a proper date-time format into any other format that you would like to convert to. There are many inbuilt formats available, and I will provide the link for the various date formats in the resources section of the course. But for our specific case, we are particularly interested in the month part, the date part, and the year part of the pipeline parameter value coming in.

So, I am just adding some entries here so that you can clearly see where we are going to apply the function. We are going to apply the function on the relative URL file date. Click in front of that pipeline parameter and click the formatDateTime function. Whenever you click this specific function, it automatically comes with opening and closing parentheses together. Remove the closing parentheses temporarily, because we need to complete the function configuration first — we will reapply the closing bracket later.

From this input date format, I am interested in extracting the month values in digit format, the date values in digit format, and the year values in digit format as well. Once done, I will close my function configuration and remove the default values that we copied earlier. Now, the function is valid. It will convert the pipeline variable value from the Universal Date Format into our source file date–specific format.

We can use the same function in our sink as well because we are also using the pipeline file date parameter in the sink to form the output file name. So, go to the sink and click the file name again. This file date value can be replaced with the formatDateTime() function using the specific format we just applied.

Now, if we run this pipeline, it will read the 1st of January 2023 source file correctly. Because we are passing 1st of January 2023 as the universal date here, when we run the pipeline, it will be able to copy the file properly and put it into the landing layer without any errors.

If you come and refresh the “lab three” folder, you will notice that only the “0101 2023” file was modified today. The previous load of the 2nd of January file remains unchanged, but in this run, only the current file has been loaded. If you look closely, the formatDateTime() function we applied in both the source and sink is exactly the same — it’s the same expression, the same function, using the same pipeline parameter, and the same format.

However, since we used it twice, there’s repetition in the code. If you find yourself repeating anything in the pipeline configuration, it’s better to create a pipeline variable to store that function result so that it can be reused wherever needed. Repetition of the same function multiple times should be avoided. Therefore, we will move the formatDateTime() function into a pipeline variable, and then we can reuse it in both the source and the sink in the next section.

# **M) Configuring Pipeline Variables and SET VARIABLE Activity**

Instead of deriving the file date value separately in both the source and sink, I would like to derive it once and reuse it across both. To achieve that, Azure Data Factory (ADF) provides the flexibility of using variables. The key difference between parameters and variables is that parameter values are passed only once at the runtime of the pipeline, and these parameter values cannot be changed afterward. If you take a closer look at our setup, we have reused parameters inside the pipeline code, but we never tried to modify their values. However, with variables, we can change their values dynamically during the pipeline execution.

So, in our case, we need a variable that can read the data from the pipeline parameter (specifically, the relative URL file date) and convert it into the specific format required to read the source file. To create this variable, click outside any activities in the pipeline and go to the Pipeline Settings. In the settings panel, navigate to the Variables tab, which is the second tab. Here, you can create a new variable. Follow standard naming conventions — since this variable is going to modify the relative URL file date, I’m copying that pipeline parameter value here to logically relate it. You can provide a default value if needed, but the main advantage of a variable is that you can change its value inside the pipeline using an activity called Set Variable.

Now, we are expanding our pipeline skills. So far, we have focused mainly on the Copy Data activity, which is one of the most important activities in ADF. That’s why we’ve spent so much time learning it with multiple variations. But now, we’re going to learn about the Set Variable activity. Drag and drop the Set Variable activity into the pipeline and name it logically. Then, go to the Settings section. You will see the list of pipeline variables that you’ve already created. If you haven’t created a variable yet, you can also create a new one directly from this panel. As soon as you create it, it will appear under the pipeline variables section.

You’ll also notice an option called Pipeline Return Value, but we’ll discuss that later in the course. For now, let’s focus on how to set the value for this pipeline variable. Click on the variable value field — it will open the Dynamic Content window, the same one we used earlier for configuring expressions in the Copy Data activity. Here, we can directly convert the parameter using the formatDateTime() function. It’s a good practice to apply the conversion logic here itself. From the list of functions, choose formatDateTime(). The input value for this function will be the relative URL file date parameter, and we’ll format it such that it first takes the month part, then the date part, and finally the year part.

Now, we have successfully created the variable. We no longer need to derive the same value repeatedly inside the Copy Data activity for both source and sink. We can reuse this pipeline variable across all activities in our pipeline. To use it, we simply connect the output of the Set Variable activity to the input of the Copy Data activity. Then, inside the Copy Data activity, go to the Source tab. Instead of deriving the file date value from the file parameter, replace it with the pipeline variable — since it’s already deriving the same value, but now in a single reusable step.

If you observe carefully, when building expressions now, you have access to all available options such as parameters, variables, and even system variables, which we’ll learn about later. Along with those, you’ll always have the inbuilt functions available. This means the value we are using now is derived through a combination of a pipeline parameter and a pipeline variable together. Similarly, in the Sink, for the file name, instead of deriving the value again, we can directly use the pipeline variable value.

Now everything will work fine. Before testing, let’s go to the landing container and clear all existing files so that we can retest from scratch. When you debug the pipeline, even if you don’t pass any value manually, it will take the default value defined in the pipeline parameter. The pipeline should now read the “1st of January” file from the HTTP web server and load it into the landing container. Once the run completes successfully, you will see that the specific file has been copied properly.

If you look closely at the pipeline Run Details, you’ll notice the additional Set Variable activity we just added appearing there. You can view its input, which is the pipeline parameter value, and its output, which is the converted date format. The Copy Data activity also runs successfully. Now, if you go to the Landing → Labs → Lab3 folder and refresh it, you will see that the “1st of January” file has been copied.

With this setup, we’ve successfully simplified our pipeline. However, there’s still one small part left to improve. Currently, the date value is still hardcoded — meaning, whenever we want to load the “2nd of January” file, we have to manually enter that date while debugging. This introduces one layer of user intervention that we still need to eliminate. Our next goal is to find a way to automatically pass these date values.

To achieve that, we’ll use an ADF component called a Trigger. We haven’t learned about triggers yet, but we’ll start with an overview in the next section. Once we complete that part, we won’t need to manually run the pipeline anymore. The pipeline will automatically trigger itself — it will pass the “1st of January” value for the first run, the “2nd of January” value for the second run, and so on. As a result, it will automatically copy both files into the landing container in the Azure Data Lake Storage account. We’ll see how to implement this in the next lesson.

# **N) ADF Triggers Overview**

We have almost automated all of the pipeline parameter values except this relative URL file date because this is changing for each run. A new date value needs to come, so we need to find a way to do that one. We have got two file date parameters — one is source and another one is sync. We can delete the sync file date value because, from this date value, we have derived the variable value. This variable value is the one referenced in the source and target. So, we can remove the sync file date parameter in the pipeline. This is the advantage of using a variable — it reduces unnecessary additional parameterization. We can derive it once and reuse it multiple times. So, we will delete the sync file date pipeline parameter.

Now, the only parameter we need to automate is passing the value for this relative URL file date value. Otherwise, when loading multiple files, you need to debug each time and pass that value manually to load the new set of source files. We need to automate that. What we are going to do is learn a new Azure Data Factory component called a trigger. A trigger is a component at the top of the pipeline that automatically runs the pipeline depending on the schedule that we set inside it. Once the trigger is set up, we don’t need to click the debug button manually. After setting up the trigger, it automatically runs the pipeline and also automatically passes values to all of these pipeline parameter values, including the source file date value.

Let us start by creating a new trigger. The trigger option now is just running the pipeline via a single trigger. It won’t run at regular intervals, so we’ll explore creating a new trigger, and then we will come back later and see the trigger. At this moment, it doesn’t have any major significance — it’s equivalent to debug, but you can see how it runs in real time after setting up the trigger. So, if you click the New/Edit button, you can choose New Trigger. We would like to create one because we don’t have any trigger created yet. It will say something like TRG_Daily_Pricing_Load — we’ll give it a reasonable name for the trigger.

There are four types of triggers available. The first one is Schedule Trigger, the next one is Tumbling Window Trigger, and we will see the difference between both of them because it’s a little relevant to this specific scenario. We will see the Storage Events and Custom Events triggers later in the course, so for now, we’ll focus on the Schedule Trigger. The Schedule Trigger is one of the basic types of ADF triggers. You can start the job from the start date that we set. For example, if the current time is 9:24 PM, you cannot set the start date in the past. You can’t set something before this 24 minutes — it needs to be in the current date or a future date.

For example, I can start to run this pipeline from tonight at 10:00 PM. Now, which time zone is this time related to? Because we are in the UK, it takes the default global time zone, which is UTC+0. There are different time zones available, and you can choose the one that fits your need. For me, UTC+0 is optimal, so I’ll choose that. Next is Recurrence — how frequently the pipeline needs to run repeatedly from this start date. For instance, if you set it to every 15 minutes, it will run at 10:00, 10:15, 10:30, 10:45, and so on. In our case, we don’t need it to run every few minutes. It needs to run once every day, so we can set it to one day. If within that day you want to execute at specific hours or minutes, that can also be set here.

If you want to specify an end date, you can do that as well. This means that after the specified date, the trigger won’t work — it won’t automatically run the pipeline anymore. However, we are not going to use the Schedule Trigger for our scenario because our first file date starts from 1st January 2023, which means we need to go back almost a year. The Schedule Trigger cannot run on past dates, so we need to use the next type of trigger — the Tumbling Window Trigger.

Before moving on, I would also like to mention that the Schedule Trigger will kick off at the specified time every day starting from the configured date if we set it that way. But we are not going to use the Schedule Trigger now — we will use it later in the course. For this specific example, we are going to use the Tumbling Window Trigger in our scenario. So, in the next lesson, we will go through the overview of the Tumbling Window Trigger and then create one for our pipeline.

# **O) Create & Configure Tumbling Window Trigger**

Let’s explore the properties of the Tumbling Window Trigger. First, I am going to rename this trigger to TumblingWindow_Trigger_DailyPricingLoad. The main difference between a Schedule Trigger and a Tumbling Window Trigger is in how they determine when to run. A Schedule Trigger starts running at the specific start time you set and repeats at the interval you define. For example, if the start time is 10:00 PM today, the next run will be tomorrow at 10:00 PM, and so on.

The Tumbling Window Trigger, on the other hand, calculates runs based on the periodic difference between the start date and the recurrence interval you define. It doesn’t start immediately at the start time; instead, it waits until the recurrence period ends before executing. For instance, if the start date is 10:00 and the recurrence is every 15 minutes, the trigger will execute at 10:15 — not at 10:00. Another advantage of the Tumbling Window Trigger is that it allows starting from historical dates, which is exactly what we need because we want to load files starting from 1st January 2023. We will set the start date to 1st January 2023, 00:00:00, with a recurrence of 24 hours since our source files arrive daily.

We also need to specify the end date; otherwise, the trigger will continue to run indefinitely. For this example, we only have two files to load, so we will set the end date accordingly. One important point to note is that the first run of the Tumbling Window Trigger happens at the end of the first recurrence window. That means the file for 1st January will only be loaded at 2nd January, 12:00 AM, and the 2nd January file will be loaded on 3rd January, 12:00 AM. This behavior is inherent to how the Tumbling Window Trigger works — it waits for the completion of the recurrence period before kicking off the pipeline.

There are some advanced properties in the trigger configuration. For example, Delay allows you to delay the start of the trigger, which can be useful if multiple triggers are dependent on each other. Maximum Concurrency defines how many pipeline runs can execute simultaneously. For example, if your data supports it, you could process 50 days’ worth of files in one run by setting maximum concurrency to 50. For now, we will set it to 1 since this is the first time using this trigger.

Another important property is the Retry Policy. If the Copy Data activity fails (for instance, if the HTTP web server is temporarily unavailable), the pipeline can automatically retry execution based on the retry count and retry interval you configure. For example, with a retry count of 1 and a retry interval of 30 seconds, the pipeline will wait 30 seconds and automatically retry the failed run.

Once we have set all the basic properties, clicking OK will prompt us to pass values for all pipeline parameters. Most of these parameter values we already know, except the Relative URL File Date, which changes for each run. For that, we will use the date value associated with this trigger, which allows the pipeline to automatically pick the correct date for each run. In the next lesson, we will start setting the values for each pipeline parameter and configure the trigger to automatically handle the file date.

# **P) Passing Tumbling Window Trigger System Variables To Pipeline Parameters**

When setting up the trigger, it prompts for values for all the pipeline parameters. This is a one-time setup—once configured, you don’t need to pass these values again for subsequent runs. The trigger will automatically use these values every time the pipeline runs until the trigger’s end date.

For most parameters, the values are straightforward. For example, the sync container name can be set to landing, which is the container in the Data Lake Storage where the files will be copied. The folder name is labs/lab three, and the file name format remains consistent across runs. The file type for both source and sink is .csv. None of these values change per run.

The only value that changes for each run is the relative URL file date. The Tumbling Window Trigger has inbuilt properties—window start time and window end time—that help automate this. These properties track the start and end of each recurrence period. For example, if the trigger runs every 24 hours and the first run starts at 2:00 AM, the first run’s window start and end times are automatically set. For the next run, the window start and end times automatically increment by 24 hours.

This makes the window start time an ideal candidate for the URL file date because it automatically reflects the correct date for each run. To reference this value in the pipeline, you use the syntax:

@trigger().outputs.windowStartTime

This inbuilt property of the trigger automatically passes the correct date to the pipeline, eliminating the need to manually input 1st January, 2nd January, or any subsequent dates. Once this is set, publishing the trigger enables it to run the pipeline automatically according to the schedule.

Before the pipeline runs, it’s a good practice to clear the target folder (labs/lab three) so you can clearly observe the pipeline’s effect. After publishing, you can view or edit the trigger settings anytime. Changes, such as updating the end date, are applied automatically, and the trigger continues from where it left off. This makes the Tumbling Window Trigger a powerful component in Azure Data Factory for automating time-dependent data processing without manual intervention.

In the next lesson, we will start the pipeline and observe it executing automatically with the trigger passing the dynamic file date.

# **Q) Monitor Automated Pipeline Runs Via Tumbling Window Trigger**

As soon as you click Publish, all the trigger changes are applied to the pipeline. The trigger automatically starts running the pipeline. However, unlike debug runs, you won’t see the output in the usual output window. To monitor the triggered runs, you need to switch over to the Monitor tab and check the Trigger Runs section. Once published, the trigger will start the pipeline within a few seconds.

After publishing, if you go to Monitor, you can see that the first run has already started. Looking at the parameter values, you’ll notice that the relative URL file date is automatically passed as 0101 2023, which is exactly what we needed. The remaining parameters are mostly fixed, so you don’t have to worry about them for each run. Once the first run completes, you can check the landing container in the Data Lake Storage, and you’ll see that the first file has been successfully loaded. The process is very fast, and subsequent runs automatically pick up the next date values—for instance, the second run passed 0102 2023 automatically.

By using this approach, you can automate the loading of a year’s worth of data just by adjusting the end date in the trigger. The trigger is a reusable ADF component, similar to a linked service, and can be used across multiple pipelines. You can also create or edit triggers under the Manage tab. In this case, we created the trigger directly from the pipeline, and once published, it appears immediately and starts running according to the schedule.

With this setup, the pipeline is fully automated—no user intervention is required. It automatically identifies changes in the source file names (within the configured naming convention) and copies the files into the landing container in the Data Lake Storage account. This achieves exactly what we intended: seamless, automated file ingestion.

The only limitation is that this pipeline currently works only for files with the specific name pattern configured in the trigger. If additional files with different names exist on the HTTP web server, they won’t be picked up automatically because the trigger is fixed to a specific naming convention. In the next section, we will explore how to handle multiple file types and dynamic file names in the HTTP web server while maintaining full automation without user intervention.

# **V) Metadata Driven Data Ingestion Pipeline - HTTP Source**

# **A) Metadata Driven Ingestion Pipeline Overview**

A quick recap of what we have done: we created a pipeline that can automatically pick up changes in source file names from the HTTP web server and copy them into the landing container in our Data Lake storage account. We first parameterized our source dataset and sink dataset to make the source connection values dynamic. Then, we created pipeline parameters to map these values to the datasets and set parameters on top of that.

To automate the run, we included a tumbling window trigger. While setting this trigger in the pipeline, the trigger asks for values for each of the pipeline parameters. Most of the values are static and do not change for each run, such as the source file name. The only changing part is the file date value, so we are using one of the trigger window properties called window start time, which automatically updates for each run of the pipeline. We passed this property and used the Pipeline Expression Builder with the pipeline parameters to form the necessary source and sink connection values. These outputs were then mapped into the dataset parameters in the Copy Data activity.

As a result, without any user intervention, the pipeline can start loading the source files with changing date values on a daily basis, and it has successfully loaded the data. However, the only constraint in this pipeline is that it will only load source files starting with a specific string value. In real-time projects, the source system often has more than one type of source file, which this pipeline cannot handle.

In our case, we have two files capturing Indian pricing information for products. Additionally, there are two more files capturing international pricing information. These files have slightly different formats and different names, capturing product prices, countries, months, and date values. We need to bring these additional files along with the Indian pricing files, but the current pipeline cannot handle this scenario.

To address this, we need to move all pipeline parameters—except the relative URL and file date—outside of Azure Data Factory (ADF). By “outside ADF,” we mean storing these parameter values in a plain text file, which will then drive the pipeline. Pipelines designed in this way are called metadata-driven pipelines.

Before developing a metadata-driven pipeline, it’s important to understand what metadata is. For example, consider a product pricing file. The actual data in the file is the pricing information, while the file name, folder name where the file is stored on the HTTP web server, and file type are all metadata. Metadata is essentially data about data. To read or write the actual data, you need information about the file holding that data, such as its name, folder, and last modified date.

In fact, in our current pipeline, all the configuration values we have used are metadata. For instance, the landing container name in the Data Lake storage account does not hold actual data but serves as a reference for where the data will be stored. The source files we are reading from the HTTP web server are also metadata inside the landing container. We created two layers of folders, Labs and Lab3; these folders hold the actual data but are themselves metadata. Similarly, the file name holding the actual data is metadata. In short, metadata acts as a pointer for processing any data.

In real-time scenarios, multiple source files may arrive, sometimes in different formats. Therefore, to handle all these variations, we need to develop a metadata-driven pipeline. This requires moving all pipeline parameters outside ADF, storing them in a file, and learning how to pass these values from the external file into the ADF pipeline. We will cover the creation, formatting, and integration of these external parameters in the next lesson.

# **B) Metadata Driven Ingestion Pipeline Requirement**

We need to move all of the parameters that capture the metadata of the source and sink file names, except for the date value. The date value can be managed within the pipeline itself. Currently, the two types of source files we need to handle are: one starting with pw_mw_doctor and the other starting with global_pricing. All other parameters remain the same.

You might ask why we can’t just create one more pipeline parameter, for example, relativeURLFileName_global, and store the source file name format like global_pricing. The issue is that the Copy Data activity source in the pipeline points to a single source file name. The file name is formed based on the file name, file date, and file type. You cannot pass two different file name parameters into a single Copy Data activity.

Technically, it is possible to create another Copy Data activity and point it to the second file name. In this way, you could connect multiple Copy Data activities in the same pipeline, using one for pw_mw_doctor and the other for global_pricing. While this approach works, it is not elegant. For example, if a third file type is added in the future, you would need to create yet another Copy Data activity. This approach does not scale and is not a proper solution for handling multiple source file names.

The solution is to develop a metadata-driven pipeline. To illustrate the improvement, we will create a clone of the current pipeline without saving any recent changes. This clone will allow us to see how moving the parameters outside the pipeline simplifies handling multiple file names. We will call this cloned version the M3B pipeline. It still uses the same source and sink datasets created for Lab 3. The only change will be in how parameter values are passed to the pipeline.

As discussed, the metadata of the actual data files includes the source and sink file names. We will move all parameters except the file date outside the pipeline. We will start with the relative URL file name and sync file name parameters. By moving these parameters into a metadata file, the pipeline will be able to handle multiple source files with different starting names. The remaining parameters, which do not change between these two file types, will stay inside the pipeline for now.

Next, we will create the metadata file for these two file name parameters, read the metadata file inside the pipeline, and pass the values to the source and sink datasets. Once this is working, we can gradually move the remaining parameters outside the pipeline. This step-by-step approach makes it easier to understand and implement a fully metadata-driven pipeline. In the next lesson, we will start by deleting these two file name parameters and creating the metadata file for them.

# **C) Create Metadata File**

We are now going to move the relative URL file name and sync file name parameters outside of ADF. For the time being, I am creating these two parameter values in a separate file, which will serve as our metadata file. Once this file is ready, we can use it to provide the values to the pipeline. First, I deleted these two parameters from the new pipeline. If required, we can still refer back to the original Lab 3 pipeline. After deleting these parameters, the source and sink mapping becomes invalid because the parameters are no longer available. For now, we will focus entirely on creating the metadata file, and later we will fix the pipeline to read the specific values from it.

We have two different types of files that need to be loaded into the Labs/Lab3 folder. One type starts with pw_mw_Doctor and the other starts with global_pricing. All other values for the pipeline have already been derived and do not need changes. The goal now is to handle the variation in the file names. For example, in one pipeline run, we need to pass the value for the pw_mw_Doctor file, and in another run, we need to pass the value for the global_pricing file. The sync file name will have corresponding values.

To achieve this, we will create a JSON file to store these two different types of file names in a structured format. The JSON file will use an array of documents, where each document represents a file type. Each element inside the array is a key-value pair. For example, relativeURLFileName is a key, and its value is the file name, enclosed in double quotes because it is a string. Similarly, the syncFileName is another key, with its value also enclosed in double quotes.

The first document in the JSON file will represent the pw_mw_Doctor file. The second document will represent the global_pricing file. Each document is separated by a comma in the array. While there are other ways to store metadata—such as CSV files or databases—the JSON format is popular because it is easy to structure and read inside a data pipeline.

Once the JSON metadata file is created with two documents, it is stored locally on my machine. The next step is to read this file inside ADF, since the file name parameters were removed from the pipeline parameter list. This approach allows us to handle multiple file types dynamically via the metadata file instead of manually updating pipeline parameters. In the next lesson, we will see how to read this JSON file inside ADF and pass the values to the source and sink datasets.

# **D) Upload Metadata File and LOOKUP Activity Overview**

We have created our metadata file to store the different source file names existing on the HTTP web server. The next step is to read this file inside Azure Data Factory (ADF) and extract the values. These values will replace the pipeline parameters that previously held the file name.

Currently, ADF can read from data stores using linked services, which establish connectivity to any source or sink. We have created two linked services: one pointing to the HTTP web server, which we do not control (in fact, we never log in), and another pointing to our Data Lake storage account, which we do control. The linked service to the HTTP server allows us to bring files from the web server into our landing container. The linked service to the Data Lake provides full control over folders and files, allowing us to develop our data analytical platform.

The metadata file we created is not actual data; it only contains the source file names from the HTTP web server. Therefore, it should not be stored in the landing container, which contains all the source data files. Instead, we will create a separate container called ADF Metadata in our Data Lake storage account. We then upload the JSON metadata file from our local machine into this container. This allows ADF to read the metadata file directly from the Data Lake.

Once the metadata file is uploaded, we need an activity inside ADF that can read this file. Unlike the Copy Data activity, which simultaneously reads from a source and writes to a sink, we need an activity that can purely read data without writing. For this purpose, we use the Lookup activity. The Lookup activity reads data from a source file and makes it available within the pipeline.

To configure the Lookup activity, we must first create a dataset pointing to the metadata JSON file in the ADF Metadata container. None of the datasets we created so far (pointing to the HTTP web server source or the Data Lake sink) reference this new metadata file. After creating this dataset, we can configure it in the Lookup activity. This allows the pipeline to read the actual source file name values from the JSON metadata file and later use them in the Copy Data activity for the source and sink.

In the next lesson, we will cover configuring the dataset for the Lookup activity and using the values read from the metadata file inside the Copy Data activity to dynamically read the actual source files.

# **E) Configure LOOKUP Activity - Read Metadata File**

We have created a Lookup activity to read the metadata file that we uploaded into the Data Lake Storage account. There are a few limitations to be aware of when using the Lookup activity. This activity is not meant for heavy data processing; it is a support activity used to read small datasets. The maximum size for a dataset should not exceed 4 MB, and if there are more than 5000 rows, the activity will process them in batches of 5000 rows. The key limitation to keep in mind is the 4 MB size.

In our case, the metadata file is very small, only about 179 bytes, which is far below the 4 MB limit, so using the Lookup activity is perfectly fine. The next step is to create a dataset to read the metadata file. Since we do not yet have a dataset for this, we will create one. Our source data is in Data Lake Storage Gen2 and in JSON format. We will name the dataset dataset_ADLS_Json_Pricing_MetadataFiles_Lab3. It’s good practice to include the lab reference in the dataset name, as all datasets related to Lab 3, Lab 3A, or 3B will point to Lab 3.

We already have a linked service to connect to the Data Lake storage account. While browsing, we will not use the landing container. Instead, we select the ADF Metadata container where we uploaded the metadata file and choose the file. At this point, we do not need to parameterize the dataset. If new file names come into the source system, we can simply add another entry to the JSON file without creating a new dataset. Therefore, we avoid parameterizing the dataset now, though we may consider it during deployment if necessary.

After creating the dataset, you can preview the data to ensure the JSON metadata file is being read correctly. Once verified, these values can be used within the pipeline to replace the pipeline parameters that previously held the file name. Before using the lookup output in the Copy Data activity, we will run the Lookup activity separately to observe its output. This is significant because it is the first time we are using the output of one activity as input to another activity in the pipeline.

To test this, I connected the Lookup activity to a Set Variable activity temporarily. In ADF, the red circle button allows us to run the pipeline up to a specific activity. We can run it only until the Lookup activity to check the output without executing subsequent steps. Observing the output of the Lookup activity is crucial, as these values will later be mapped into the source and sink datasets of the Copy Data activity. The actual use of the Lookup output in the Copy Data activity will be covered in the next lesson.

# **F) Configure LOOKUP Activity Settings & Read Metadata File Values as Array**

Let's debug the pipeline to see how the Lookup activity is running. At this point, the pipeline still contains all the pipeline parameter values, which is fine because none of the Copy Data activities will execute during this debug run. By leaving the parameters at their default values and enabling the debug option, we can observe the output of the Lookup activity.

When the pipeline runs, we can examine the input of the Lookup activity to see which source data and source file it is configured to read. However, our main interest is in the output of the Lookup activity. We can copy this output into a notebook or a text editor to review the values. Initially, the Lookup activity only reads the first row of the JSON file. This is because the default setting in the Lookup activity is “First row only”, which is checked by default. Since our metadata file contains two rows (two source file names), we need to uncheck this option to ensure that the activity reads all data.

After unchecking “First row only” and running a quick debug, the Lookup activity reads both source file names correctly. The output shows a value array, which contains two elements: the first element corresponds to the pw_mw_Doctor file name, and the second element corresponds to the global_pricing file name. This array structure is crucial because it is a complex data type in ADF.

Previously, variables we used were simple data types, such as a single string or integer. However, the output of the Lookup activity is an array, and each element in the array has a key-value pair. We cannot directly map this array output into a Copy Data activity because the Copy Data activity expects a simple data type, not an array.

To use these values, we need to replicate a programming-style loop in ADF. We would iterate over the array, assign the key-value pairs to variables, and then process each element individually. This approach allows us to dynamically use both source file names from the metadata file in the Copy Data activity.

To prepare for this, I plan to rearrange the pipeline activities. The Set Variable activity should run first because it only executes once. If we connect the Lookup activity output directly to the Copy Data activity, the source shows the value array, which cannot be directly used. Attempting to map the array to a single value will cause the pipeline to fail, generating an error. In the next lesson, we will run the pipeline with this mapping to observe the error and then discuss how to properly handle the array output from the Lookup activity.

# **G) Configure FOR EACH Activity to Loop Through LOOKUP Output Value Array**

We tried to map the output of the Lookup activity, which is an array value, directly into the file name property of the Copy Data activity. When we debugged the pipeline, it failed as expected because the Copy Data activity cannot accept an array as a value—it expects a single string.

Looking at the error details, the pipeline was attempting to concatenate the folder path (Labs/Lab3) with the entire array value, treating it as a file path. Naturally, this failed because the source system only contains individual file names, not the entire array. What we need is to extract only the relative URL file name from the first element of the array, rather than passing the entire array.

To achieve this, we need to loop through the output of the Lookup activity and process each element individually. In ADF, we use the For Each activity for this purpose. Until now, we were mostly working with Move and Transform activities, but now we are exploring activities under Iterations and Conditions, which allow us to implement loops.

The input of the For Each activity will be the value array from the Lookup activity. Inside the loop, we can reference individual columns from each element in the array. This is done using the Pipeline Expression Builder, which now supports activity outputs in addition to parameters, system variables, and other functions.

We start by passing the lookup output.value array into the For Each activity. We can give the loop a descriptive name, such as IterateSourceFileNames. In the settings of the For Each activity, the main mandatory property is the Items, which defines the collection to iterate over. By referencing the value array from the Lookup output, the loop will process each element sequentially. For the first iteration, it will take the first element, and for the second iteration, it will take the second element. Once all elements are processed, the loop exits automatically.

In the next lesson, we will see how to use the output of the For Each activity as input to the Copy Data activity, enabling the pipeline to dynamically read each source file from the metadata.

# **H) Configure FOREACH Activity To Pass Metadata Values to Dataset Parameters**

We configured the For Each activity to take the Lookup output array as input using the Pipeline Expression Builder. All previous activity outputs are available in the builder, and we are specifically interested in the value array, as it contains the file names we need to map in the Copy Data activity.

Inside the For Each activity, any activity that needs to run as part of the loop must be placed in its sub-window. In our case, the Copy Data activity, which reads the source files and copies them into the landing container in the Data Lake storage account, needs to be inside this sub-window. To do this, we cut the Copy Data activity from the main pipeline and paste it inside the For Each activity’s sub-window. You can access this sub-window either by clicking the edit button inside the For Each activity or by editing through the activity section.

Now, for the first run of the loop, the For Each activity will take the first element from the array. We map the relative URL file name from the item output to the source dataset parameter. Instead of directly using the Lookup output, we now reference it as item.relativeURLFileName. This allows each iteration to pick the correct file name from the array. Similarly, for the sync dataset parameter, we use item.syncFileName to reference the corresponding value from the current item in the loop.

To summarize the setup: the Lookup activity reads the metadata JSON file, producing an array of two items. Since we cannot map the array directly into the Copy Data activity, we use the For Each activity to iterate over each item. Inside the loop, the Copy Data activity references the individual key-value pairs from the JSON file using the item object. The remaining pipeline parameters remain unchanged and are still used as before; only the file name values are now dynamically fetched from the metadata file.

Regarding execution, if the sequential option is checked in the For Each activity, the loop will run one iteration at a time. If unchecked, it will run both iterations in parallel, effectively executing two instances of the Copy Data activity simultaneously. For the time being, sequential execution is enabled to observe the process step by step.

At this stage, the pipeline does not yet include a trigger. The date parameter is still hardcoded, for example, 2023-01-01. During the run, the pipeline will copy both the local pricing data and the global pricing data into the landing folder, without requiring manual entry of the file names. The date parameter can later be automated using a trigger. In the next lesson, we will run the pipeline fully and observe the results in the landing container.

# **I) Debugging Metadata Driven Ingestion Pipeline & Error Handling**

Let's debug the pipeline and pass the default values to the pipeline parameters. Please note that the relative URL file date is set to 1st January 2023. Upon a successful run, the pipeline is expected to copy the two different source files corresponding to this date.

We start the pipeline and configure the For Each activity to run the files sequentially. This ensures that only one Copy Data activity runs at a time. The first iteration of the loop loads the first file from the Lookup activity output, and once that is complete, the second Copy Data activity runs for the second file. As expected, the first file is processed successfully, and the second file initially fails. This is useful because it allows us to examine the error message and understand the root cause.

Upon inspection, the errors occur while reading data from the HTTP web server. Looking closely at the request URL, it becomes clear that the issue is with the file naming in the metadata file. Specifically, the original source file names include an underscore after global_pricing, but this underscore was missing in the metadata JSON file. This is a simple error, but it prevented the Copy Data activity from finding the correct source file.

The beauty of this metadata-driven approach is that fixing such errors is straightforward. We can directly edit the metadata file stored in the ADF metadata container in the Data Lake storage account. Simply adding the missing underscore resolves the issue—no changes to the ADF pipeline code are required.

Next, we explore the parallel execution settings. By default, For Each can run multiple iterations in parallel. You can configure how many Copy Data activities run simultaneously using the batch count, but in our case with only two source files, it runs two Copy Data activities in parallel.

After editing the metadata file to include the missing underscore and republishing it, we debug the pipeline again. Now, both iterations of the For Each activity should run successfully. During the debug run, the Lookup activity correctly reads both file names (including the underscores), and the For Each activity executes two Copy Data activities concurrently.

At the end of the run, both source files are successfully copied into the Landing/labs_lab_three folder in the Data Lake storage account. One file represents the domestic product pricing, and the other represents global pricing. Currently, this process is limited to files for 1st January 2023 because the pipeline trigger to dynamically pass the relative URL file date has not yet been configured. That step will be implemented in the next lesson.

This entire run highlights several important points about metadata-driven pipelines:

Using metadata files allows you to manage source file names without changing pipeline code.

Lookup activities provide array outputs that can be iterated using For Each loops.

Sequential vs. parallel execution can be controlled to optimize pipeline performance.

Errors due to incorrect metadata are easy to fix without touching pipeline logic.

In summary, the pipeline now successfully reads the metadata file, iterates through each source file, and loads them into the landing folder, demonstrating a fully functional metadata-driven ADF pipeline for multiple source files.

# **J) Organising Folder Structure in ADF**

We can automate the pipeline run by adding triggers, which allows us to dynamically pass values for the file date parameter from the output of the trigger properties. When we try to include an existing trigger, we notice that it does not appear because a trigger, such as a tumbling window trigger, can only be mapped to one pipeline. If we want to use this type of trigger for a new pipeline, we need to create a new tumbling window trigger specifically for that pipeline.

As we develop the final production-ready pipeline, we will expand our current setup. So far, we have only been processing two files as part of lab exercises. The final pipeline will be designed to handle a full year of data into our landing container. The approach remains the same: all parameters, except the date parameter, will be moved into the metadata file, allowing for a flexible and scalable design.

Before building the production pipeline, it’s a good practice to organize the ADF workspace. We can create a folder structure under both Pipelines and Data Sets. During the learning phase, we have already created multiple pipelines (lab one, lab two, lab three) and several datasets just to understand different ingestion scenarios. For the final pipeline, we will create a clean set of pipelines and datasets without lab references, ensuring a professional, production-ready structure.

To organize the workspace, we create a folder called Working Labs for all the pipelines and datasets developed during the learning phase. Pipelines can be moved into this folder either by dragging and dropping or by right-clicking and selecting Move Item. Similarly, we create a corresponding Working Labs folder under Data Sets so that references between pipelines and datasets remain clear and structured.

Once the learning pipelines are safely organized into the working labs folders, we can minimize or close all existing pipelines to declutter the workspace. We then create a new folder called Ingest under both Pipelines and Data Sets, which will hold the production-ready ingestion pipeline. This folder will contain all the new datasets and activities required for the pipeline, and it will serve as the foundation for processing the full set of source files using the metadata-driven approach we have learned.

This setup ensures a clean, maintainable, and automated pipeline structure. We now have a solid foundation for building the final ingestion pipeline, leveraging metadata files, Lookup and For Each activities, and triggers to dynamically control processing based on date parameters.

# **K) End To End Metadata Driven Ingestion Pipeline - Create Metadata File**

We are now going to repair the Lab 3B pipeline and the datasets associated with it in order to create our final ingestion pipeline. The first step is to move all of the parameters—except for the file date—out of the pipeline and into the metadata file. This is because many of these parameter values are subject to change depending on the source system or other environmental factors. For instance, in the earlier pipeline, we were pointing to labs/lab3, but the actual one-year dataset now resides in the daily pricing folder of the HTTP web server. Therefore, parameters that define folder names or container names should be externalized into the metadata file for flexibility, while the file date will continue to exist as a pipeline parameter since it will be dynamically passed from the trigger.

To do this, we begin by copying all the existing parameters from the Lab 3B pipeline so that their names can be reused in the new metadata file. We then take the previously created metadata file and make modifications. Since we no longer need to reference the global pricing data for this pipeline, we remove it from the metadata file. That earlier configuration was mainly used to demonstrate looping through multiple files. In the future, if we need to load additional file types, we can easily extend this same metadata file by adding new entries for those files.

Next, we add a new key called relative URL folder name in the JSON metadata structure. This field defines the source folder path on the HTTP server. We format the JSON properly by enclosing the keys and values in double quotes. The value for this new field changes from "labs/lab3" to "daily pricing", since that is where the one-year source data resides. The file date parameter will continue to be supplied at runtime by the trigger, so it remains as a pipeline parameter.

In the same metadata file, we also define a relative URL file type and set it to "csv". Similarly, we include additional parameters for the sink (destination), such as sink container name and sink folder name. The sink container name will be "landing", which, although constant, is still worth parameterizing to maintain flexibility for future changes. The sink folder name, previously pointing to labs/lab3, will now be updated to daily pricing data. Thus, all ingested files will be copied under the landing/daily pricing data path. Finally, we add the sink file type as "csv".

After finalizing the new metadata structure, we save this file locally inside our area parameters folder. Since this is the finalized version for production ingestion, we will not include any “lab” references in the file name. Once saved locally, we upload this new metadata file to the Data Lake Storage Account, specifically under the ADF Metadata container. This ensures that our ingestion pipeline can dynamically reference all required configuration details from a centralized, parameterized metadata file.

With this, all the prerequisites for developing the proper ingestion pipeline are complete. The new pipeline will be built entirely from scratch—rather than cloning Lab 3B—so that we can consolidate and apply everything we have learned so far in one place. This will serve as a complete revision of all the concepts we have covered, including metadata-driven design, looping, parameterization, and dynamic activity execution. In the next lesson, we will begin creating the necessary datasets required for our ingestion pipeline from the ground up.

# **L) End To End Metadata Driven Ingestion Pipeline - Create Datasets**

Let's start by creating the source dataset for our ingest pipeline under the Ingest folder. We will refer to the Lab 3 dataset because that is the key reference for us. To begin, right-click on the Ingest folder and select New Dataset.

We know that it’s an HTTP Web Server dataset because our source data resides in the HTTP web server, and the format of the file is Delimited Text. We will provide a proper name for our dataset here. You can choose the existing linked service and specify the relative URL. However, we are not going to give the relative URL because this dataset is parameterized — meaning it will not point to any specific source file directly. Once this is set up, click OK.

Next, refer back to our Lab 3 dataset to review the parameters we created earlier, and understand how those parameters were mapped to the relative URL value. We can reuse the same parameter values because they were properly created and tested during the previous lab.

Now, go to the new dataset that we have just created. You’ll notice it doesn’t have any relative URL pointing to a source file yet. Go to the Parameters tab, click New, and create the same parameter that we used in Lab 3B. Then, we need to map this parameter to the connection object’s relative URL. Click Add Dynamic Content, and from there, map the parameter that you have just created.

This step also serves as a good revision of what we have done so far in the earlier labs. Once you make these changes, click Publish to save them.

Next, we will work on the Sink dataset parameters that we created for Lab 3. Open that dataset as soon as the previous changes are saved. It’s a good practice to keep closing any completed items so that you don’t get confused about which component you are currently working on.

Now, we need to create a new dataset for our Sink under the Ingest folder. Click New Dataset again. This time, our Sink dataset will be stored in Azure Data Lake Storage Gen2, and the format will again be Delimited Text. Give the dataset a proper and meaningful name. This time, we exclude “Lab 3” from the name because this pipeline is meant to be production-ready, not just for lab testing.

Once again, we will use the existing linked service, but we will not specify any container name or folder name directly for this dataset. This is because we are going to parameterize the full file path of our Sink directory, just like we did in the Lab 3 dataset.

To do that, copy the same parameters used in Lab 3. In this new dataset, go to the Parameters tab and create three parameters — one for Container Name, one for Folder Name, and one for File Name. Some parts of the parameters may change slightly, but you can quickly edit them instead of switching between datasets repeatedly.

Next, we need to map these parameters in the connection properties. For the file system, map the Container Name parameter. For the directory, map the Folder Name parameter. You can delete any incorrect or indirect mappings and add them again properly. Finally, map the File Name parameter to the file name field.

Now, these parameters will later be passed from the pipeline itself. Once done, publish the changes quickly so that we are ready with all the datasets needed for our final ingestion pipeline. You can close this dataset as well once it’s saved.

There’s one more dataset we need — the one that reads data from our metadata file. Copy the name from the existing Lab 3 metadata file, and create a new dataset under the Ingest folder. This metadata file resides in the Data Lake Storage Account, and the format of this dataset will be JSON.

It’s important to note that this is not a data file — it’s a metadata file. This file stores information such as the source file name, source folder name, and source file type values. It is used to read these values from the Data Lake Storage account.

Since this metadata file is always going to be one specific file for one type of ingestion, we don’t need to parameterize it. Instead, map it directly to the second metadata file that we created — not the Lab 3B one. This helps simulate a real-time project scenario, where metadata drives your ingestion dynamically.

Once mapped, click OK. You can quickly preview the data to ensure there are no errors in the JSON file format. If everything is correctly configured, it will read properly.

At this stage, we have created all the necessary datasets required for developing our ingestion pipeline. All changes are saved, and the datasets are properly organized under the Ingest folder.

In the next lesson, we will start creating a brand new pipeline under the Ingest folder, where we will use all these datasets to perform end-to-end ingestion of source files existing in the HTTP web server into the landing container of our Data Lake.

# **M) End To End Metadata Driven Ingestion Pipeline - Create Pipeline Part 1**

Now we can start creating the brand new pipeline under the Ingest folder. Once again, we are going to refer to the Lab 3 pipeline, so that we can revisit all the components we have already implemented. Some parts will be slightly different, but for the most part, we are replicating what we learned earlier in this new ingest pipeline.

Create a new pipeline and give it a proper name — similar to Lab 3B, but exclude the Lab 3B part from the pipeline name, as this is going to be a more generalized, production-ready version.

Next, we need to create the pipeline parameters. In Lab 3, we had a parameter named RelativeURLFileDate. We have moved almost all components except this parameter, and now we’ll rename it to something more meaningful — SourceFileDate — since this parameter actually represents the source file’s date value, which drives multiple components throughout the pipeline.

Similarly, we also need to create a pipeline variable that will store the converted version of this date value. This variable will hold the date in a specific format that is required to read files from the HTTP web server. Again, we’ll rename this variable from RelativeURLFileDate to SourceFileDate, maintaining consistency between parameters and variables.

We can also include a default value for this parameter to make quick testing easier after we finish developing the pipeline. This allows us to run the pipeline immediately for one sample date, verify its functionality, and later configure a trigger to automate it.

Now that we have our pipeline parameters and variables in place, the first activity we need to add is one that converts the date format into the specific structure required for reading the source files from the HTTP web server. The required format is MMddyyyy — it’s almost memorized for me, and hopefully, you’ll remember it easily too.

To achieve this, we’ll use the Set Variable activity. This activity will set the value for the SourceFileDate variable. Give this activity a meaningful name, and then, in the Settings section, select the pipeline variable we want to assign a value to.

In the Value field, click on Add Dynamic Content. This opens the Pipeline Expression Builder. Here, we are going to convert the pipeline parameter value (SourceFileDate) into the correct format by extracting the month, day, and year parts, since the original value might also contain a time component or a different date structure.

From the functions list, select the function formatDateTime(). Inside the parentheses, we need to pass two arguments — the source date value and the target format we want.
So, between the opening and closing brackets, we’ll write something like:
@formatDateTime(pipeline().parameters.SourceFileDate, 'MMddyyyy')

This expression converts the date into the required file-date format. You can quickly debug this step to verify that the output value is correct. Once executed, you’ll see that the variable now holds the expected date format.

The next step is to read the metadata file we created earlier, which contains the parameters that drive our ingestion logic. We already have a dataset configured for this metadata file, so we don’t need to create a new one.

To read this metadata file, we’ll use the Lookup activity. Drag a Lookup activity into the pipeline canvas and connect the output of the Set Variable activity to it. Give it a logical and descriptive name, such as FileJsonMetadata.

In the Settings section of the Lookup activity, select the dataset that corresponds to the metadata file. You can easily identify it by name — make sure to choose the one without “Lab 3” in its name, as that’s the latest dataset we created for this pipeline.

To double-check, you can click Preview Data to ensure it is reading the correct metadata file. If the data preview loads successfully, close the window. Now, make sure to disable the First Row Only option, because by default, the Lookup activity returns only the first record of the JSON file — and we need all the rows. We learned this behavior in our previous labs, and we’re simply reapplying that learning here.

When you run or debug this activity, you’ll notice that the Lookup output contains a property called value, which is an array. This array will be used as input for the next step — the ForEach loop. You can quickly debug and check the output structure; in earlier labs, it showed two array items, but in this scenario, it shows only one because we temporarily removed Global Pricing data. We’ll add that back later with the correct scenario.

Next, we need to include a ForEach activity to iterate over the items in this Lookup output. Connect the output of the Lookup activity to the ForEach activity, and give it a meaningful name.

In the Settings section of the ForEach activity, we’ll specify the input as the Lookup output’s value array. The Lookup activity returns multiple properties, but we are only interested in the value property, which holds the array of metadata records. This array will drive the looping logic for each file ingestion process.

Now, inside the ForEach activity, we’ll configure our Copy Data activity. This is where we’ll actually copy data from the HTTP source dataset to the Data Lake Sink dataset that we created earlier.

Additionally, we’ll need to pass the lookup output values — such as the Folder Name, File Name, and File Type — into the dataset parameters of both the source and sink datasets. This ensures that for each iteration, the correct file is read and written to the right location dynamically.

We’ll handle the configuration of these dataset parameters and map them correctly in the next lesson.

# **N) End To End Metadata Driven Ingestion Pipeline - Create Pipeline Part 2**

We need to click the activity section in the ForEach loop, or you can click the edit button inside the ForEach activity in the Pipeline design window. Both of them will take you into the sub-window. Now, we need to use the Copy Data activity here to read the data from the source and write it into the sink. Again, give a reasonable name for the Copy Data activity — for example, Pricing Data — and go to the source. We already configured the source dataset for this one, so just select the HTTP source pricing data. Look for it — I think it’s the shortest name here. Once it appears, it will ask for the value for the dataset parameter relative URL.

Because we already parameterized the relative URL connection object in the dataset, it’s now asking for the value for this parameter. Now, the value for this one, compared to the 3B pipeline, is slightly different. In the previous instance, most of the values were coming from the pipeline parameters, and one of the values was coming from the pipeline variable. But in our case, the file date is coming from the pipeline variable, and the remaining values are coming from the output of the Lookup activity. So, it would be better to copy the output of the Lookup into a Notepad so that we can easily map it later.

I would like to copy this value array output into a Notepad so that we can refer to it back when needed, or even we can refer to the metadata file that we created earlier. If you look at the output of this value array, you’ll see that the values are exactly the same as those coming from the metadata file. These key-value pairs are actually coming directly from the metadata file. So, we can refer to this metadata file to pass the values to the relative URL inside the Copy Data activity.

Now, close this and come inside the ForEach activity. Go to the Copy Data source and click the Dynamic Content option for the dataset parameter relative URL. Most of the values are coming from the output of the Lookup, and only the file date is coming from the variable value that we derived. If you click the ForEach iterator, it appears as item. — this is the reference for accessing the output of the ForEach loop anywhere in ADF. If you want to refer to the output coming from the Lookup through the ForEach, it will be referred to as item, and the values will either be copied from the metadata file or directly from the Lookup output — both are identical.

The first item we need to form in the relative URL is the relative URL folder name. You need to refer to it using the dot notation, e.g., item.folderName. The next one is the file name. However, we need to concatenate the folder name, file name, file date, and file type to form the full string for the relative URL. That’s what we have done in the 3B section as well. There, we used a concatenation of pipeline parameters, one output from the ForEach, and one variable value.

But in our current case, we need to get three values from the output of the ForEach and only one value from the pipeline variable. So, before referencing item, we need to include the concat() function that exists in ADF. If you are not sure about how to add it, remove the earlier dynamic content and start with the concat() function first — open and close the brackets properly.

The first element inside concat() is the ForEach item output for the relative URL folder name. That’s the one we start with. The next parameter is the file name, which also comes from the ForEach output. So, add a comma and then click on the ForEach item again. Remember, item is the default syntax to refer to anything inside the ForEach output.

Now, go back to your metadata file — the next part is the file name. The third part is the pyFileDate, which is coming from the pipeline variable that we already set. So, go to the variables section and add the variable value. The last part of the source file is the source file type, which is also coming from the ForEach output. So, again, click on the ForEach output, or you can even type item. followed by the key name. In your metadata file, this will be defined as relative URL file type.

Once the relative URL for the source is complete, we need to configure the sink parameters as well. Now go to the sink tab and select the sink dataset — ADLS Daily Pricing Data, which is the first dataset. It will ask for the values for three parameters.

The first one is very straightforward — it’s coming from the ForEach folder output again. So just click item. and go to your metadata file. This is stored as syncContainerName, so you can provide that value here. The next one is the sync folder name. We can directly map it here again — select the ForEach output and refer to the metadata file, where the sync folder name key is defined, and map it accordingly.

The last parameter is formed based on the file name, file date, and file extension. Again, we need to use the concat() function to combine multiple parameters coming from the ForEach output as well as the variable. The first part of the concatenation starts with item.syncFileName, which we defined as a key in the metadata file. Copy that one, then add the next part — file date, derived from the variable — and finally the last part, which is again coming from the ForEach activity output as item.syncFileType.

Hopefully, everything works fine. Sometimes, if we remove one of the closing brackets by mistake, we can manually add it after adding the sync file type. These three parameters together will form the sync file name. It’s okay if we deleted one of the closing brackets — we can just reinsert it.

Now, everything is set. If you publish the pipeline, your end-to-end pipeline is completely ready. It almost took about eight minutes to complete this pipeline, but to reach this stage, we have done a lot of experiments. This process helped us understand what value needs to be defined as a pipeline parameter, which ones need to be pipeline variables, and which components should be moved to the metadata file — and, most importantly, how we can reference them across different activities that we use.

Once we publish the code, our pipeline is ready for execution. In the next lesson, we will do one quick run to load a single file into the proper daily pricing folder in the landing area. Then, we will configure the trigger to load at least one month’s worth of data from the source files into the landing layer.

# **O) End To End Metadata Driven Ingestion Pipeline - Debugging And Error Handling**

I quickly opened our Data Lake Storage account and checked the landing folder. It contained only the Lab subfolder, but in this case, we are trying to load data into a new folder called Daily Pricing Data. So, if I run this pipeline now, it will load only one day’s worth of the file. I would like to make sure the pipeline is running end to end properly, without any issues.

To begin with, I am passing the pipeline date value as 2023-01-01 just to test it. Later, we will modify this setup by adding a trigger that will automatically pass the date value dynamically from the trigger output. But for now, I just want to run it once manually to ensure that all the configurations we have done for this pipeline are correct and there are no errors occurring anywhere.

When I executed the pipeline, it failed again. I decided to take this opportunity to debug it to find out which part of the configuration or code was causing the issue. You truly gain confidence in a specific technology only when you can analyze an error, identify its root cause, and fix it independently. Until then, you might feel unsure. That’s why one shouldn’t be afraid of errors—they are actually the best way to learn.

Looking at the error details, I noticed that the problem was again with the Request URL, which has been a common issue from the beginning of our setup. I copied the Request URL value into the metadata file to examine it more closely and identify the root cause.

On inspection, I realized that the first part of the URL comes from the linked service, and then the Daily Pricing folder name follows. That part looked fine. However, I noticed that there was no slash ( / ) after the folder name, which is required to correctly form the path. That was one issue.

Additionally, after the date value in the URL, the source file name was being repeated, which suggested that instead of mapping the relativeURL_fileType, I had accidentally mapped relativeURL_fileName again in the pipeline configuration.

To confirm, I went back to the Copy Data activity and reviewed the Source configuration. As suspected, I had mapped the wrong field. I corrected the mapping to ensure that relativeURL_fileType was properly referenced instead of the file name.

Next, I needed to fix the missing slash issue. I opened the metadata file, added a slash ( / ) after the relativeURL_folderName, and saved the file. With these corrections in place, I expected the pipeline to run successfully.

Before re-running, I also double-checked the Sync file name mapping to ensure that the sync_fileType parameter was copied correctly. It looked fine.

Now, I re-ran the pipeline by clicking Debug again, passing the same date value (2023-01-01). This time, the pipeline ran successfully without any errors.

I quickly navigated back to the landing container in the Data Lake to verify the output. As expected, a new folder named Daily Pricing Data had been created, and it contained the newly copied file. I opened and checked the data inside — everything looked perfect.

With this, our pipeline is now confirmed to be running end to end successfully. It is fully ready to be included in the scheduled trigger so that it can automatically load multiple days or even months of data from the source files into the landing layer going forward.

# **P) End To End Metadata Driven Ingestion Pipeline - Create Tumbling Window Trigger**

We can add the trigger to start running from the 1st of January 2023. For now, we will run the first ten days, and later we can extend it for the entire year. So, we need to create a new trigger. Even though we already created the tumbling window trigger, it won’t start to appear because that is one of the limitations of the tumbling window trigger. Therefore, we need to create a new tumbling window trigger for the daily pricing load.

We are going to choose the type as a tumbling window trigger, and we need to start from January 1st, 2023. I would like to set the time as 00:00 (midnight). It needs to start at 12 a.m., and we will slowly increase the end time. For the time being, we’ll set it for one week, and it should run every 24 hours because new files are generated every 24 hours.

When you go to the “Specify End Date” section, I would like to set it for one week first to make sure everything is working fine. Or maybe we can set it for ten days, up to January 10th, 2023, 00:00 hours. I think it will load nine files because tumbling window triggers start only at the first end time, not at the start time. That should be fine — if it loads nine files, we are okay.

Also, one more option I mentioned earlier — I would like to run two days’ worth of data in parallel. Previously, we ran one after another, but now, in a single run, it will start the 1st and 2nd together, then 3rd and 4th, 5th and 6th, 7th and 8th, and the last run will probably be a single one. We can see this behavior in the Monitor window as well.

As soon as I click OK, this trigger is associated with the pipeline. Now it’s asking only for the value of the pipeline parameter source_file_date. We need to pass the output of the tumbling window trigger property called window start time, just like we did earlier. I will share the link to the specific Microsoft support document for reference. You need to include “@” before it — that’s the way to pass the trigger output value to the pipeline parameter.

Once we click OK, and then Publish, it will start running via the trigger. Previously, we ran it in Lab 3, but this time the pipeline will start running the specific configured pipeline. I’ll now click Publish All and publish. Hopefully, the first trigger run will be successful. But if some errors occur, we’re happy to look into them — because that’s the opportunity to learn about different types of errors.

If you observe, since the concurrency is set to two, it’s starting the 1st and 2nd of January together. Previously, it ran sequentially, but this time, with the concurrency property set to two, it runs two pipelines at the same time. For the historical data, we need to catch up almost 365 days — actually, around 400 days of data since it’s the 30th of January. So, we can set it up to run any number of days, even up to 50 days, in parallel.

We will wait for the completion of this trigger run. It’s running two days’ worth of ingestion in parallel after each successful completion of the previous one. If you look at the pipeline parameter value passed here, it’s 0103, then it keeps increasing — 0104, 0105, and so on — until it reaches the 10th of January 2023. Then it stops because we’ve set the end date.

We don’t want to start loading 365 days’ worth of data right now because we still need to develop the subsequent layers in the Data Factory. I would like to quickly bring back the entire architecture to remind ourselves where we are and what we’ve done so far — as a summary of this section — before moving on to the next lesson.

The run was successful for all the days we configured. When we check, the final day processed will be the 9th of January 2023 because we set the end date as the 10th. If we go to the landing container and refresh the Daily Pricing folder, it should now contain nine days’ worth of data.

So, at last, we have developed a proper pipeline that loads data from the source (HTTP web server) automatically. It dynamically picks up changes in the source filenames and stores the data in our landing container in the Data Lake Storage Account without any user intervention. Once the trigger is set, you don’t have to do anything manually — just observe how it runs in the Monitor window.

We’ve done a really good job! It took three hours to reach this level of understanding of a real-time pipeline. Now, if we want to develop another metadata-driven pipeline for reading data from a database instead of an HTTP web server, we can reuse this same logic. The only difference will be in the source and sink datasets.

We can quickly create one metadata file listing the tables to be loaded from the database, build a similar pipeline, and run it inside a ForEach loop. In the Copy Data activity, we can configure parameter-driven source and sink datasets, and it can be done in just ten minutes.

However, since this is our first time working in Azure Data Factory, we needed to explore each and every component step by step to reach this point. I’m really happy — if you were able to develop this final pipeline successfully, you can easily refer to all our previous pipelines without any issues.

That’s why we built all those earlier pipelines — to show you different variations in pipeline development. This one is the optimal pipeline, designed to run automatically without any manual intervention. You can load any number of days’ worth of data effortlessly.

We’re starting from January 2023 and can eventually extend it to today — around 400 days’ worth of data in total. I plan to execute that full run after developing the subsequent layers.

In the next lesson, I’ll give you a quick summary of what we’ve done so far against our original architecture. Then, we’ll move on to building the next layer — because we now have enough data in the landing layer to start building our reporting layer.

# **Q) Data Ingestion From HTTP Web Server - Summary**

Now that we have developed our first ingestion pipeline, let’s go through the overall end-to-end project architecture to understand all the components we have completed so far.

We are ingesting data from the CDP Web Service, and we have developed the ingestion pipeline to read the data from the HTTP web server. In this pipeline, we applied a metadata-driven ingestion approach so that whenever new files need to be ingested from the HTTP web server, we only need to include them in the metadata file — no code changes are required in the pipeline at all.

The pipeline also runs automatically without any user intervention, thanks to the scheduling component — the trigger in Azure Data Factory. This trigger ensures that the pipeline runs daily, reading data from the HTTP web service for that specific day’s file and ingesting it into the landing container in our Data Lake Storage Account.

We have also implemented an incremental load mechanism. This means that the pipeline reads and ingests one file per day. Once a file is successfully ingested into the landing container, it won’t be read again from the source. We achieved this using a combination of the trigger mechanism and trigger properties. For each run, a new date value is passed dynamically to the HTTP web server, which fetches the corresponding source file and loads it into the landing container.

There are various approaches available to perform incremental loading, and we will revisit this concept in the transformation section under the topic of delta records processing. We will also explore different types of schedulers when we move on to building the reporting database.

The next section we are going to focus on is the reporting layer. To begin that, we will start with dimensional data modeling. In the next section, we’ll start designing the dimensional data model for the pricing data that we have copied into the landing container under the folder Daily Pricing.

# **VI) Reporting Database Design - Dimensional Data Modelling ( Star Schema )**

# **A) Dimensional Data Modelling Overview**

In the previous section, we developed the Data Factory pipeline to read data from a web service and ingest it into the landing container in the Data Analytics project as part of our development. We learned how to ingest data from an HTTP web server and how to make that pipeline metadata-driven so that any new source files in the source system are automatically included in the pipeline by simply updating the metadata file stored externally from the Data Factory. We also explored the Data Factory automatic scheduling component, called a trigger, which allows the pipeline to run automatically without user intervention.

So far, we have successfully loaded ten days’ worth of data into the landing container in the Data Lake storage account. Additionally, we explored how to perform incremental loads by fetching only the new source files generated in the source system on a daily basis. Although there are still two more ingestion components that we need to develop, we now have a clear understanding of our ingestion pipeline, which will make the remaining ingestion development quicker. I would also like to bring in these additional ingestion components later in the course, with proper requirements, to show why this additional data is needed for subsequent layers.

Next, we are going to explore how to build Data Factory pipelines for transforming our source data in the landing layer. To define the necessary transformations, it is essential to know the output required in the final layer. Without understanding what the final layer will produce, we cannot properly define the transformations. Therefore, our next step is to build the reporting layer.

Designing the reporting layer requires designing the final layer in the Data Analytics project using a data modeling technique called dimensional data modeling. We will explore dimensional data modeling first because once the final model is designed, we can return to Data Factory and develop the pipelines to transform and load the source data into this dimensional data model.

We will focus on learning how to perform dimensional data modeling for our source data rather than discussing why this modeling technique is chosen. Dimensional data modeling is a mature and efficient technique that has been widely recommended for reporting requirements for many years. As soon as reporting requirements arise, it is common practice to use dimensional data modeling.

Dimensional data modeling is widely supported by major service providers, including Microsoft, Databricks, IBM, and Amazon. These providers offer infrastructure and features that facilitate building dimensional data models because this technique is frequently used and well understood. For reporting purposes, dimensional data modeling is the preferred approach. While other modeling techniques, such as Data Vault, exist, they are not entirely suited for reporting purposes. In contrast, any reporting requirement can generally be met efficiently using dimensional data modeling.

In the next lesson, we will focus on designing the dimensional data model for our source data, which will then guide the development of Data Factory pipelines to load this model.

# **B) Dimensional Data Modelling - Source Data Overview**

We are going to perform dimensional data modeling for our source daily pricing data that we ingested into the landing layer under the folder named daily pricing. To perform this data modeling effectively, we first need a clear understanding of the data. Normally, data engineers do not perform data modeling themselves, but it is important for us to understand the outcome of the data model. This understanding is essential because the design of the pipelines to populate the reporting layer in our project depends directly on the data model.

To better understand the data, I have copied one of the source files into an Excel spreadsheet to gain a clearer visibility of the data. While we have already explored the nature of the data copied into our landing layer, we will review it again because understanding the data thoroughly is a prerequisite to performing data modeling.

The data captures pricing information and the quantity of products arriving at various markets across different states in India. Both the pricing information and quantity of arrivals are recorded on a daily basis, giving us date-wise information. The second column, row ID, is a unique identifier for each row in the table, but it does not carry any business significance. The state name column is associated with each individual market, and products are logically grouped into product groups. Some products also include variety information. The origin information is not consistently populated; in many cases, it is recorded as “not recorded,” but we will not focus too much on the origin information.

Within this dataset, the non-changing or slowly changing information includes the market, product group, and products. Most of the time, this information is stable and rarely changes. For example, if the pricing for a specific product in a specific market is missing on a particular day, it may not appear in the file for that day, but once the pricing is available, it will be recorded.

On the other hand, the changing information includes the quantity of products arriving at the market on a specific day and the pricing information for that product in that market on that day. These values change daily and form the dynamic part of our data, which will drive the fact tables in our dimensional data model.

# **C) Identify Business Description(Dimension) and Business Measures(Fact) Columns**

Let’s start performing logical data modeling. As mentioned earlier, logical data modeling involves designing the data model purely based on the business context, without considering how it will be implemented in the database. To do this effectively, we need to frequently switch between the source data and the logical data modeling sheet because the structure of the model is entirely determined by the nature of the data.

To guide our logical data modeling, I have listed a few steps. The first step is to identify all the columns, attributes, or data elements in the dataset. Whenever I refer to columns, attributes, or data elements, I mean the same thing and will use these terms interchangeably. In our case, the source data is in a consistent format across all days, so we can capture all column names from the source file and copy them into the logical data modeling sheet. I have also created some sample data from the source, which includes different variations. Bringing this sample data into the logical data modeling sheet will help us perform the next steps.

The next step is to split the columns into business description columns and business measure columns. We need to identify which columns describe the business context and which columns quantify the business. Business description columns are mostly textual and provide context about the data. For example, the state name represents the market where a specific product arrived on a specific day. Similarly, market name, product group name, product name, and variety are textual values describing aspects of the data.

On the other hand, business measure columns are numeric and quantify business activities. In our dataset, arrival quantity, minimum price, maximum price, and modal price are business measures because they quantify the quantity of products that arrived and the price range for that product on a given day.

Some columns, like row ID, are not significant for modeling because they are just sequential numbers and do not affect pricing or product quantities. The date column, however, is critical and should always be included in the data model since it allows us to analyze business metrics over time. The origin column is inconsistently populated and will not be considered in our modeling.

In this step, we will copy all the business description columns—from state name through variety—into one section of our logical data modeling sheet. Separately, we will copy all the business measure columns—arrival quantity, minimum price, maximum price, and modal price—into another section. We will leave one column space between the business description and business measure columns for clarity. This separation allows us to clearly see which columns describe the business and which ones quantify it.

With this step completed, we are ready to proceed to the next stage of logical data modeling, which we will start in the next lesson.

# **D) Identify Business Description(Dimension) Column Groups Having 1-1 Relationship**

In the previous step, we identified business description columns and business measure columns. Naturally, business description columns store information in textual form, while business measure columns capture data in numerical values.

The next step is to group the business description columns. The idea is to group columns where a value in one column is related to only one value in another column. We start by creating the first group and comparing data between state name and market name. If one state is always associated with only one market, they can be grouped together. However, in our dataset, a state like Uttar Pradesh has multiple markets, so these columns cannot be grouped together. We also check the reverse relationship: if one market always exists in one state, then they could be grouped. But in some sample records, there is ambiguity—for example, a market name exists in both Uttar Pradesh and Odisha—so these two columns are placed in separate groups.

Since these two columns have a one-to-many relationship rather than a one-to-one relationship, we do not need to compare them with other columns for grouping. Moving on to product group and product name, we compare these next. One product group can have multiple products, which is a one-to-many relationship. However, if we look from the product name perspective, each product is associated with only one product group. This means these two columns can be grouped together because each product name maps to a single product group, even though multiple products exist within the same group.

Finally, we consider the variety column. This is a slightly tricky situation. Variety information has a one-to-one relationship with the product name, but the pricing information for different varieties may change for the same market on the same day. If we include variety in the same group as the product, we would not be able to capture these differences in pricing. Additionally, logically, over a longer period, a product can have multiple varieties, each potentially having different pricing in the same market. Therefore, variety is placed in a separate group.

Following this process, we have created four groups of business description columns. The next step will be to convert these groups into dimension tables, which we will cover in the next lesson.

# **E) Logical Data Modelling - Designing Dimension Tables**

The next step is creating the dimension table for each group of business description columns that we identified in the previous step. Now, we need to understand what a dimension table is. A dimension table is basically a terminology used in dimensional data modeling to store or identify the group of business description columns that have a one-to-one relationship together as a single table.

So, we need to copy all of the groups that we identified in the previous step and convert each group into a dimension table. Logically, we can start by naming them. The first one can be called dim_state, where dim stands for dimension. This is the standard naming convention followed in most projects, so we’ll adhere to the same practice here. The next one will be dim_market, followed by dim_product, and finally dim_variety.

Now, we have successfully changed each group into its respective dimension table reference. The next step involves creating a surrogate key for each dimension table.

So, what is a surrogate key? If you look at it closely, when we talk about a one-to-one relationship, it means that each group or each dimension table will store only the unique values of the columns that we identified earlier. For example, in the source file, the state name might be repeated multiple times. However, when we store it in the reporting database, we don’t need to store all the repeated state name values. Instead, we will identify the unique state name values from the source file, and for each of those unique state names, we will assign an ID value. This ID will be used as a reference in the reporting database to link the state information between tables.

Therefore, we need to create a unique ID column in each dimension table to represent the dimension attributes we are storing. This is what the current step is about. We’ll copy all of the dimension tables and include an ID column in each of them.

For instance, the state name will have a new surrogate key called state_id, which we are going to generate and populate using the Data Factory pipeline. Similarly, the market dimension will have market_id. In the product dimension, we have two elements, but since the product group name does not change for each product, we will assign only one ID column for the product dimension. Finally, the variety dimension will have variety_id as its surrogate key.

We will keep the columns we are adding (the surrogate keys) in a different color from the actual columns coming from the source so that it’s easier to distinguish them. Now that we have included surrogate keys for all the dimension tables, we can arrange all the columns properly in a single row view rather than spreading them across columns. This helps us clearly visualize all the dimension tables side by side.

With this, we have successfully included the surrogate keys into each of the dimension tables. The next step in the process is identifying the fact table, which we will discuss in the upcoming lesson.

# **F) Logical Data Modelling - Designing Fact Tables**

We have almost completed our dimension table creation steps, and now we are moving on to the fact table creation step. A fact table is a terminology used in dimensional data modeling to store the business measure column values. In other words, it contains the quantitative data or numerical metrics that represent business performance.

So, as per our model, we need to create a fact table for our daily pricing data. We will name this table fact_daily_pricing. In this table, we will include all the business measure columns, which capture the measurable aspects of the business process.

To better understand this, let’s focus on the business measure values themselves. If we hide all the business description columns and only look at the business measure values, these values alone don’t convey any meaning. For example, if we just see a number like 23 in the dataset, it doesn’t make sense unless we know which product, which market, and which state that value belongs to. Without the context provided by business description columns, the numbers are meaningless.

In the source data, all these columns existed together in a single file, so we could easily relate the measure values with their corresponding descriptive attributes. However, now that we have split the data into multiple dimension tables and a fact table, the relationships must be re-established using keys. Therefore, when creating the fact table, we must link it to the dimension tables using foreign keys.

These links will not be based on the original business description columns (like state name or market name) but instead on the surrogate keys we created earlier. Each dimension table now contains a unique surrogate key (for example, state_id, market_id, product_id, and variety_id). In our pipeline development, we will use these surrogate keys to join the fact table with the respective dimension tables.

Hence, the fact table will include both the business measure columns and the surrogate key columns from the dimension tables. This structure ensures that each fact record is connected to the correct business context — such as which product, market, or state it refers to. That’s essentially how the fact table is designed and created.

Now, we have almost reached the final step — creating the dimension table for date columns. As mentioned earlier, date is a default and essential dimension in any reporting database. Without a date, it’s impossible to track or analyze data over time, since every business event occurs at a specific point in time. Therefore, we will include a date dimension table by default in our reporting schema.

For now, we’ll include only the date_id column — a surrogate key representing each unique date. The date dimension table is typically pre-populated, as dates can be derived and generated in advance (for example, one entry for every day of the year). This pre-population process is something we’ll handle in one of our upcoming jobs.

So far, we have successfully identified and defined both our dimension tables and fact tables. However, at this stage, we are only performing logical data modeling. That means we are focused on understanding and designing the structure conceptually — without worrying about how these tables will be physically created in the reporting database, which naming conventions will be followed, or what data types each column will have.

In the next lesson, we will move to physical data modeling, where we will learn how to implement these identified dimension and fact tables in the reporting database, define the appropriate data types, and follow best practices for naming conventions and database design.

# **G) Physical Data Modelling Overview**

Now, we are moving on to the physical data modeling phase, which is based on the output from our logical data modeling. From the logical model, we have already identified a set of dimension tables and one fact table. In this step, we will take all those identified tables and apply the necessary steps involved in physical data modeling to complete our overall dimensional data model design.

To begin, we will copy all the dimension tables together, along with the fact table that we identified earlier during the logical data modeling phase. Once we have them all in one place, we can start the physical data modeling process systematically.

The first step in physical data modeling is to identify the data type for each column in the logical data model tables. It’s important to note that we do not define data types for the tables themselves — only for their columns. Data types determine what kind of data (for example, text, number, or date) can be stored in each column when we implement the model in the reporting database.

Let’s take the Dim_State table as an example. This table contains two columns. Since we are now preparing to implement this table in the actual reporting database, we must specify appropriate data types for each of its columns. When creating dimension and fact tables physically, defining data types is a crucial step because it ensures proper data storage, consistency, and query performance.

To make the process clearer, we will organize our tables and columns in a structured layout. We’ll create a header called Table_Name, where we will list all the table names. Next to that, we’ll have another header called Column_Name, where we’ll list all the columns corresponding to each table. This arrangement helps us visualize and understand which columns belong to which table more effectively.

After rearranging, we will include all the dimension tables and the fact table that we captured earlier. We’ll also ensure that the Dim_Date table is added here, so that we don’t miss anything. The Dim_Date table contains the columns date_pricing and date_id, which are part of our date dimension.

Now, we have successfully listed all the dimension tables and the fact table that were identified during the logical data modeling stage. The next step in this process is to assign data types to each of these columns appropriately. This step will be performed in the upcoming phase of our physical data modeling process.

# **H) Physical Data Modelling - Identifying Data Types**

Now, we are going to identify the data type for each of the columns that we defined earlier during our logical data modeling. The data type determines how data will be stored in the database, and since we are using the SQL Server database for our reporting system, we will use the data types available in SQL Server. We can choose the most suitable data type for each column based on the type of data it will hold.

Let’s start with the state name column. To decide the correct data type, we first need to know what kind of values are coming from the source. Since the state name is a text value, we’ll need to assign a text-based data type. Additionally, we must check the length of the values coming from the source file to determine the maximum number of characters used.

To find this, we can use an Excel function to calculate the length of each state name and identify the longest one. After applying the filter, we find that the maximum state name length is 18 characters. To be on the safe side, we will define the data type as VARCHAR(100). This ensures that all possible state name values will fit comfortably without truncation.

We can also confirm that SQL Server supports the VARCHAR data type. The benefit of using VARCHAR is that if the value stored doesn’t use the full defined length, SQL Server will not allocate that extra space — making it efficient in terms of storage. Hence, VARCHAR(100) is a good choice for the state name column.

Next, let’s move to the state_id column. This column will contain a surrogate key, which means it will store a sequence of numbers generated for each unique state. Therefore, we will use an INTEGER data type. According to Microsoft’s documentation, the integer data type can store values up to billions, which is far more than what we’ll need in this case. Hence, INTEGER is sufficient for all ID columns.

We’ll apply the same logic for all other ID columns across the dimension and fact tables, such as market_id, product_id, variety_id, and date_id. To maintain consistency, we’ll use INTEGER in uppercase for all these columns, since these are the key identifiers used to link tables.

Now, let’s look at the market name column. We’ll examine the source data to determine the maximum length of the market name. Using the same Excel function, we find that the maximum length is 41 characters. To stay consistent and safe, we’ll again use VARCHAR(100) for this column. The same logic applies to product name and product group name — even if their current lengths are less than 100, defining them as VARCHAR(100) ensures flexibility for any new or longer values that may appear in future data files.

This is the typical process followed in real-world projects — we identify what values are being stored in each column, determine their maximum lengths, and then decide the appropriate data type and its length accordingly. By using VARCHAR(100) for all string columns, we ensure that no values will be truncated and that there’s enough room for potential future growth in data size.

Now, let’s move on to the numerical columns such as arrival_intent, minimum_price, and maximum_price. Since these values can contain decimals, we need a data type capable of storing decimal values accurately. In SQL Server, the DECIMAL data type allows specifying both precision and scale. Precision determines the total number of digits, and scale specifies how many of them appear after the decimal point.

We can store up to 38 digits in a decimal type, which is more than enough for our needs. After reviewing the product pricing data, we find that the largest whole number goes up to around five digits. Therefore, to stay on the safe side, we’ll use DECIMAL(18,2) — which allows up to 16 whole numbers and 2 decimal places. This will ensure that all our pricing-related values are stored accurately without loss of precision.

Next, let’s look at the date_pricing column. This column comes directly from the source data and represents a date value. For this, we will use SQL Server’s DATE data type, which can efficiently store date information without including time components. Finally, the date_id column will again use the INTEGER data type, since it serves as a surrogate key representing each unique date.

With this, we have completed the first step of physical data modeling, where we identified and assigned the appropriate data types for all columns across our dimension and fact tables. In the next lesson, we will continue with the subsequent steps of the physical data modeling process to further refine and implement our dimensional model.

# **I) Physical Data Modelling - Applying Naming Conventions**

The next step in our process is to apply proper naming conventions to all table names and column names.

Fortunately, most of the naming conventions have already been applied — for instance, I’ve used underscores (_) in column names instead of spaces. This is a crucial best practice because spaces in object names can create unnecessary issues when building or querying database tables.

When converting our logical dimension tables into physical dimension tables, it’s important that we follow consistent and standardized naming conventions. This ensures that the tables can be easily created, maintained, and referenced in the actual reporting database without running into syntax or compatibility problems.

Therefore, for each of the dimension tables, I’ve replaced any spaces in the table names with underscores. I’ve followed the same process for the fact table as well. Remember — even the fact table name should not contain any spaces.

These steps align with standard database best practices, which emphasize using underscores and lowercase letters for naming database objects to maintain clarity and avoid errors.

I’ve now copied and renamed all relevant tables accordingly, including the last one — the dim_datetime table — where the space has also been removed.

Now, moving to the next step — since we are working on a dimensional data model, this structure is typically created within the logical layer of a data analytics project. In practice, this layer is often referred to as a data mart, data warehouse, or star schema — all of which represent similar concepts used to organize and store analytical data efficiently.

As part of building this physical data model, we also need to include auditing columns in each table.

These columns are essential because we are responsible for populating and maintaining these tables. Having audit columns allows us to track when each record was created and when it was last updated in the reporting database.

This additional logging helps us ensure data integrity, maintain accountability, and trace data changes over time.

So, for every table — whether it’s a dimension table or a fact table — we will add a few extra columns specifically for auditing and logging purposes.

# **J) Physical Data Modelling - Including Audit Columns and Define Database Schema**

The next step is to add ARD Reporting Database Audit Columns.

Now, what is meant by “audit”?

For example, suppose we are loading a specific table that contains a unique list of state names and state IDs. In such cases, we need to know when a particular record was inserted into the reporting database. Later, if the same record is updated, we should also be able to identify on what date and time that update took place.

This process of maintaining audit information helps us have better understanding and control over the data we store in the reporting system. The reporting database is typically loaded on a daily basis, and sometimes a specific error might be ignored or an error log might be missed on a particular day. If a user raises an issue at a later time, we must be able to verify when that specific record was created and when it was last updated.

In some cases, even the source system may send incorrect information. If we have the audit details stored, we can easily trace back and confirm that on a specific date we received incorrect data from the source. This helps us in identifying and rectifying data issues efficiently.

Both of these audit columns are designed to store datetime values, which capture the exact timestamp when each record was inserted and when it was updated in the reporting database. This is considered a standard best practice that we follow in all professional reporting database designs.

Therefore, we need to include these two columns in all the tables that we have created so far. By doing so, we will be able to maintain a better track of the data being loaded into the reporting database and ensure proper data governance.

Just to clarify once again for your reference: all the text shown with a white background represents columns that we will create and populate ourselves, whereas the text in the blue background represents columns that come directly from the source file.

We are responsible for developing the data pipelines that will load these tables with data from the source systems. However, before we can build those pipelines, we first need to create the tables in the database. And before we create those tables, we must first create the reporting database itself in our Azure tenant. That’s exactly what we will be doing in the next lesson.

After completing all the steps in physical data modeling, the final step in physical database modeling is to identify and create the database schema. The database schema will serve as the logical structure that holds all of our tables.

The database stores data in the form of tables, which represent the storage layer of our reporting system. Within a single database, we can have multiple schemas, meaning that several applications can store their data in the same database, each within its own schema.

For our reporting-specific tables, we should be able to easily identify and group them separately. A schema name functions similarly to a folder name in normal file storage. It serves as a logical grouping of a specific set of tables inside the database, making them more organized and easier to manage.

For our project, we will create a schema named reporting. Once we have created the database, we will come back here and define this schema name inside the reporting database.

At this point, we have completed all the physical data modeling steps. The next step is to create the SQL Server database in our Azure account and then start creating these tables within that database.

I’ll see you in the next lesson where we begin setting up the Azure SQL Server and the reporting database.

# **K) Setup AZURE SQL DATABASE - Overview**

We have now completed designing the reporting database using the dimensional data modeling technique. As the output of this modeling process, we have identified a set of dimension tables and a single fact table.

The next step is to create these dimension and fact tables in the SQL Server database and then proceed to develop the Azure Data Factory (ADF) pipeline that will load data into these tables.

To begin this process, we will first create the Azure SQL Database resource within the Azure Cloud environment. Once the database resource is successfully created, we can then move forward to implement the dimension and fact tables — specifically, the star schema design that we identified earlier as part of our dimensional data modeling phase.

This will establish the foundation for our reporting database, enabling us to perform efficient data loading, transformation, and reporting through our Azure Data Factory pipelines.

# **L) Azure SQL Database Query Editor Overview**

The database and the database server have now been successfully created. When you go to Resources in the Azure portal, it will open the database overview window. This overview displays important details about your database, such as its name, location, and connection information.

If you need to connect to the database externally, you must use the server name provided in this overview. Within the Azure portal, you will also find the Query Editor window. This editor allows you to quickly connect to and interact with your database directly inside the Azure environment.

When connecting to the database, you can use either Microsoft Entra Authentication or the SQL username and password that you created earlier while setting up the database server. If you choose the username option, simply go back to your database server, select Go to Resources, open the Query Editor, and provide the password that you configured during creation. Once authenticated, you will be successfully connected to your database server.

There are two ways to connect to your database — using Microsoft Entra Authentication or your SQL username and password. Both of these methods will work and allow you full access to the database. Once connected, if you want to store any data, the basic object that you need to create is a table.

At the moment, there are no tables in our database, which is why nothing is displayed under the tables section. Other database components such as views, stored procedures, and user-defined functions can be created later once we have the proper requirements. For now, the table is the most fundamental object we must create before exploring any additional components in the database.

We have already identified the database tables from our dimensional data model. As an example, let’s start by creating the DimState table. I will now teach you the SQL syntax used to create tables — it’s quite simple and easy to follow, even if you’re new to database servers.

To create a table, we use the SQL command:

CREATE TABLE <table_name> ( ... );

You first specify the table name, followed by an opening and closing bracket. Inside these brackets, you provide a list of columns along with their respective data types.

For now, we will create just one table to learn how the CREATE TABLE command works. If you already have the column names and data types prepared in an Excel sheet, you can copy and paste them directly into the Query Editor. When you do so, make sure that each column definition is separated by a comma, except for the last one — otherwise, the SQL command will fail.

Once everything is ready, run the SQL command. This will create the table in your database. If you don’t see it immediately, click the Refresh button, and it will appear under the list of tables.

You’ll notice that the table was created with the name dbo.DimState. The prefix dbo refers to the database schema. In SQL Server, a schema is a logical grouping of database objects such as tables, views, and stored procedures.

Since we did not specify a schema name during table creation, SQL Server automatically used the default schema, which is called dbo. The dbo schema is built into every SQL Server database by default.

However, in our case, we have already decided to use a custom schema for our reporting database. Therefore, we do not want to keep this table under dbo. Instead, we will drop this table and recreate it under the correct schema.

To drop a table, we use the SQL command:

DROP TABLE <schema_name>.<table_name>;

You can either prefix it with dbo or leave it out. If you omit the schema name, SQL Server assumes the dbo schema automatically. So if you run the command DROP TABLE DimState, it will look for the table under the dbo schema and remove it.

If you only want to execute a specific SQL statement inside the Query Editor, simply select that line and click Run. After executing the drop command, you can click the Refresh button again to confirm that the table has been deleted from the database.

Next, since we have planned to use the reporting schema, we need to create the schema before creating any tables under it. To create a schema, the SQL syntax is:

CREATE SCHEMA reporting;

After running this command, you’ll see a message that says “Query succeeded. Affected rows: 0.” This means the schema was created successfully.

Now, we can go ahead and create our first table under this new schema. To do this, we prefix the table name with the schema name followed by a dot. For example:

CREATE TABLE reporting.DimState ( ... );

Here, the dot (.) separates the schema name and the table name.

If you try to create this table and receive an error stating “There is already an object named DimState in the database,” it likely means the table was already created earlier during previous runs. You can confirm this by expanding the Tables section in the Query Editor — you’ll be able to see the table name along with all the columns and data types that you defined.

The Query Editor also allows you to execute simple queries. For instance, you can check the data in a table by running:

SELECT TOP (100000) * FROM reporting.DimState;

Currently, this query won’t return any rows since we haven’t loaded any data yet.

In summary, the Azure Query Editor is a powerful and convenient tool that enables you to connect to your database, execute SQL commands, create schemas and tables, and query data — all directly within the Azure portal.

# **M) SQL Server Management Studio Overview**

Another commonly used SQL Server database client tool for connecting to and managing databases is called SQL Server Management Studio (SSMS). This is a powerful and user-friendly application that provides a graphical interface to interact with your SQL databases.

I will provide you with the download link for SQL Server Management Studio. You can download it directly onto your computer and proceed with the installation. The setup process is straightforward — once installed, you can open the application to begin using it.

When you first open SQL Server Management Studio, you will see a connection window where you need to enter the Server Name. The server name can be copied from the database overview window in your Azure portal. Simply go to your Azure SQL Database resource, copy the server name, and paste it into the SSMS connection dialog box.

Next, under the Authentication section, you will notice that SSMS supports multiple authentication types. The two main options are:

(i) Azure Active Directory – Universal with MFA (Multi-Factor Authentication)

(ii) SQL Server Authentication

For this example, we will use SQL Server Authentication. You will need to provide the username and password that you set up while creating the Azure SQL Database server. Once you have entered these credentials, click on Connect to log in to the database server.

After a successful connection, SSMS will display the Object Explorer panel on the left-hand side. This panel shows the list of all databases available on the connected server. You can expand the databases to explore their objects — such as tables, views, stored procedures, and more.

Inside the database, you will be able to see any tables that have already been created. For instance, earlier we created a table called reporting.dim_state. You should be able to locate this table within the reporting schema in the Object Explorer.

If you want to view the data stored inside this table, SSMS provides a convenient feature. You can simply right-click on the table name and select “Select Top 1000 Rows”. This will automatically generate a SQL query in a new query window that retrieves the top 1,000 records from the table.

To execute this query, click the Execute button on the toolbar (or press F5). The results will then appear in the Results pane below the query window. Since we have not loaded any data into the table yet, the result set will be empty — but this step confirms that your table is accessible and ready for data loading.

At this point, you can choose to continue working with either SQL Server Management Studio or the Query Editor inside the Azure portal. Both tools serve the same purpose — allowing you to interact with the database, run queries, create tables, and manage objects.

Whichever tool you find more convenient or comfortable to use, you can continue with that for your upcoming database development and management tasks.

# **VII) Dimension Tables Load - ADF DATAFLOW Overview**

# **A) Dimension Table Load Overview**

We have completed loading the data from the web service into the landing layer in our data analytics project. After that, we moved on to developing the reporting layer of the project. As part of this phase, we started with dimensional data modeling and successfully completed it. Through this process, we identified the list of reporting dimension and fact tables that need to be created.

Next, we set up an Azure SQL Database and created the reporting database within it. In this Azure SQL Database, we have already created one dimension table. Now, the next step is to develop the Data Factory transformation pipelines to load data into the reporting dimension tables. This is what we are going to start working on in this section. I’ll see you in the next lesson.

# **B) Dimension Table Load - Data Transformations Overview**

We have identified and set up several dimension tables and one fact table that need to be loaded to create our reporting database. Let’s begin by developing the pipeline for our first dimension table.

In a real-time project, you will typically receive a document called the Source to Target Mapping Document. This document contains the basic transformation rules that need to be applied while populating your dimension table. I have taken our first dimension table and included it in the Source to Target Mapping Document, along with all the details we have so far. Additionally, I’ve added some extra columns to this document, similar to what you would find in a real project.

For each column in the table, the document specifies the source location, and if the source is a file, it includes the source file name. It also indicates which source column needs to be mapped to the corresponding dimension table column, along with any transformations, filter conditions, or join conditions that need to be applied.
Let’s start filling out these details based on our understanding. We know that the source data comes from the landing container. We will not refer to the original HTTP web server source, because the purpose of the ingestion pipeline is to bring the source data into the data analytics platform. Therefore, all the data needed to develop our dimension table currently exists in the landing container.

We are going to read the data from the landing container’s daily pricing folder. While there are some datasets available in the labs folder for reference, the actual data for building our transformation pipeline will come from the landing/daily pricing folder. So, we can mention the source location as the landing container and the daily pricing folder in the Data Lake Storage account.

For now, we’ll refer to any one of the source file names, but in practice, we need to load data from all the source files into the dimension table. We’ll handle that part a little later—right now, we’ll work with a single file.

As mentioned earlier, any column highlighted with a specific background color indicates that its value is coming from the source file. So, we can copy the source column name directly as it is to maintain consistency in how each column is populated.

We have now seen how the DimState table is going to be populated. The goal here is to extract all the state name values from the source, identify the unique state name values, and load only those into the dimension table—excluding duplicates. In Excel, this would be done using the “Remove Duplicates” feature, and we’ll perform the same kind of operation using Data Factory transformations.

So, the transformation rule for the StateName column is to identify and load unique state name values from the source. The filter conditions are not applicable here because we are reading data from a single source, and join conditions aren’t relevant either since we aren’t joining multiple sources.
Next, for the StateID column, we will derive it while populating the reporting table. We’ve decided to generate a running number for each unique state name value. Therefore, there’s no direct source file or column for this — we’ll set the source location as “derived” and apply the transformation rule to generate unique IDs for each state.

For the VWCreatedDate and VWUpdatedDate columns, these are used for auditing purposes, allowing us to track when the records were loaded. We’ll map both these columns to the system date.

Now that we’ve identified all the requirements for loading the DimState table, we can move on to implementing this process in Azure Data Factory in the next lesson.

# **C) Dimension Table Load - Configure Source Dataset**

We have identified the transformation rules required to load the Dimension State table. So, let’s start implementing them in Azure Data Factory.

We know the process now — our source data exists in the Landing/Daily Pricing folder. The file named ProductWiseMarketWiseDailyReport_0101_2023 will serve as our source. Our sink will be the new dimension table that we created in the SQL Server database.

As per Azure standard practice, we need to create the dataset first. Since we are still exploring how to load this dimension table, we’ll create the dataset under the Working Labs folder before moving it to the final destination folder.

Right-click the Working Labs folder and create a new dataset. Our first dataset exists in the Data Lake Storage Gen2 account. Please note that now, our source is the landing layer — not the original source web service. That’s the main reason why we ingested all the data into the landing layer in the first place.

The landing layer is stored under the Azure Data Lake Storage Gen2 account, and our source files are located there. These files are delimited text files, so we’ll create the dataset accordingly and provide a meaningful name.

We have already created some datasets that point to the landing container, but those datasets were used as sink datasets in the ingestion pipelines. Now, we’re going to use this ingested data as the source for loading the reporting dimension table.

It’s better to create a new dataset with a proper naming convention. I’ve included “landing source” in the dataset name to make it clear. We can continue using the same linked service as before and browse through the files stored under landing/daily pricing/. For now, we’ll point to one specific file.

We also need to parameterize this dataset, and we already know how to do that. But before parameterizing, we’ll first experiment with how to design the transformation pipeline for loading this dimension table.

Now that we’ve created our source dataset, it’s important to import the schema from the source file. This step is crucial because we need access to the column names for mapping. For instance, according to our Source to Target Mapping Document, we need to read the StateName column from the source file. Without importing the schema, we won’t be able to reference that column.

To import the schema, after creating the dataset, click on “Clear” and then select “Import schema from connection/store”. This will automatically detect the first record as the header and bring in the column names as the schema. These represent the actual column names in the source file.

So, we’ve now created our source dataset that points to the file in the Landing/Daily Pricing folder.

Next, our sink dataset will point to the DimState table. Currently, we don’t yet have a linked service that connects to the new SQL Server database we created. So, the next step is to create a linked service for connecting to that database, and then we can create the sink dataset.

Although it’s possible to create the linked service while setting up the dataset, this time, we’ll use the Manage tab in Azure Data Factory. Under the Manage tab, there’s a section for Linked Services, where we can create a new one.

In the ingestion pipeline development earlier, we created both linked services directly while creating the datasets. But this time, we’ll explicitly create the linked service under the Manage → Linked Services section and then use it for our new sink dataset.

# **D) Dimension Table Load - Configure SQL Database Linked Services and Sink Dataset**

Let’s start by creating a new Linked Service to connect to the SQL Server database.

This time, we won’t be choosing Data Lake Storage or HTTP as the data source. Instead, we’ll look for Azure SQL Database, since that’s the database we created to load our reporting data.

Select Azure SQL Database as the connection type and provide a logical name for the linked service — for example, LinkService_AzureSQL_ReportingDB. This name clearly indicates that the linked service points to the reporting database.

From the Azure subscription, we’ll have only one option available, so choose that. Next, select the server name (which we already created) and then choose the database name.

For authentication, select SQL Authentication. You’ll need to enter the admin username and password that were configured when setting up the SQL Server database. Later, when configuring security settings between resources, we may change this authentication type, but for now, we’ll use SQL authentication to establish the connection.

After entering the credentials, perform a Test Connection to verify the configuration. If everything is set up correctly, the connection should be successful. Once confirmed, we have successfully created a new Linked Service to connect to the Azure SQL Reporting Database.

As soon as the linked service is created, make sure to publish the changes so that it’s saved and available for reuse in other datasets or pipelines.

Now, switch over to the Author tab and create a new dataset for our sink database table, which is the DimState table. For now, create this dataset under the Working Lab folder, so we can experiment with developing the pipeline before moving it to the final destination folder.

Since this dataset resides in the SQL Database, select Azure SQL Database as the dataset type (you can search by typing “SQL” or “Azure SQL”). Provide a meaningful name such as DimState_Lab, since we’ll be experimenting with the pipeline in the lab environment.

Next, point this dataset to the Linked Service (AzureSQL_ReportingDB) that we just created. The linked service will automatically display the list of tables in the connected database. Since we’ve created only one table — ReportingDimState — it will automatically be selected.

At this stage, it’s important to import the schema. Previously, when we were developing ingestion pipelines, importing the schema wasn’t necessary because we weren’t performing transformations at the individual column level. However, now we are working on column-level transformations, so having the schema is essential.

Importing the schema will allow the dataset to automatically detect the list of columns from the DimState table and include them in the dataset structure. This enables us to define specific transformation rules for each column and populate them correctly during the pipeline run.

Now that both the source and sink datasets have been created successfully, go ahead and publish all the changes.

In the next lesson, we’ll start building a new pipeline that reads data from the landing source file and loads it into the SQL Server database table.

# **E) Dimension Table Load - COPYDATA Limitations and Usage Requirement for DATAFLOW**

We have now created both our source and sink datasets. The next step is to create the pipeline that will load data into our sink database table using the source file located in the Landing/Daily Pricing folder.

Let’s start by giving the pipeline a meaningful name. In this case, we’ll name it Load_Reporting_Dim_Table_Lab, since we are working within the lab environment.

As we know, we can use the Copy Data activity to move data from one source to another sink. So, we’ll begin by using the Copy Data activity and configure it to perform the initial data transfer. Let’s give it a clear and descriptive name such as CopyData_Load_Dim_Table.

For the source, we’ll select the dataset that corresponds to Lab 4, as there’s only one file and one dataset pointing to that location. Then, for the sink, we’ll again search for Lab 4 and select the dataset that points to our Azure SQL Database table.

Once configured, you’ll notice that within the Copy Data activity, there’s an option to perform some mapping between source and sink columns. However, this activity doesn’t provide the flexibility to apply the transformation rules we identified earlier.

For instance, in the case of the StateName column, we need to identify the unique state names from the source file before loading them into the target. But the Copy Data activity only allows simple column mappings — it doesn’t let us apply custom transformation logic at the column level.

This limitation becomes even clearer when we consider columns like StateID, DWCreatedDate, and DWUpdatedDate. These columns don’t even exist in the source file — we need to derive their values based on the unique state names. However, the Copy Data activity doesn’t provide any mechanism to generate or transform such derived columns.

Although we can import schemas and automatically map matching columns from source to sink, it doesn’t help in this case. For example, since there’s no StateID in the source file, the activity won’t know how to populate that field. The same applies to DWCreatedDate and DWUpdatedDate — we must generate these values dynamically, which isn’t possible with Copy Data.

Therefore, the Copy Data activity is suitable only for straightforward 1-to-1 mappings, where every column in the sink has a corresponding column in the source and no additional transformations are needed. If your source already contains all the required columns with clean, ready-to-load data, then Copy Data works perfectly.

However, in our scenario, we require column-level transformations, such as generating unique IDs, removing duplicates, and deriving additional fields. This makes Copy Data insufficient for our use case.

In Azure Data Factory, there are only two activities that handle data movement — the Copy Data activity and the Data Flow activity. All other activities (like Set Variable, Lookup, or ForEach) act as supporting operations around these two.

So, it’s important to understand when to use Copy Data and when to use Data Flow:

(i) Use Copy Data when your source file contains all necessary columns and no transformations are required — just a direct transfer from source to sink.

(ii) Use Data Flow when you need to apply transformations, derive new columns, or perform logic at the individual column level.

In this particular case, since our data requires transformations such as identifying unique states and generating new columns like StateID, we must use the Data Flow activity. The Copy Data activity will not work for this scenario.

In the next lesson, we’ll start exploring how to configure and use the Data Flow activity to implement these transformations effectively.

# **F) Dimension Table Load - DATAFLOW Overview**

We have identified that we won’t be able to use the Copy Data activity to perform the necessary transformations required for loading the DimState table. Therefore, we need to use another Move and Transform activity called Data Flow to perform the necessary transformations for loading data from the source file into the DimState dimension table.

So, we will bring the Data Flow activity into the pipeline design. However, I would like to keep the Copy Data activity for some time so that I can explain some quick differences between the Copy Data activity and Data Flow, helping you understand when to use Data Flow and when to use Copy Data.

Next, I will give a reasonable name for the Data Flow activity — Load Dimension Tables. As soon as we go to the Settings section of the Data Flow activity, it opens another design interface known as the Data Flow Canvas. This is likely the last new user interface we will be learning, but it is an important one since we will be developing the actual transformation logic here using the Data Flow.

When you click New, it opens a completely different design interface — the Data Flow Canvas. The Data Flow activity that you add inside the pipeline is simply calling a data flow object. You are actually creating the data flow itself when you click New.

Along with the pipeline, this Data Flow design interface is entirely separate from the pipeline interface. If you want to call a data flow from the pipeline, you use the Data Flow Activity. The Data Flow itself is an independent component, much like a dataset. If you look at the structure in Azure Data Factory, you’ll notice that Data Flows have their own dedicated folder — meaning you can even create them independently.

When calling from the pipeline, we need to use the Data Flow Activity, but for the first time, we’ll create a new Data Flow from within it. We’ll follow proper naming conventions, keeping everything consistent for Lab 4, which involves loading the reporting dimension table. Therefore, I will name it DF_Load_Reporting_DimStateTable_Lab4. We’ll maintain Lab4 as a common tag across all our components for this lab.

Inside the Data Flow Canvas, you have a range of transformations available to perform additional data processing steps. The first task, or transformation, within a data flow is adding a source. Without defining a source, you cannot perform any transformations inside the data flow.

When you click the Add Source button (represented by a plus or arrow icon), it allows you to add your data source. After clicking Add Source, similar to the pipeline interface, the settings window will appear at the bottom. This bottom panel shows configuration settings for the currently selected transformation — in this case, the Source transformation.

Here, there are some naming restrictions — you cannot use spaces, underscores, or hyphens. The name must be a single continuous string. For example, you could name it SourceReadDailyPricingData to keep it logical and clear.

Next, under Source Type, you have an option to choose between Dataset or Inline Dataset. The good thing is that you can reuse the same datasets that are already used in your pipeline. The Dataset is a common component between the pipeline and the data flow.

You can select an existing dataset by choosing the Dataset option, or you can create one on the fly by selecting Inline. For now, we’ll use an existing dataset that we have already created for Lab 4. When we select it, all the datasets available for Lab 4 will be displayed. The ADLS dataset is the first one we will use to read data from the source file.

Once you choose your dataset, navigate to the Projection option. This section displays all the columns present in the dataset schema because it reads the schema directly from the dataset definition. If you open our source dataset schema, you will notice that these same columns appear in the Projection tab.

Apart from that, there are a few additional options, such as Allow Schema Drift. For instance, suppose our current source file contains 12 columns, but in the next file received from the source, there’s an additional column. If we enable Allow Schema Drift, the data flow will still be able to read that file without failing due to the schema change.

There are some other settings as well, but they aren’t directly relevant to our use case right now, so we’ll leave them as default. For now, our focus will be on the Source Settings and Projection options.

In the next step, we’ll apply transformations on the State Name column to identify and extract unique values from the source file — which we will cover in the next lesson.

# **G) Dimension Table Load - DATAFLOW SELECT Transformation**

As I mentioned earlier, there are some additional options available in the Data Flow settings, but we will revisit them later in the course when we discuss performance tuning and defining user-derived columns.

For now, the most useful feature for developers during the early stages of building data flows is the Data Preview option.

While developing, the Data Preview allows you to view the actual data being read from your source file. To enable Data Preview, you must turn on the Debug Cluster. This cluster runs in the background to execute your data flow logic in real time and display preview results. However, if you are not actively using it, it’s recommended to keep it disabled, as it runs for about an hour and can be a bit costly in terms of resources. But while learning, it’s extremely useful because it lets you instantly see the output after each transformation you apply.

From our source file, we only need the State Name column. We don’t require any of the other columns. Before applying the transformation rule to identify unique state names, we’ll first exclude all the unnecessary columns. Keeping only the required column will improve performance and reduce memory consumption during execution. Unused columns consume additional memory space and can slow down the Data Flow job.

To perform these kinds of operations, Azure Data Factory provides a variety of predefined transformations within the Data Flow. While the pipeline handles activities at a higher level (like movement or orchestration), the Data Flow deals with transformations at the column level.

In our case, since we only want to select the State Name column from the source schema, we’ll use a transformation from the Schema Modifier category — the Select transformation. You can add a transformation by clicking the plus (+) icon next to the previous step, which will display a list of available transformations. From that list, choose the Select transformation, and it will appear next to your source transformation in the flow.

Once you select it, the configuration options for the Select transformation will appear in the settings panel at the bottom of the screen. Here, we’ll give a logical name to the transformation and choose the State Name column from the list of available source columns. The Select transformation displays all columns from the source dataset, and we can either deselect all and then check only the State Name column, or manually delete the others one by one.

After this, we can use the Inspect tab to review the columns that will move forward to the next stage of the data flow. Initially, in the source transformation, we can use the Projection tab to view all columns available in the source schema. But going forward, as we build transformations, the Inspect tab becomes more relevant—it shows the columns that will be passed from one transformation to the next.

If we now look at the Inspect tab after applying the Select transformation, it will show only the State Name column from the source, confirming that all unnecessary columns have been excluded.

Next, we need to apply a transformation to identify unique state name values from the source data. Currently, if we preview the output of the Select transformation, it displays all state names as they appear in the source file, including duplicates. Our next goal is to remove these duplicates and extract only the distinct state names.

We will implement the transformation logic for identifying unique State Name values in the next lesson, right before mapping the results into the DimState dimension table in the sink.

# **H) Dimension Table Load - DATAFLOW AGGREGATE Transformation**

In our next step, we need to identify the unique state name values from the list of state names present in our source file. The data already exists in our landing container as a CSV file. If this data were in a database, we could easily use a SQL query with the DISTINCT clause to identify the unique state names. However, since our source is a file, we need to find a workaround to achieve the same result within Azure Data Factory (ADF).

In the source CSV file, there are multiple duplicate state name values, and our goal is to extract only the unique state names from them. To accomplish this, we can use a counting technique that helps us identify how many times each state name appears.

If we calculate the count of state name values, the result will show each unique state name along with the number of times it appears in the source data. Essentially, this means that ADF will internally sort the column containing state names and then apply a running count for each state until the name changes. Once a new state name appears, the counter resets and starts again.
For example, when we apply this logic using the Aggregator Transformation in Azure Data Factory, the output will display two columns — state_name and count_of_state_name.

For instance, Andhra Pradesh might appear 53 times in the source file.

Similarly, another state might appear 118 times, and so on.

Instead of repeating each state multiple times, the Aggregator Transformation outputs each unique state name once along with its count. In this way, we can identify unique state names from a flat file, which is a commonly used technique in data analytics projects when the source is a file rather than a database.
To implement this in Azure Data Factory, we will now use the Aggregator Transformation. Currently, the data flowing from the previous transformation still contains duplicate state names, as we haven’t yet applied the aggregation logic. So, the next step is to add an Aggregator transformation to the data flow.
You can find the Aggregator Transformation under the Schema Modifier category because it modifies the structure of the data by introducing new columns into the output. We’ll add the transformation and give it a logical name — for example, Aggregate_Count.
Each transformation in ADF has specific configuration options, and it’s important to understand what each setting does.

In the Select Transformation, we removed all unnecessary columns and retained only state_name.

In the Aggregator Transformation, we’ll configure two key sections — Group By and Aggregate.

In the Group By section, we’ll specify which column to group the data by. In our case, it’s the state_name column, as we want to aggregate records based on each distinct state name.
Next, in the Aggregate section, we’ll create a new output column. We can name it count_state_name and then define its calculation logic. This is where we’ll use the Data Flow Expression Builder to define our expression.

We’ve previously learned about the Pipeline Expression Builder while working with the Copy Data Activity in ADF pipelines. However, the Data Flow Expression Builder is slightly different — it is specifically designed to handle expressions and logic at the data transformation level within a Data Flow.
In the next lesson, we will explore this Data Flow Expression Builder in detail and learn how to use it effectively to define our aggregation logic for counting unique state names.

# **I) Dimension Table Load - DATAFLOW EXPRESSION BUILDER Overview**

In this lecture, we have applied a group by column as the state name, based on which we need to identify how many times that particular state is appearing in the source file. Now, we are going to set the actual expression to count the state names. If you open the expression builder, you will notice that this is the Data Flow Expression Builder, which is entirely different from the Pipeline Expression Builder. It has a different interface, and again, you can create expressions here in the expression elements section. The functions also exist here, but they are a different set of functions compared to the pipeline expressions.

If you click the Input Schema, it will display the column names coming from the source file. And if you click the Parameters tab, it will display the Data Flow parameters, not the pipeline parameters such as dataset parameters. The data flow itself also has parameters, and the last three options in the panel will be explored later. For now, we are primarily interested in finding the function to count the state name. It is better to use the search functionality so that the relevant function appears quickly. If you search for the count function, it will start to appear in the expression, similar to how it works in the Pipeline Expression Builder.

Now, you need to choose the input column name. There is a provision here to select it from the input schema. However, since you are searching for the count function, you need to remove the search string; otherwise, the input schema won’t appear because all items are displayed in one output window. Based on that, you can choose accordingly. When you select “function,” it displays only the functions, and when you select “input schema,” it displays only the input schema. But since you are searching for the count function and that exact name does not exist in the input schema, it won’t display it. Therefore, you should keep searching and removing the search string as necessary; otherwise, you may get a little confused here.

Now, we need to count the number of times each state name appears. By mistake, I removed one of the opening brackets, so be careful — these expressions are slightly different from the pipeline expressions we used earlier in the copy data activity. Once your expression is properly set, click Save and Finish. If you then look at the Inspect button, you will see there are now two columns. Initially, we had only one column because we deleted all of the source columns earlier. Now, there is one column coming from the source and one additional column that we created for the count of state names.

The good thing about Data Preview is that it allows you to verify whether your logic is working correctly or not, right there in the editor itself. You can click Refresh, and it will apply your logic to produce and display the output of this transformation. As we can see, it has properly counted the number of times each state appears and brought out the unique state names. Comparing this with the data preview from the source, you can see that, for example, Uttar Pradesh was appearing multiple times in the source file, but the output of the Aggregator Transformation now displays it only once with the corresponding count. Everything is now working as expected.

With that, we have completed the first transformation rule — identifying the unique state names. The next step is to allocate a unique ID for each of these unique state name values. However, before that, we need to remove the “count of state name” column because it will not be used in our sink table. We included it only because the Aggregate Transformation requires at least one aggregate function to work. The aggregator can be used for other purposes as well — for example, if you want to calculate the sum of quantities of arrivals for a specific product in a specific state, you can use the aggregate transformation to summarize all those values.

So, the aggregate transformation can be used in multiple ways to summarize and group data, but in this case, we used it to identify the unique state names. Since we no longer need the “count of state name” column, we will exclude it. To do that, we use the Select Transformation once again. When you click on the select transformation, it displays the two column names. You can quickly delete the “count of state name” column because we no longer need it for loading into the target table. So, we are excluding that column.

After excluding it, if you look at the Data Preview again, you will see only the state name column appearing. Similarly, in the Inspect tab, the other column is excluded, and everything still looks good to load into the target table. Our next transformation step will be to allocate a unique ID for each of the unique state name values that we have identified. We will derive that in the next lesson.

# **J) Dimension Table Load - DATAFLOW SURROGATE KEY Transformation**

Now the task is to allocate a unique ID for each of the state name values. For example, the first state name, starting with Uttar Pradesh, should be allocated the value 1, the next state name should get 2, the next should get 3, then 4, 5, and so on, continuing in that order until the last state name. That’s the requirement here.

To achieve this, you need to understand the concept of transformations available within the data flow. Remember, we are not going to write any code manually here as we did in the pipelines. Instead, we simply configure the existing transformations available in the data flow. However, some transformations may have certain limitations, and in those cases, we need to find appropriate workarounds. One such case is when we need to create a surrogate key — in this context, the state ID.

If you recall, while performing logical data modeling, one of the steps we followed was to add surrogate keys to all dimension tables. These IDs act as surrogate keys — unique identifiers for each record in a dimension table. In Data Flow, there is a built-in transformation available specifically for this purpose. It automatically generates unique ID values for every row that passes through the transformation. Hence, we are going to use this transformation, which is called the Surrogate Key Transformation, to generate our State ID values.

So, we will configure the Surrogate Key Transformation and give it a suitable name like Generate State ID Value. There are some default configuration options and description fields available in the properties panel, but for now, we will skip those and focus only on the properties that are specific to our current transformation. We can always revisit and adjust the default settings later if necessary.

The Surrogate Key Transformation will take the incoming stream from whichever previous transformation is connected to it — in our case, the output from the Select Transformation that carries the unique state names. Next, we need to specify the key column name. If you observe carefully, we do not have any existing column name in the dataset to map to the state ID column in our dimension state table, because this is a new value we are going to derive. Therefore, we can give the same name, state_id, so that it will be easier to map it to the final dimension table during the sink configuration.

Now, we can specify the Start Value and Step Value for generating these surrogate keys. You can start the numbering from any value you prefer. Typically, we start from 1, so we’ll set the start value as 1. The Step Value determines the increment for each subsequent record. For example, if the step value is 10, the first record will have a key of 1, the next record will have 11 (1 + 10), and the next will have 21 (11 + 10), and so on. However, that’s not what we want here — we need each record to increment sequentially by 1. So, we’ll set the Step Value as 1.

As you configure these properties, you can keep an eye on the Inspect Tab, which dynamically displays the columns being modified or added in each transformation. This helps you verify that your configuration is being applied correctly. Once you’ve set everything up, you can open the Data Preview to confirm that the surrogate key transformation is working as intended.

When you refresh the data preview, you’ll see that it’s generating unique surrogate State ID values for each of the unique state names passing through. You can even count and verify — for example, if there are 23 states in the source file, you will see 23 unique state IDs generated, each corresponding to a unique state name. This confirms that the transformation is working perfectly.

Now that the State ID values have been successfully created, the next step is to derive two additional columns — DW_Created_Date and DW_Updated_Date. These are straightforward to derive and will be implemented in the next lesson.

# **K) Dimension Table Load - DATAFLOW DERIVED COLUMN and SINK Transformation**

We have mapped these audit columns. We call them audit columns because they allow us to audit the data that is loaded into the reporting database. Both of these columns are pointing to the system data existing in Azure Data Factory. However, this data is not in the same format — it exists in UTC format. We can change this mapping later if required.

Our current task is to create two new columns in our data flow and assign system date values to these new columns. Essentially, we are deriving these columns. Earlier, we created new columns using a surrogate key, where we performed specific operations to generate them. But in this case, we just need to create two new columns and directly assign values to them.

For such straightforward column creation, there is a transformation called Derived Column in Azure Data Factory. Using the Derived Column transformation, we can create any number of columns and assign expressions to them using the Data Flow Expression Builder.

Here, we are going to create two derived columns for the audit process. The first column is DW_Create_Date. We need to assign the system date value representing the time when the specific record is loaded into the database table. For this, we will use the system date function. So, we will search for any available date and time functions and use currentDate(), as that is the one closest to what we need. If any errors occur, we can come back and fix them later.

After mapping the first column to the current date value coming from the data flow, we will create one more column. Click Add Column and name it DW_Updated_Date. Again, assign the same expression (currentDate()) to this column. You can either copy and paste the expression or open the Expression Builder and paste it there. If you paste it, it should work fine. This is a very simple process.

Now we have included two additional columns. If you look at the data flow now, we have all the source columns needed for mapping into the Dim_State table. All four columns have been derived successfully, and now we can populate this data into the sink.

A data flow must have at least one source and one sink. The sink here is where the transformed data will be written. In this case, we have split the source and sink operations. They are not present in the same place, unlike the Copy Data activity. Here, we start with the source, apply all the necessary transformations at the column level, and then map the data to the sink.

As soon as you click the sink, it asks you to map it to a dataset. There are multiple dataset options available, but for now, we will go with the standard dataset. Select the sink dataset named Sink_Dim_State, which we have already created to point to our Dim_State table. It was created earlier under Lab 4.

If you click on that and go to the Settings section, it asks whether you want to insert, delete existing data, or perform an upsert (update existing records). We will explore all these options later. For now, we do not want to recreate the table since it already exists, so we won’t apply any of these changes.

Next, we move to the Error section. If any of the source data does not meet the target database’s data type or schema requirements, you can choose to redirect those error records elsewhere, stop the data flow, or continue on error. This is where we configure error handling to ensure that any data mismatches or type conflicts are properly handled.

One of the most important configurations right now is the Mapping section. We need to ensure that the source columns coming out of the final transformation match exactly with the column names in the target table. If the names are the same, Azure Data Factory will automatically perform the column mapping.

To verify this, you can uncheck Auto Mapping. This will display the mapping that has been automatically applied. Since our source column names from the transformations match the target table columns, they have been mapped automatically. The target table columns have been identified from the sink dataset, and everything looks good.

Once all of this is verified, click Publish All to save all your code and configurations into the Data Factory repository. However, since we still have the Copy Data activity in our pipeline, it might throw an error during publishing because some of the columns cannot be mapped in the copy data activity.

To fix this, delete the Copy Data activity since we no longer need it. After deleting it, perform Publish All again. This time, all changes will be successfully stored in the repository.

Now that publishing is complete, the next step is to run the pipeline to ensure that the source data is properly transformed and loaded into the SQL Server database. We will perform this step in the next lesson.

# **L) Dimension Table Load - Recap DATAFLOW Transformations & Debugging DATAFLOW**

Let us start debugging this pipeline. First, we will close all unnecessary windows to focus on our work. This is the main pipeline where we created our data flow. Data flows in Azure Data Factory can be created independently, similar to how we create datasets. However, for the first time, we created this data flow using the Data Flow Activity directly within the pipeline by clicking the New button. This action opened the Data Flow Design Window, also known as the canvas.

Now, we can open the same data flow from the pipeline. In Azure Data Factory, every data flow must have at least one source and one sink. Without these, the data flow will not be validated successfully. In most cases, data flows also include several transformations that must be performed on the data between the source and sink.

We identified our transformation rules from the source-to-target mapping document. Based on that, we started by extracting only the State Name column from the source file. For this, we used an existing transformation called Select. Then, we applied an Aggregate Transformation to identify the unique state name values from the source data. By applying a count of state names as an aggregate function, we were able to obtain the distinct state name values.

Next, we used another Select Transformation, which works similarly to the first one, to remove the additional column that was created in the aggregate transformation. After that, we added a Surrogate Key Transformation to generate a running ID for each of the unique state name values. This transformation automatically creates a new ID column value for each record passing through it.

The last transformation step involved deriving two audit columns — DW_Create_Date and DW_Updated_Date. These columns were added to align with the structure of our dimension table. Once this was done, we created our sink, which points to the SQL Server database. All the transformed columns from the previous steps were mapped correctly to the sink columns in the target table.

Now, when we click Debug, it uses the existing Data Flow Debug Session. It’s important to note that, in Azure Data Factory, data flow components cannot be executed individually at the transformation level. You can preview the data at each transformation using Data Preview, but that only helps you verify whether your transformations are functioning correctly — it doesn’t load any data into the sink.

To actually execute and load data, you must use the Data Flow Activity within the pipeline, link it to your developed data flow, and then run the pipeline. Once the pipeline runs, you can monitor its progress from the Pipeline Output section.

During execution, the run details at each stage are displayed. If you look at them closely, you will see all the transformations used, starting with the source. The source reads the input file containing 12,877 records, which seems accurate. We can cross-check this, and indeed, it reads 12,877 records since the first row is a header containing column names — that’s absolutely correct.

In the next stage, the same number of records (12,877) pass through, but only the State Name column is carried forward. Then, the aggregate stage processes the data and calculates 25 unique state names. We can later explore the partition chart and related details, but for now, our goal is to ensure that the data flow development process is clear.

The next stage removes the count column generated by the aggregate transformation, and then the surrogate key transformation assigns unique ID values to each of the 25 state name records. Following that, the derived column transformation creates the two audit columns — DW_Create_Date and DW_Updated_Date.

Finally, in the Sink stage, the transformed data is successfully loaded into the target table — a total of 25 rows are inserted into the SQL Server database. Everything appears to be working correctly.

Now, to confirm the results, we can go to the SQL Server database and verify whether the data is loaded properly. Open the Home section and access the SQL Server Reporting Database that we created earlier. You can quickly check the data using the Query Editor. For authentication, use Microsoft Entra Authentication, which eliminates the need to enter passwords manually.

Once connected, navigate to the Dim_State table to view the loaded data. You can write your own SQL query to check it. For example, run:

SELECT * FROM reporting.dim_state;

This query retrieves all records from the table. The data is loaded correctly — we can see 25 unique state name values, each with a unique state ID. Everything looks good and as expected.

Now that the data flow is running successfully and the data is verified, our next step will be to make this data flow stable. In the next lesson, we will rerun the pipeline using another source file from our Data Lake Storage Account and observe the behavior.

# **M) Dimension Table Load - Change Data Capture (CDC) Overview**

When we complete our data flow development and get it ready for daily execution, it should not run for only one specific source file. As of now, we have not yet parameterized our source file. In our landing folder, under the daily pricing directory, there is not just the 1st of January file — there are several files already available, and more files will continue to arrive over time. Therefore, our data flow needs to run for each of these incoming source files and consistently produce the output in the SQL Server table.

An important aspect of this setup is that the data flow must not load any duplicate state name values into the table. This is a critical principle in dimensional data modeling, because the keys in the dimension table are mapped back to the fact tables. The linking between the dimension and fact tables happens exclusively through these ID column values. Hence, it’s crucial that no duplicate records exist in the dimension table, as this would compromise data integrity and cause incorrect relationships in reporting.

Now, let’s proceed to test this by passing the 2nd of January file and rerunning the pipeline. We will first publish the changes for the time being. At this stage, it is still part of the Lab 4 or Lab 5 pipeline, and we still have time to develop the complete pipeline. The only change made now is switching the source file from 1st of January to 2nd of January.

When we run the pipeline, ideally, it should not create any duplicate state name values. Otherwise, it will lead to unnecessary issues. Let’s execute the pipeline and observe what happens. The pipeline runs successfully, and now we will quickly check the data in the SQL Server database for the Dim_State table.

To verify the result properly, we will order the rows by the State_ID column so that we can easily spot any duplicate values. Upon checking, it looks like some duplicate records have been loaded because the total number of records now exceeds 25. To confirm this, we can use the ORDER BY clause in our SQL query to sort the results by the State_ID column and inspect the data.

After running the query, we can clearly see that duplicate values for the same state have been generated. This is not the expected behavior. The reason for this issue is that we did not handle the scenario for existing records within the data flow.

If we look back at our data flow, we simply changed the source file from 1st January 2023 to 2nd January 2023. This means that the data flow read all the state names from that file, calculated the unique state name values within that file, generated surrogate IDs for them, derived audit columns, and then loaded everything into the sink table. However, there is no validation step that checks whether the state name values coming from the new source file already exist in the target table.

What we need to do is ensure that before loading data into the sink, the data flow verifies whether each state name value from the source already exists in the target table (Dim_State). If it exists, it should not be reloaded, because in our dimension table, there must be one unique state name mapped to one unique state ID value. This rule is fundamental to maintaining data consistency in dimensional data modeling.

If duplicate data is inserted into the dimension table, it will completely compromise data integrity in the reporting database. To prevent this, we need to add logic in our data flow to check if each incoming state name from the source already exists in the target table before performing the insert.

In other words, we must read the sink table (i.e., the existing target table in SQL Server) as an additional source in the data flow. Without reading the sink table as a source, we cannot compare and identify whether a state name coming from the source file already exists in the target table. The Sink Transformation itself cannot be used for this comparison, as it is designed only for writing data — not for reading or referencing existing records.

Therefore, to implement this logic, we will use the sink table as an additional source in the data flow. We will then perform a comparison between the state name values coming from the source file and those already present in the sink table. This comparison will help ensure that only new, unique state names are loaded, and duplicates are avoided.

We will carry out this enhancement by adding an additional source and an additional transformation in the next lesson.

# **N) Dimension Table Load - Change Data Capture Add Sink Data Into Source Stream**

To stop loading duplicate records into our Dim_State table, we need to read the existing state name values from our sink table. To achieve this, we must first create a new dataset. Although we already have a dataset connected to the Dim_State table, that dataset was specifically created for loading data into the Dim_State table. However, when we want to read data from this same table, we need to create a separate dataset. This is because the configuration settings used when reading data as a source differ from those used when writing data as a sink.

Therefore, I am going to create a new dataset for the same Dim_State table. To clearly differentiate between the two, I will follow a naming convention that makes it obvious whether the dataset is used as a source or as a sink. For example, since this dataset is meant for reading existing data, I will name it something like “report_dim_state_source_lab4.” This dataset will connect to the Azure SQL Database and will be used to check whether the state names already exist in the target table.

Once the new source dataset for the sink table is created, we can return to the data flow. Within the data flow, we can add multiple sources, so we will now add this new source, which I’ll call “source_dim_state_lookup.” This source will use the new dataset we just created. As a result, we now have two datasets that point to the same table — one for loading (sink) and another for reading (source).

After adding the source, we can go to the Projection or Inspect window to confirm that it has successfully imported the column names from the dataset. Now that it’s connected, we have state name values coming from both sides — the source file and the sink table (lookup source).

To avoid confusion in the design and to keep the columns clearly distinguishable, we should rename the column coming from the lookup table. Additionally, from the target table, we don’t need all columns — we only need the state name column to perform the comparison. For this purpose, we will use a Select Transformation.

Let’s call this transformation “Select_Dim_State_Lookup.” In the description, we can note that this transformation is used for lookup purposes. Within this transformation, we will select only the State_Name column from the sink table and delete the rest. Then, we’ll rename this column to “lookup_state_name.”

It’s important to understand that we are not changing the actual column name in the source table; we are only renaming it inside the data flow to make our design easier to follow. Essentially, the renamed column lookup_state_name still points to the State_Name column in the sink table, but the name change helps differentiate it from the State_Name column coming from the source file.

The Select Transformation is not only useful for removing columns but also for renaming columns — especially when multiple sources contain columns with the same name. This way, we can avoid conflicts when merging or comparing data from different sources.

At this stage, we have two separate streams in our data flow — one coming from the source file and the other from the sink (lookup) table. If we press the preview button for the lookup stream, it will display all of the existing (and currently duplicate) records from the target table.

However, these two streams are currently separate. Without merging them, we cannot compare the state names from the source file with those from the target table to identify duplicates. Therefore, the next step is to merge these two streams so that we can perform the comparison.

Before we proceed with the merge, we need to clean up the data in the target table because it currently contains duplicate records. To start fresh, we will truncate the target table. Go to the SQL Server database and run the following SQL statement:

TRUNCATE TABLE [reporting].[Dim_State];

This command removes all the records from the target table. Be cautious when running SQL commands like this — always double-check before executing to avoid accidentally deleting important data. A good practice is to temporarily comment out any SQL statements that you don’t want to execute immediately.

Once you run the truncate command, you can verify that the table is empty by executing:

SELECT * FROM [reporting].[Dim_State];

This should return no records. Similarly, if you refresh the data preview in your data flow source, make sure to click Refresh from Source rather than just Refresh, because the regular refresh might still show cached data.

Now that the target table is empty, we are ready to proceed. The source file contains new state name values, and everything looks good. Our next step is to merge the two source streams (the one from the source file and the one from the lookup table). Without merging them, we cannot perform the necessary comparison between the two datasets.

We will accomplish this merging process and perform the comparison logic in the next lesson.

# **O) Dimension Table Load - Change Data Capture LOOKUP Transformation**

Now I need to identify the new transformation that can join these two sources — one coming from our original source file and the other from our sink table. I need to compare whether the source state name is already existing in the sink table or not. For that, I am reading the data from my sink table. For the time being, it’s null — there’s no data there — but still, it will work. So, we are going to include one more transformation before the surrogate key. Specifically, why I am including it before the surrogate key is because surrogate keys need to be generated only for the state names that are going to be inserted into the sink table. From before the surrogate key itself, I can filter out any state names already existing in the sink table. Then we don’t need to do any further actions. That’s why I am including this before the surrogate key.

I am clicking this button, and there are a couple of transformations available for merging multiple inputs and multiple outputs. In our case, it is multiple inputs. You can use these available transformations to merge the two datasets. Specifically, we can use the Join transformation because Join will join two datasets — the name itself implies that it can merge the two datasets. The other thing we can do is use the Lookup transformation. The difference is that the Join transformation will match based on the join type — the two datasets are merged based on matching rows — but in Lookup, irrespective of whether a record exists between the two sources, all of them will be merged, and if no record is present, it will come as a null value from one of the streams.

So, I am not going to use Join; instead, I am going to use the Lookup transformation. In this instance, we will explore all of them — multiple input and multiple output transformations — so don’t worry. For now, I need to merge these two sources: one is coming from the source file, and the other is coming from the sink table. Irrespective of any record existing in either of these, if a record is not existing in one of the sources, that value needs to come as null.

So, I am going to include the Lookup transformation here. As this is a multiple input transformation, it will ask us to configure two inputs and also ask us to specify the condition for how to merge both of these inputs. So, I am naming this as Lookup_StateName, because we are looking up the actual state name value. As I said, the primary stream has to be included here — it automatically connects from the source file transformation output. This is the primary stream. I need to compare this primary stream against the lookup stream — and for this purpose only, we created the Select DimState Lookup, the new source we created earlier. In the Select transformation, we excluded unnecessary columns.

So this is the one that needs to be the lookup stream, and from this, you need to choose appropriately. That’s why I included the word “lookup” in the naming conventions on the Select transformation — to make it clear. Now, it’s asking if multiple rows match between these two sources, do we need to match all or only match on any row? It should be fine to enable the multiple match rows option, because if we load the data properly, there will only be one record existing in the target table. It can match on any row for the time being, so we can leave these two settings as default.

Now it’s asking for the lookup condition — on what basis do I need to merge these two datasets? The common column name between these two sources is the state name. From the main source stream, we have the state name, and the same state name value is also appearing in the sink table. But to differentiate the state name inside the code, we renamed it to lookup_state_name. So now it is matching between these two sources.

If you come to the Inspect Output, it shows both the state_name and lookup_state_name columns. If you look at the Data Preview, and refresh it, it is reading the data from the 2nd of January file. Please note that we mapped it to the 2nd of January file. Probably we can switch it back to the 1st of January file so that we can start it as a fresh run. If you refresh it, it will read the data from our source file. Our source file has data, but our sink table does not — because we truncated the data earlier, since erroneous data was loaded in the previous step.

So, the lookup_state_name is coming as null. That means this source state name value does not exist in the target table. These records can be passed after this Lookup transformation to load them into the sink table. To filter out only these records, we need to use an additional transformation called Filter Transformation. We will configure the filter transformation in the next lesson.

# **P) Dimension Table Load - Change Data Capture FILTER Transformation**

In this lookup transformation, we have configured two streams — one is the stream coming from the source file, and the other is the stream coming from the sink target table. We are matching these two datasets based on the state name column that exists in both the source and the sink. If you look at the data preview, whenever the lookup state name value is null, that means this record is coming from the target table. In other words, this state name is not yet loaded in the sink table. These records need to be filtered out and passed to the subsequent transformations to generate the surrogate ID, created date, and updated date columns.

To filter out only these records, we are going to use another transformation called the Filter transformation. The Filter transformation exists under the Row Modifier category. It determines whether a specific row should be passed through or not, which is why it is called a row modifier. We are going to filter the new state name values coming from the source using the Filter transformation. Inside the Expression Editor, when we open the Expression Builder, the Data Flow Expression Builder interface appears.

Now, we need to apply the condition that checks whether the lookup state name column is null. This means we are verifying whether the lookup (from the sink) did not find a match for a particular source state name. If the lookup state name column is null, it indicates that the corresponding state name does not exist in the sink table and thus needs to be passed forward for loading into the target table. This ensures that duplicate records will not be loaded again.

In the Filter settings, when you open the Expression Builder, you can search for the isNull function to check for null values. Once you find it, click on isNull, and then specify the column name you want to check. After that, delete the function search and go to the Input Schema section where you can see the actual column names coming into the Filter transformation. Here, we need to check against the isNull of our sink state name values — which we have defined as the lookup state name column. Once this is done, click Save and Finish.

If you then check the Data Preview, in this current instance it will pass through all of the state name values because our target table currently does not have any data. Once we have loaded the data, if we come back and check again, the Data Preview will show that no state name values are passed through, since they already exist in the sink. Everything looks good and is working fine.

After the Filter stream, we will need to include the Surrogate ID generation for the state names that are identified to be loaded. Then, we can publish the changes. Now we can start running the pipeline again. Currently, it is still pointing to the file dated 01-01-2023, but soon we will parameterize this value so that during runtime it will dynamically ask for the date instead of manually changing it in the dataset. We are already familiar with parameterization, but for now, we are focusing on understanding the complexity within the Data Flow itself before parameterizing everything. The goal here is to first introduce and master different transformations available in the data flow before moving on to the proper pipeline development.

Now, let’s run the pipeline again. Since there is currently no data in the target table, the first run will load all of the state name values. If we run it a second time, it will not load any duplicate state name values — this is the expected behavior based on the logic we have implemented using the Lookup and Filter transformations. The pipeline ran successfully. We can quickly check the database server to confirm whether the data has been loaded into the final target table.

There are 25 state names that have been loaded, which looks good. Now, to further test, we will rerun the pipeline with the next day’s source file. For that, we will change the source file name in the dataset from 0101_2023 to 0102_2023. After updating it, we publish the changes and rerun the pipeline. This time, it should not load any duplicate records because we have already implemented protection by comparing the source and sink datasets. After running the pipeline again, it completed successfully. Checking the target database table confirms that there are still only 25 rows, which means no duplicate records were inserted.

This proves that our logic and configuration are working as intended. We are gradually improving our data flow development skills to handle various real-world scenarios. Initially, we mapped and performed all the transformations required for the sink table. Now, we have added additional protection to ensure no duplicates are loaded, which is crucial since this pipeline will run daily. There is only one more issue remaining in this data flow, but apart from that, it is fully ready to be converted into a real-time data flow. We will address that remaining issue in the next lesson.

# **Q) Dimension Table Load - Change Data Capture SURROGATE KEY Limitation**

I went back to my SQL Server database and verified that I have 25 state names loaded from both the first of January file and the second of January file. Now, I want to simulate a real-time scenario that you would typically encounter in an actual project. For example, during the first day’s file load, let’s assume that two specific state names did not get loaded, so we can test our logic thoroughly.

To simulate this situation, I will delete those two records from the target table. This will help recreate the scenario where the next day’s file needs to pick up and load only those missing records. While executing a delete command, we need to be extremely careful—because if we forget to include a WHERE condition, it would behave like a truncate operation and remove all the records from the table. So, to be safe, I’ll execute a query like:
DELETE FROM [target_table] WHERE state_id IN (24, 25);
This will delete only those two specific records so that when I rerun the pipeline, I can confidently verify that the logic correctly identifies and loads these missing state names into the SQL Server database.

These types of test simulations are very important in real-time projects. During development, we rarely have access to complete or perfect datasets, so it’s essential to perform such small data adjustments to make sure our logic works as expected. That’s exactly what I’m doing here — testing the robustness of the logic. After deleting those two records, my target table now has only 23 state names. It’s a good practice to always comment out truncate or delete statements in your SQL editor once executed to avoid accidentally re-running them later.

Now, the target table has 23 records, and we know that the two missing state names exist in the second January file. When we rerun the pipeline, it should ideally load only those two missing state names, assigning them the next state_id values of 24 and 25. So, I ran the pipeline again to verify this behavior.

The pipeline ran successfully, and when I went back to the SQL Server database and checked, I could see that the two deleted state names were indeed reloaded. However, there was a problem. Even though the two missing state names were loaded correctly, the state_id values generated for them were 1 and 2 instead of 24 and 25. This issue occurs because, in the data flow, we are using a Surrogate Key Generator to create surrogate IDs for the state_id field. The surrogate key generator always starts from the configured start value for each new run. It does not remember or continue from the last maximum value in the target table.

So, even though the logic correctly identified and passed only the two missing state names, the surrogate key generator still began assigning IDs from 1, resulting in incorrect values. This is a known limitation of the Surrogate Key Generator, as it cannot dynamically pick up the last used key value from the target table.

To fix this issue, before loading any new state names, we need to first identify the maximum surrogate key value currently existing in the target table. Once we have that value, we should pass it into the data flow and add it to the newly generated surrogate key IDs. This way, the new records will receive sequential IDs that are greater than the existing maximum value in the target table.

At this point, we have some erroneous data in the table because two different state names are now sharing the same state_id values. To correct this, I will truncate the target table and reload it with the proper state ID sequence. After reloading, I will again delete the last two rows manually, and then modify the data flow logic to ensure that in the next run, it dynamically generates the new surrogate key IDs starting from the maximum value already present in the target table.

Since we deleted the first two IDs (1 and 2), we don’t want any strange gaps or restarts in our surrogate key sequence. Therefore, I executed the TRUNCATE TABLE statement, which cleared the table completely. After that, I reran the pipeline. This time, it successfully loaded all the 25 state names properly. I verified the result in the SQL Server database, and everything looked correct — the final dimension table contained exactly 25 records with proper state IDs.

Now, I’m going to delete the last two state names again — Himachal Pradesh and Uttar Pradesh — whose IDs are 24 and 25. I made a note of these details so that I can verify them later after making further changes. Next, we will modify the data flow to fetch the maximum surrogate key dynamically from the final target table and then reload these two missing state names with the correct IDs, 24 and 25, in the next lesson.

# **R) Dimension Table Load - Change Data Capture Get Max SURROGATE KEY Using Query**

The actual problem we are facing is related to how the surrogate key transformation works in the data flow. All of the state names can come from any of the files — the first file, the next file, or any subsequent file. In our real-time scenario, we don’t have any control over the data in these files. In our case, both the first and the second January files contain the same list of state names.

To simulate a realistic scenario, I deleted two of the state names that already existed in the target table, assuming that they didn’t appear in the first day’s load. Now, when we run the pipeline using the second day’s source data file, it should ideally insert those two missing state names with the next sequential state ID values, which are 24 and 25.

However, when we run this pipeline with the current data flow configuration, the two new state names are being generated with state ID values 1 and 2 instead. This happens because of a limitation in the Surrogate Key transformation. The surrogate key generator always starts assigning values from the same starting point — usually 1 — and continues sequentially from there, regardless of what values already exist in the target table. Every time the pipeline runs, it resets and starts again from 1, rather than continuing from the last highest state ID.

To fix this, we need to identify the maximum state ID value that currently exists in the target table before loading any new records. Once we identify that maximum value, we can use it to adjust the newly generated surrogate IDs, ensuring that they continue from the correct sequence. For example, if the maximum state ID in the target table is 23, the next two new state names should receive 24 and 25 as their IDs.

Finding this maximum value is quite straightforward — we can generate it using a simple SQL query. For instance, we can use a SQL function such as:
SELECT MAX(state_id) AS MaxStateID FROM [target_table];
This query returns the highest state ID currently present in the target table. We can use the same SQL logic directly inside Azure Data Factory (ADF) to fetch the maximum state ID dynamically before inserting new records. When tested, this SQL query correctly brought back the value 23, which matches the maximum state ID currently in our table.

Now, before inserting any new data into the target table, we need to make sure that our data flow is aware of this maximum value. To do that, we’ll create one more dataset in ADF. So, in the workspace, go to the “Working Labs” section and create a new dataset for the sink table. This dataset will connect to our Azure SQL Database. We’ll name this dataset DataSource_SDK, which stands for Data Source for Surrogate Key. The purpose of this dataset is to retrieve the maximum surrogate key ID from the target (labpur) table.

After creating the dataset, we will select the existing linked service and choose the corresponding table. This dataset will now serve as the data source for fetching the maximum state ID value from the sink table. Once the dataset is created, we need to add an additional source to our data flow.

So, in the data flow canvas, add a new Source and name it something like Source_MaxStateID. From the available datasets, choose the new Labpur dataset we just created. When you look at the Projection tab, you’ll see that it displays all the column names and values from the sink table. Similarly, in the Data Preview, it shows the full set of data from that table. But we don’t need all of that information — we only need the maximum state ID value.

To achieve this, we can modify the behavior in the Source Options. By default, the source tries to read all the data from the entire table, but we can control that by changing the source type. Instead of selecting the Table option, we will select Query. In the query option, we’ll write a SQL query that returns only the maximum state ID value. This way, the source will only fetch and output the result of that query, rather than the entire dataset.

Once we apply this change, the number of columns being output by this source changes — now it should only output the maximum state ID value. When you check the Projection and Inspect tab, it initially still shows all column names. To update it correctly, we need to click on Import Projection.

At this point, ADF will show an error, which is expected. When you open the Notifications and view the Details, it says that in the source Source_MaxStateID, the column name needs to be specified in the query — specifically, an alias must be set if a SQL function is used. Since we’re using the SQL function MAX() to calculate the maximum value, we need to give it a proper alias name. This is a standard SQL aliasing concept.

So, in our query, we’ll write something like:
SELECT MAX(state_id) AS MaxStateID FROM [target_table];
By providing this alias, ADF can recognize and map the column name properly. Now, when we click Import Projection again, the projection updates successfully. The Projection and Inspect tab now correctly displays the single column MaxStateID, and the Data Preview also shows the value 23, which represents the maximum state ID value currently in the target table.

Now that we have this additional source correctly configured, the next step is to merge this source with the main data flow. By doing this, we can use the maximum state ID value retrieved from the target table (which is 23 in this case) and add it to the newly generated surrogate IDs. This will ensure that the new state names are assigned IDs starting from 24 and 25, instead of 1 and 2.

We will configure this merge logic and update the data flow in the next lesson so that the surrogate key generation dynamically starts from the maximum state ID value already present in the target table.

# **S) Dimension Table Load - Merge Max SK with Source Using JOINER Transformation**

When we previously used the additional source last time, we had a common column name between the mainstream source coming from the source file and the sink table. However, this time we only have the maximum state ID, and the state ID value is not at all appearing in the mainstream source file. If you inspect the data, you can see that there is no state ID column anywhere. The only place where the state ID is generated is at the surrogate key output. The state ID values in the surrogate key are generated sequentially, such as one and two for each of the source rows passing through. These generated values will never match the state ID values present in the additional source that we created from the sink table.

Now, we need to identify a way to match this additional source with the mainstream source coming from the source file. Probably, we need to apply a specific logic to join the mainstream source with this additional source. From the source, we are getting the state name values, and in the lookup stage, we are comparing the state name values against the existing state name values in the sink table. If the state name does not exist in the sink, then only we pass that record to the next step, and those records are the ones that get inserted into the target table. This means that the state name value coming from the mainstream will never be null after the filter transformation. Only such non-null records will get inserted into the target table.

Similarly, if any state ID exists in the target table, then this maximum state ID value also will not be null. Therefore, we are going to use these two conditions to join these two sources. Probably, I will do a data preview here. Again, it will bring the two state names we have deleted from the target table earlier. Based on the logic that we discussed, Himachal Pradesh and Uttar Pradesh will be appearing as the state name values in the mainstream source.

In the filter stream output, we can see these two state names. The state ID already exists as eight in the target table, and hence it will not be null. The 23 value we see here has nothing to do with the state names themselves; therefore, we cannot use these values to match. Whenever two sources are created, we must merge them together in the main stream. Otherwise, we cannot use the values coming from the other source or make any decisions based on that data.

Now, we need to join the maximum state ID value that we derived from the sink table with our mainstream source. To achieve this, we are going to use the Joiner transformation. By applying the Joiner transformation, both the maximum state ID value and the new state ID value will be available before loading the data into the target table. So, I am going to include the Joiner transformation this time to join these two datasets.

The Joiner transformation is a multi-input transformation, so it requires two input streams to be connected to it. In our case, the left stream is already connected from the output of the filter transformation, which contains the new state name values that need to be loaded into the target table. The right stream will be the new source that we created — basically, the source containing the maximum state ID.

Now, within the Joiner transformation, we can set five different types of join conditions based on the column names that we select. However, in this case, we do not have any common column names between the two sources. The output of the filter has a column named state_name, and the output of the maximum state ID source has a column named maximum_state_id. These two columns are not the same and cannot be joined directly.

If we had a common column name, we could specify the join type accordingly. For example, if we selected an inner join, only the matching records between these two sources would pass through after the join. If we selected a left join, all records from the left stream would pass through, and only the matching records from the right stream would be included. In a right outer join, all the records from the right stream (which is the third source) would pass through after the transformation, and only the matching records from the main stream would be included. If we set a full outer join, then all of the records from both sources would pass through after the join transformation.

However, none of these standard join types are useful for our current scenario. Instead, we need to define a custom join condition based on the data we have. One dataset consists of filtered new state name values, and the other dataset contains the maximum state ID value. Both of these values are not null, and we only need to pass the records where these conditions hold true. After this inner transformation, we will set that configuration using the custom join type in the next lesson.

# **T) Dimension Table Load - Merge Max SK JOINER Transformation Custom Join Condition**

We don’t have a common column name between the filtered new stream and the source containing the maximum state ID. That’s why we are going with the custom join type. This is a really special case because such join conditions cannot be easily implemented directly within a database. It is one of the more complex and powerful features available in Azure Data Factory (ADF).

We opened the Expression Builder in the Joiner transformation to define the logic. The condition we need to implement is that the state name coming from the mainstream source should not be null, and the maximum state ID value coming from the sink table should also not be null. If both these conditions are met, then the records should be passed through after the join transformation — that’s exactly what we are trying to achieve here.

Now, there is no direct IS NOT NULL function available in ADF Data Flow expressions. If you search for IsNull, you will find that only the IsNull() function exists. Therefore, we must use the IsNull() function in combination with the NOT operator. In the expression builder, there is a section in the middle where operators are listed — we will use the NOT operator from there. First, click on NOT, and then open and close brackets to form the expression. Inside the brackets, specify IsNull() for the first column you want to check. So the expression becomes Not(IsNull(state_name)) — this ensures that the state name coming from the mainstream source file is not null.

Next, we need to add another condition for the maximum state ID value. We use the AND operator, which is also available among the operators in the middle panel of the expression builder. The second condition will be Not(IsNull(max_state_id)). Combining both, our final expression becomes:

Not(IsNull(state_name)) && Not(IsNull(max_state_id))

This means that only records where both the state name and maximum state ID are not null will pass through the join transformation.

After applying this condition, if we look at the data preview of the join transformation, we will see that the two state names we deleted from the target table — Himachal Pradesh and Uttar Pradesh — are now appearing correctly in the output. Each of these state names is now associated with the maximum state ID value derived from the sink table.

If we further look at the output of the Surrogate Key transformation, we can see that it has generated new surrogate key values such as 1 and 2 for these new rows. Meanwhile, the maximum existing state ID value coming from the sink table is 23. Now, if we add these two values together, we will get 24 and 25 — which are the correct new state IDs that should be assigned to these two new state names.

Basically, what we are doing here is overcoming the limitation of the Surrogate Key Generator transformation, which always starts generating keys from 1 for each new load. Instead, we are building our own logic to incrementally generate state ID values based on the existing maximum state ID value in the sink table.

The surrogate key generator output gives us the new surrogate values (1 and 2). In the Derived Column transformation, we will now create a new column named new_state_id. In the expression editor, we will define it by adding the maximum state ID value from the target table to the state ID generated by the surrogate key transformation. This means our expression will be something like:

new_state_id = max_state_id + state_id

This ensures that for the new state name records, the state IDs will be correctly calculated as 24 and 25.

In the Sink mapping, we must ensure that the new column new_state_id is mapped to the state_id column in the target table, not the one directly generated by the surrogate key generator. This is because the surrogate key-generated values (1 and 2) already exist in the database table and we don’t want to reuse them. By using our derived column instead, we ensure that the state ID values remain consistent and incremental based on existing data.

Once the mapping is properly configured, we can publish the changes and run the pipeline again. During this run, the two state name values — Himachal Pradesh and Uttar Pradesh — will be inserted into the target table with the correct state ID values 24 and 25.

After the pipeline execution completes successfully, we can verify the results in the SQL Server database. When we query the target table, we will see that Himachal Pradesh and Uttar Pradesh are indeed loaded with state IDs 24 and 25 respectively. This confirms that the logic works perfectly.

We have made excellent progress here. Throughout this single data flow, we’ve managed to explore and apply a variety of transformations available in ADF. For example, under the multiple input/output section, we used both the Join and Lookup transformations. Under the schema modifier section, we used Derived Column, Select, Aggregate, and Surrogate Key transformations. In the row modifier section, we used the Filter transformation. And finally, we also configured the Sink transformation for output.

This is a very good starting point because we now have a proper logic for developing and loading dimension tables using Data Flows in Azure Data Factory. However, we have not yet parameterized our source and sink datasets. That will be our next step — in the upcoming session, we will develop one more data flow where we parameterize everything for the Reporting Dimension Table Load.

# **VIII) Reusable DATAFLOW Design For Loading Dimension Tables**

# **A) Reusable DATAFLOW Design - Create Source and Sink Datasets**

I would like to close all the unnecessary things. I’m going to refer to this data flow for creating the generic data flow with parameters and as much reusability as possible in that pipeline. We are going to do that under the actual folder name. So, for the ingest, we created one folder name, and in the same way, for transformation pipelines, we are going to create another folder name. So click on “New Folder” and create a new folder called transform. As soon as you create the folder under the pipeline, create it under the dataset as well so that any datasets related to the actual transform pipelines will be stored there. In the same way, under the data flow, also create the transform folder so that we will have the proper folder structure across the subcomponents of the ADF data flow.

Now, I am going to use the existing data flows as a reference for creating the new data flow. I am going to use that same name without the “lab” suffix, as that’s how we are following the naming convention. So, under the transform folder, I’m going to create the data flow. In the previous step, we created the data flow from the pipeline, but this time we will try to create it directly under the Data Flows section, and then we will call it from the pipeline. However, before creating the data flow, it’s better to first create the necessary parameterized datasets so that we can easily create and reuse the data flow.

The first dataset used in the source of the data flow is RDS ADLS Daily Pricing Landing Source. We will create this new data source without the “lab” suffix, but we will parameterize all of the container name, folder name, and file name as well. So, I’m going to create the new dataset under the transform folder. This dataset will point to the Azure Data Lake Storage Gen2 account, and it is a Delimited Text file. I’m going to give the name RDS_ADLS_DailyPricing_Landing_Source. We are going to use the same linked service here. I’m not going to give the path name or import the schema at the moment because I’m going to parameterize all of these file path connection settings.

We know where to create the parameters. You can come here and create three parameters: dataset_prm_landing_container_name, dataset_prm_landing_folder_name, and dataset_prm_landing_file_name. Previously, we have used cm_sink_container_name and sink_folder_name in the ingestion pipelines, but now we are reading it as a source. So, we have given the landing file name and the landing folder name accordingly. After creating these three parameters, we can quickly map them using the Pipeline Expression Builder. I’m going a little quick, but you already know all these steps from previous lessons, so hopefully, you can follow along easily.

The first mapping is for the container name, the next one is for the folder name, and the last one is for the file name so that we can pass the file paths to the dataset at runtime. However, we need the schema because we are working on individual column-level transformations. When you import the schema, it will ask for the values of these three parameter values. You can take them from the existing Landing dataset — for example, this one is Daily Pricing, and for the file name, you can provide any one of the existing file names in the Data Lake Storage account or from the previously created dataset. That way, it will import the necessary columns for us. This step is required for our data flow since we’ll perform transformations on specific columns.

Now that we have parameterized our source dataset, we can publish all changes to store it under the transform folder. Once done, close the dataset to keep things tidy.

The next source we need to create is for getting data from the sink table. This is the one we need to create the dataset for next. If you look at the existing dataset, it’s pointing to that specific table. We can parameterize this dataset’s table name and schema name so that it can be reused across multiple lookup tables. Therefore, we will create a parameterized dataset for the Dim State Source, which reads data from the sink table — that’s the purpose of this one.

So again, come here and create a new dataset. This one will be of type Azure SQL Database. Choose Azure SQL Database and provide the name as SQL_Report_DimState_Source (without the “lab” suffix). Use the existing linked service for the SQL connection. For the table name, I do not want to provide it at the moment because we are going to use a different technique to read the data from this source. So, I’ll just click OK without specifying the table or schema. I do not want the schema either for this specific source because I’m going to use this same source for looking up all of the sink tables, not only one specific table.

If we publish it, hopefully, it won’t invalidate, and that’s fine — it’s working correctly. If we come back to the data flow, there’s one more source we might need, but I think we can manage with the Dim State Source that we already created. I just need to rename it from Dim State Source to Dim Tables Source because this is the one I am going to use generically for multiple dimension lookups. So probably, we can rename it DimTables_Source to make it clear and consistent with naming conventions.

Now we have created all the necessary source datasets. Next, we need to create the sink dataset. We will create one dataset per sink table — that is the approach we need to follow. So, it’s better to go that route. Go ahead and create a new dataset, again choosing Azure SQL Database as the type. Then provide the name as DimState, and choose the same linked service. Because the column names are specific to each table, we can’t parameterize this one. It’s better to choose the existing DimState table directly and publish the changes.

So now we have created all the datasets needed for our final data flow that we are going to build for the transformation stage. In the next lesson, we will start creating the actual data flow using these parameterized and reusable datasets.

# **B) Reusable DATAFLOW Design - Configure Source Transformation**

We created all the data sets and now needed to start developing the proper data flow to load the dimension table. So, I clicked on the transform folder to create a new data flow, and again, we are going to load the same dim state table. This time, we will do proper development on each of the sources wherever possible, bringing reusability into the code. The first step in the existing data flow is reading the daily pricing data source, which we can reuse since it has a very generic name. We create the source and provide the same output stream name used in the previous data flow. Now, instead of using the lab dataset, we use the new generic daily pricing landing source dataset that we created. Searching for the landing dataset will show two options: one with “lab” and another without. We choose the one without “lab.” Once we configure the source, the projection shows all column names coming from the source file, and the inspect view shows the same column names. If needed, more than one file from the source directory can be read using a wildcard path, which we will likely use when developing the data lake, but for now, we stick with one source file and leave the remaining properties as default. Next, we configure a source to read data from the sync table to check whether the data in the source file exists in the sync table. Previously, we read the entire sync table and used a select activity to delete unnecessary columns, but this time, we are focusing on reusability. Instead of naming it “select dim state lookup,” we call it “select dim lookup,” making it generic for all dimension tables. We select this source as the Azure SQL Report Dim Table source. To locate the dataset, we copy the full dataset name and search using the complete string, which makes mapping easier. For this specific dataset, we do not configure any source table or import any schema because we intend to use this source to derive anything we want by writing queries. If the source points to a table, it can only read data from that table; if it is from a query, we can write a query to read from any dimension table. 

For example, we can get the maximum state ID value from the target table using the same source. Previously, two sources were created for this, but now we use one reusable dataset. I write a query to select the state name from reporting.dim_state, which will be used in this data flow. At the moment, there is no proper projection because the system doesn’t know which columns or table names to bring, so whenever writing a query, it is necessary to click “Import projection,” otherwise it won’t work. 

The dataset parameter values we set for the original source file are unrelated to this one, but providing them is necessary to run the entire data flow successfully. We save, and the import projection completes, showing the state name value. Instead of providing a direct query, I plan to generate a dynamic query in the next lesson, as converting this into a dynamic query will allow the same source to be used for all dimension tables.

# **C) Reusable DATAFLOW Design - Generate Dynamic SQL Query Using Dataflow Parameter**

We are loading the dim state table, which is why we are selecting the state name value from reporting.dim_state. When we develop the data flow for loading the dim market table, the column name and table name will change. If we can parameterize these two components in this source, then the same source component can be reused for all dimension tables. To achieve this, we use data flow parameters. If you click anywhere outside the transformations, the data flow settings appear. This works just like parameters in datasets and pipelines, and these parameters will be passed from the pipeline that calls the data flow.

For now, we need three parameters: one for the reporting table lookup column name, one for the reporting table schema name, and one for the reporting table name. We create these three parameters at the data flow level. Later, I will show how to use these parameters to dynamically generate the SQL query.

Next, we return to the second source—this is the one used to check whether the state name values coming from the source exist in the target table. Earlier, we created this in the lab, but now we are making it generic so it can be reused for other dimension tables. We open the source and click “Add dynamic content” for the existing SQL. The goal is to recreate the same SQL statement using the Expression Builder.

The first part of the SQL, the keyword “SELECT,” will not change, so it stays as it is. The state name column will be replaced with the parameter we created for the lookup column name. Similarly, the “FROM” keyword stays fixed, but the reporting schema name will be replaced with the reporting schema name parameter, and the table name (dim_state) will be replaced with the reporting table name parameter.

To combine all of these values, we must use the concat() function. Without concat, the expression will fail. So we rebuild the SQL step-by-step using concat(). The first part is "select " with a trailing space. Spacing is important since we are dynamically building SQL—missing spaces can break the query. The second argument is the lookup column parameter. The third part is " from " again with a leading and trailing space. Then we insert the reporting schema parameter. After that, we include a dot (.) as a constant string because we do not have a parameter for it. Finally, we append the reporting table name parameter and close the concat function.

If any comma or argument is missing, the validation will fail. Once everything is added correctly, the expression validates. This dynamically generated SQL will produce the same query we manually wrote earlier. Using this method, we can clone the same data flow for any other dimension table—only the table name and column name parameters will change, but the component remains reusable.

Before finalizing, we need to add one more detail. We want to give an alias name to the lookup column. Right now, it will return the original state name column, but we want a generic alias such as "lookup_target_column". So we add one more string to the concat() statement: as lookup_target_column. This allows every dimension table to return a standardized column name from the lookup source.

Now we have a fully generic second source. The next step will be creating another source that retrieves the existing maximum state ID values from the target table, which we will handle in the upcoming lesson.

# **D) Reusable DATAFLOW Design - Dynamic SQL Query Import Projection**

In the previous data flow, we simply mapped the second source into a specific table. From that table, the schema information was imported. After that, we included a select transformation to exclude additional columns. In this setup, the same source could not be used for loading multiple dimension tables.

When generating the new data flow, we parameterized everything in the select statement and provided a general alias for the lookup column retrieved from the sync table. Regardless of whether it’s a dim_state or dim_market table, it always comes as lookup_target_column_value. This alias needs to be reflected in the projection because the projection happened when we ran the previous select statement on the dim_state table. Therefore, we need to reapply the import projection.

Now, the system is asking for the values for the data flow parameters that we created. Previously, we had passed these values, but since we just created the data flow parameters, we need to provide the names based on the specific table we are working on. Eventually, these names will become generic. For example, the schema name is reporting and the table name is dim_state. This is also a good exercise to check if our alias is working properly.

These values will replace the placeholders in the concatenated select statement and execute the output expression, which is basically the select statement. For example:

SELECT state_name AS lookup_target_column_value 
FROM reporting.dim_state

That’s what will execute when we do the import projection. The alias name lookup_target_column_value will appear in the projection.

The process initially failed, and we identified the reason. This is a good opportunity to remember: when passing string values to data flow parameters, you need to enclose them in single quotes. Without the quotes, the data flow expression builder will not accept them. Once the parameters are passed correctly, re-clicking import projection will work. The data set parameters pointing to a folder name worked fine without issues.

After saving, the import projection works. The alias name given in the select statement now appears as a column name in the projection. This generic name allows the same data flow to be used for multiple dimension table loads. Previously, the projection pointed to state_name, but now it points to a generic dim lookup value.

Next, we need to create a generic source to get the maximum surrogate ID value from the sink table. We can copy the existing source temporarily for this purpose because it is not pointing to any source table. Click “Add Source” and use the same data set that was used to get the maximum surrogate ID value.

In the source options, click the query button and pass the query that selects the maximum state ID value from the dim_state table. We plan to dynamically change the select statement like we did before. The maximum state ID value comes from the reporting dim_state table. We already have parameters for the table name and schema name, but we need one more parameter at the data flow level to populate the state ID column name, as there is no existing parameter binding for this column.

We will cancel the current attempt because it won’t allow validation. Instead, we’ll go back to data flow parameters, create one more parameter for the surrogate key value, and configure the dynamic SQL. This way, we can use the same data set without binding it to any table in the database. By using SQL queries dynamically, the data set can serve multiple purposes.

Creating the new data flow parameter and configuring the dynamic SQL will be covered in the next lesson.

# **E) Reusable DATAFLOW Design - Dynamic SQL Query For Max Surrogate Key Value**

We start by generating a new data flow parameter whose purpose is to hold the key column name dynamically. This parameter allows us to reuse the same data flow for different dimension tables without hard-coding column names. We name this parameter DFL_PRM_ReportingTable_IDColumn. This parameter represents the ID column we are interested in for the current data flow.

For this specific data flow, the value will be State ID, but for subsequent data flows, this value will change based on the dimension table being loaded. That is why we parameterize it instead of hardcoding it.

Next, we come back to the existing query that we have used in the past and copy-paste it again. This time, instead of a static query, we will make it dynamic by using the concat function to generate the SQL statement dynamically.

Before applying the concat function, we remove the closing bracket of the existing expression. The first part of the SQL query, starting from SELECT up to MAX(, remains unchanged. This portion of the query will always stay the same.

The only part that needs to be dynamic is the State ID column. Instead of hardcoding StateID, we replace it with the data flow parameter DFL_PRM_ReportingTable_IDColumn. This parameter dynamically injects the key column name into the query.

After the first string literal, we add a comma, then place the data flow parameter, followed by another comma. The remaining portion of the query—specifically the closing bracket of the MAX function and the alias—remains unchanged.

Instead of using the alias MaximumStateID, we rename it to MaximumSurrogateKeyID. This naming is intentional so that the alias can be reused consistently across all dimension tables, regardless of the actual column name.

The query remains unchanged up to the FROM clause.

Next, we address the schema and table name. The schema name reporting is replaced with a schema name data flow parameter. After the schema name, we add a dot (.) inside quotes, followed by a comma.

Finally, the table name DimState is replaced with the data flow parameter for the table name. Once all replacements are done, we apply the closing bracket of the concat function.

At this stage, validation may still throw an error. This usually happens if a comma is missing in the concat arguments. Since concatenation works based on multiple values separated by commas, every component must be correctly separated.

After verifying, we notice that one comma was missing. Once it is added, everything validates correctly. We then save and finish the step.

Now, when we perform Import Projection again, the system prompts us to provide values for the data flow parameters:

Schema name

Table name

ID (key) column name

These values were already provided earlier, but we must enter the ID column name again, ensuring that it is passed inside quotes. This is important to avoid runtime errors.

At this point, everything looks correct, but an error still appears related to the alias name. On closer inspection, we realize the issue is due to incorrect usage of the concat function. Instead of properly using concat, it was mistakenly nested or duplicated.

After removing the extra concat function calls, we save and finish again.

When we perform Import Projection once more, the data flow runs successfully. The output now correctly brings the alias column name defined in the SELECT statement, which is MaximumSurrogateKeyID.

If we compare the existing Lab 4 data flow with the new data flow we are developing, the difference becomes very clear.
In the older data flow:

The second source column name is specific, such as LookupStateName

The third source outputs MaximumStateID

In the new data flow:

The second source output column is DimLookupValue, which is completely generic

The third source outputs MaximumSurrogateKeyID, which is also generic

This shows that we are building a fully reusable data flow. It is no longer tied to a specific table or column. The same data flow can now be reused to load multiple dimension tables simply by changing parameter values.

That is the core objective of this exercise—to design a generic, parameter-driven data flow.
In the next lesson, we will continue building the subsequent sections of this reusable data flow.

# **F) Reusable DATAFLOW Design - Configure SELECT , AGGREGATOR and LOOKUP**

Now that we have defined the three required sources, we can start building the subsequent sections of the data flow.

The first transformation we need to add after the source is by clicking the plus (+) button and selecting the Select transformation. This step is used to choose only the required column from the source and remove all unnecessary columns.

In the current scenario, we are loading the Dim State table. From the source, we only need the State Name column. So, we select the State_Name column and remove all other columns by unchecking them.

Once that is done, we rename the State_Name column to a generic column name. This is an important step to make the data flow reusable. Instead of keeping it specific to “State Name,” we rename it to:

SourceFileDimColumn

This represents the column from the source file that will be used in the dimension table. By doing this, the same data flow can be reused for other dimension tables without changing the internal logic.

Next, we use an Aggregate transformation to identify distinct values from the source dimension column. Previously, we used the State Name column directly, but now, since everything is generalized, we use the renamed column SourceFileDimColumn.

We add an Aggregate transformation and name it something like Find Unique Source Values. The source column used in the aggregation is SourceFileDimColumn. Although in this case it represents State Name, in future data flows it could represent something else, such as Market Name or Category Name.

Inside the Aggregate settings, we specify the count of SourceFileDimColumn. To do this, we use the count() function and ensure that the column selected inside the count function is SourceFileDimColumn.

Even though this column is technically pointing to State Name in the current flow, we consistently use the generic name. This reinforces the idea that the same data flow can be reused across multiple dimension tables without any internal modifications.

At this stage, we keep the count column in the output. Any unnecessary columns can be removed later using another Select transformation if required.

The next step is to look up existing records from the dimension table to determine which values already exist in the sink. For this, we add a Lookup transformation and name it generically, such as Lookup Dim Table.

The aggregate output is connected as the main stream of the lookup transformation. The lookup stream is connected to the second source, which represents the existing dimension table (source dim lookup).

In the lookup configuration, we define the matching condition as follows:

From the source stream: SourceFileDimColumn

From the lookup stream: DimLookupValue

Effectively, this means we are comparing:

State Name from the source file

State Name from the existing dimension table

Even though these are State Name columns in this data flow, we use generic names to maintain reusability.

If the DimLookupValue coming from the lookup stream is NULL, it indicates that the corresponding source value does not exist in the sink table. These are the records that need to be inserted into the dimension table.

Filtering out these NULL lookup values will be handled in the next lesson, where we will add a filter transformation to pass through only the records that do not already exist in the dimension table.

At this point, we have successfully:

Selected and generalized the source dimension column

Identified distinct source values using aggregation

Looked up existing dimension values to detect new records

In the next lesson, we will continue by filtering the unmatched records and proceeding further in the data flow.

# **G) Reusable DATAFLOW Design - Configure FILTER , JOINER and DERIVED COLUMN**

Now, we include a Filter transformation to filter out only the new records coming from the source that do not already exist in the sink table.

We add a Filter transformation and name it Filter New Source Values. In the filter expression, we specify the condition that the DimLookupValue is NULL. This condition was already identified earlier during the lookup step.

To build the expression, we select the isNull() function, remove the default search string, and pass DimLookupValue into the function. If DimLookupValue is NULL, it indicates that the corresponding source record does not exist in the target dimension table. Only those records should pass through the filter, as they are the ones that need to be loaded into the sink.

Next, we create a Join transformation to join these filtered records with the maximum surrogate key value coming from the sink table. The required SQL for fetching the maximum surrogate key was already generated earlier.

We add a Join transformation and name it Join Max Surrogate Key. The main stream comes from the filtered source records, and the second stream comes from the source that provides the maximum surrogate key value (the third source defined earlier). We connect both streams accordingly.

Since there is no common column between these two streams, we configure a custom join condition. The join condition ensures that both streams have valid data.

The custom join expression is built as follows:

NOT isNull(SourceFileDimColumn)

AND (&&)

NOT isNull(MaximumSurrogateKeyID)

There is no direct notIsNull() function available, so we use the NOT operator along with the isNull() function. This ensures that only rows with valid source dimension values and a valid maximum surrogate key value are joined.

Once the join condition is configured, we save and finish the transformation.

At this stage, all transformations are correctly connected. Only the source values that do not exist in the target table will pass through the pipeline. These are the records for which new surrogate keys need to be generated.

Before generating the final surrogate key values, we remove any unnecessary columns flowing through the pipeline. After the join, the only columns we actually need are:

The source file dimension column

The maximum surrogate key ID

The count of source values and the DimLookupValue are no longer required at this point.

Instead of adding multiple Select transformations at different stages, we add a single Select transformation just before mapping the data into the sink. We name this transformation Select and Map Dim Columns.

In this step, we explicitly remove:

Count of SourceFileDimColumn

DimLookupValue

We retain only the columns required to generate the final surrogate key and load the dimension table.

Next, we add a Surrogate Key transformation to generate new surrogate IDs. The key column is named generically as KeyID (or SurrogateKeyID), rather than referring to a specific column such as StateID. This keeps the data flow completely reusable across multiple dimension tables.

The surrogate key generated here represents the incremental ID for new records within this data flow execution.

Now, we need to generate the final surrogate key value that will be loaded into the target table. This requires adding the newly generated surrogate key value to the existing maximum surrogate key value from the sink.

To do this, we add a Derived Column transformation and name it Derive New Key and Audit Columns.

In this transformation, we derive a new column called SurrogateKeyID. The expression used is:

MaximumSurrogateKeyID + GeneratedSurrogateKeyID

This ensures that the new records continue the surrogate key sequence from the existing maximum value in the target table.

In the same Derived Column transformation, we also create the required audit columns:

DW_Created_Date

DW_Updated_Date

Both of these columns are populated using the current date function available in the data flow. The current date value is assigned to both columns, ensuring consistent audit tracking for newly inserted records.

At this point, we have:

Filtered only new source records

Joined them with the maximum existing surrogate key

Generated new surrogate key values

Derived final surrogate keys and audit columns

The final step—mapping all these columns to the sink (dimension table)—will be covered in the next lesson.

# **H) Reusable DATAFLOW Design - Configure SINK & Pipeline To Automate Run**

Now, we create a Sink activity to map all the derived values into the final target dimension table. We name this sink activity Sync Dimension Tables, again using a generic name so it can be reused across different dimension loads.

We have already created the dataset for the sink table, which in this case is DSA_SQL_Report_Dim_State. We select this dataset, and it resolves correctly.

Next, we go to the Settings section of the sink. For now, we enable Allow Insert only. We are not truncating the table at this stage. The objective here is to insert only new records identified by the data flow.

Then we move to the Mapping section to ensure all required columns from the data flow are correctly mapped to the sink table.

At this point, we notice a small issue. In the previous version of the data flow, columns were automatically mapped because their names matched the sink table column names. However, in this reusable data flow, we have renamed columns to generic names, such as SourceFileDimColumn.

Because of this:

The dimension value (State Name) now comes from SourceFileDimColumn

The dimension ID (State ID) comes from the newly generated SurrogateKeyID

The remaining technical or intermediate columns are no longer needed and are not mapped

After validating the mappings, everything looks correct.

Now we publish the data flow. At this point, only the data flow definition is saved. Nothing is executed yet.

Next, we need to build a Pipeline to execute this newly created data flow.

We navigate to the Transform subfolder under the Ingest folder. To keep everything consistent and reusable, we create a new pipeline and give it a name without referencing Lab 4, so it can be reused in the future.

Before proceeding, we close all unnecessary windows to keep the workspace clean.

Inside the pipeline canvas, instead of manually adding a Data Flow activity, we directly drag and drop the data flow from the Transform folder. This automatically creates a Data Flow activity and links it to the correct data flow definition.

Once added, the activity prompts us to provide values for:

Dataset-level parameters

Data flow-level parameters

Dataset-level parameters appear under the Settings section of the activity.
Data flow-level parameters appear under the Parameters section of the data flow activity.

For now, we hardcode the parameter values for a quick test run. Later, these values can be fully automated using pipeline parameters.

We provide:

Landing folder name as daily-pricing

File name by selecting an existing file from the landing container to ensure the pipeline runs successfully

This process is similar to passing values to pipeline parameters, but data flow parameters behave slightly differently.

When passing values to data flow parameters, we must be careful. In the Parameters section:

Click on each parameter

Choose Data Flow Expression (not Pipeline Expression)

Pass string values inside quotes

Data flow expressions work differently from pipeline expressions, and failing to use quotes will result in validation errors.

We now pass the data flow parameter values as follows:

Schema Name → "reporting"

Table Name → "dim_state"

Lookup Column Name → "state_name"

Key ID Column Name → "state_id"

After entering all parameter values, we save and finish the pipeline configuration.

When we run the pipeline, it will load data into the SQL Server dimension table. In this case, it will populate the table with all 25 state records, generating surrogate keys dynamically.

For testing purposes, we may choose to truncate the dimension table first and then run the pipeline again to verify that the data is loaded correctly.

If the pipeline runs successfully, it confirms that:

The reusable data flow logic is working

Parameterization is functioning as expected

Surrogate key generation and mapping are correct

If any errors occur, that is also useful for learning and debugging.

In the next lesson, we will:

Monitor the pipeline run status

Review execution logs

Analyze any errors or warnings in detail

# **I) Reusable DATAFLOW Design - Debugging**

Sometimes, when you run the data flow, it may not respond for a longer time than expected. This usually happens because the Data Flow Debug cluster that was created earlier is no longer in a reachable or healthy state.

In such cases, the best approach is to disable the Data Flow Debug option first. Once it is disabled, enable the Data Flow Debug again. This forces the system to recreate a new debug cluster instead of reusing the old one.

After recreating the debug cluster, when you rerun the data flow, it typically executes much faster. This is exactly what we are doing here, because the previous run was taking too long to respond.

Now, when we click the Debug button again, the data flow either runs successfully or throws an error. Ideally, seeing an error is also helpful, as it allows us to debug and identify the root cause of the issue.

In this case, the data flow runs successfully again.

Next, we go back to the SQL Server database and run a query on the dimension table. As expected, there are no duplicate records. Only 25 state names are present in the table, which confirms that:

Duplicate filtering logic is working

Lookup and filter conditions are correct

Surrogate key generation is functioning as intended

All the implemented logic is working perfectly.

Now, to load the next dimension table, there is no need to build a new data flow from scratch. All we need to do is clone this existing data flow.

Inside the data flow, the only change required is in the Select transformation, where we replace:

State_Name with the specific dimension column name (for example, Market Name, Category Name, etc.)

When calling the data flow from the pipeline, we simply update the data flow parameter values:

Schema name

Dimension table name

Lookup column name

ID (key) column name

These parameter changes are the only modifications needed to load any other dimension table.

This approach allows us to reuse the same data flow to load all remaining dimension tables with minimal effort.

In the next lesson, we will:

Create all required dimension tables in the database

Run the same pipeline repeatedly with different parameter values

Demonstrate the flexibility and reusability of this design across multiple dimension tables

# **J) Reusable DATAFLOW Design -Produce Dimension and Fact Tables CREATE SQL Scripts**

As part of a data engineer’s responsibilities, we also need to generate the CREATE TABLE scripts for all the dimension tables and fact tables.

To make this process easier and more efficient, I have already added commas at the end of all column names in the column definition list. This small step helps us quickly reuse and modify the script for multiple tables without manually adjusting syntax every time.

Next, we copy this column definition block into SQL Server Management Studio (SSMS). SSMS is another tool available for working with SQL Server databases, and it provides more advanced features compared to other interfaces, making it ideal for executing DDL scripts.

We begin by writing the CREATE TABLE statement. I start with the CREATE TABLE keyword and add the opening bracket. Then, I update the table name accordingly.

To maximize efficiency, I reuse the same column definition block for each dimension table. For every new dimension table:

I paste the same column definition string

Update the table name

Remove the last comma at the end of the column list before executing the statement

This approach allows us to quickly create all required tables with minimal effort.

Once the CREATE TABLE statements are ready, we also generate the corresponding DROP TABLE statements. These are useful when we need to rerun the script or reset the environment.

We copy the CREATE TABLE script and modify it to use the DROP TABLE IF EXISTS syntax. This ensures that the script can be executed safely without throwing errors if the table already exists.

At this point, we realize that we missed one important detail—the schema name. We update all table references to include the reporting schema.

After adding the schema name, all CREATE and DROP statements are complete.

Now, we execute the entire script at once in SQL Server Management Studio. All commands execute successfully, and the tables are created without any errors.

When we refresh the table list, we can see:

Five dimension tables

One fact table

This confirms that all required tables have been created correctly.

Finally, we save this script and make it available in the Resources section, so it can be reused to create tables in any reporting database.

In the next lesson, we will move on to creating reusable data flows for the remaining dimension tables.

# **K) Reusable DATAFLOW Design - Reusing to Populate DIM_MARKET Dimension Table**

Now that we have created all the dimension tables and the fact table in the database, the next step is to create datasets for the remaining tables. This needs to be done before we start reusing the reusable data flow for loading other dimension tables.

To make this faster, we can simply clone the existing dataset (for example, the one created for Dim State) and update only the table name and schema mapping.

We start with Dim State and then move on to Dim Market.
For Dim Market:

Clone the Dim State dataset

Update the table name to Dim_Market

Go to the Schema tab

Clear the existing schema

Use Import Schema to fetch the correct column structure

Publish the dataset

Because each dimension table has a different column structure, importing the schema ensures the dataset is correctly aligned with the table definition.

We repeat the same process for the remaining dimension tables:

Dim Product

Dim Variety

For each table:

Clone an existing dimension dataset

Update the table name

Clear the existing schema

Import the new schema

Publish the dataset

All these dimension tables use the same source dataset for loading data, and the same SQL dataset structure, which is why our design is fully reusable.

The Date dimension is a special case. It is usually loaded using a one-time upload or a specific logic. We will handle that separately later.

For now, all remaining required dimension table datasets are created and ready.

With the datasets in place, we can now reuse our data flow very easily. In just a few minutes, we can populate multiple dimension tables using the same logic.

We start by cloning the Dim State data flow.

After cloning:

Rename the data flow to Dim Market

Remove the “copy” suffix to keep the naming clean

Inside this cloned data flow, the only change required is in the Select transformation after the first source:

Replace State Name with Market Name

All remaining transformations continue to work without any change.

Next, we update the Sink transformation:

Select the Dim Market dataset that we created earlier

Go to the Mapping section

Ensure that:

SourceFileDimColumn maps to Market_Name

The new surrogate key maps to Market_ID

That is the only change required at the data flow level.

Now, we add this new data flow to the main pipeline.

We are not creating separate pipelines for each dimension table. That is why we named the pipeline Load Reporting Dim Tables.

We drag the Dim Market data flow into the pipeline and connect it after the Dim State data flow.

When we click the Dim Market data flow activity, it prompts us for the source dataset parameter values. We can simply copy these values from the first data flow.

For now, we hardcode the file name, folder name, and container name so that we can quickly verify everything is working. Later, we will automate these values using pipeline parameters.

Next, we configure the data flow parameters using the Data Flow Expression editor:

Table Name → "dim_market"

Lookup Column Name → "market_name"

ID Column Name → "market_id"

After providing these values, we save and finish the configuration.

At this point, if we run the pipeline, it will:

Load data into Dim State

Load data into Dim Market

Since we previously dropped and recreated all dimension tables, the Dim State table is currently empty. Therefore, both data flows will load data fresh into their respective tables.

In the next lesson, we will:

Run the pipeline with both data flows together

Validate the data in Dim State and Dim Market tables

Continue loading the remaining dimension tables using the same reusable approach

# **L) Reusable DATAFLOW Design - Reusing to Populate DIM_PRODUCT Dimension Table**

Let’s start debugging the pipeline so that it loads both dimension tables together.

We continue using the existing debug cluster, which is already in a ready state. Since the cluster is available, the pipeline will run a little faster. The pipeline is configured to execute the two data flows one after another. Although it is possible to run them in parallel, we deliberately avoid that for now because the debug cluster is very small, and we do not want to overload it.

With this setup, the pipeline will load data into both the Dim State and Dim Market tables sequentially.

While the pipeline is running, we start preparing the next data flow for the Dim Product table. Once again, the required changes are minimal. In just a couple of minutes, the same reusable data flow can be adapted to load another dimension table.

The only special consideration with the Product dimension is that it contains both:

Product Name

Product Group Name

However, the Product Group Name does not play any role in the lookup or join logic. It has a one-to-one relationship with Product Name, so the existing logic remains valid. The Product Name continues to be mapped to the SourceFileDimColumn, which means the data flow logic still works without any structural changes.

When configuring the Sink for the Product data flow, we select the Dim Product dataset.

In the Mapping section, we notice that only four columns are mapped automatically. The Product Group Name needs to be mapped manually. To do this, we add a new fixed mapping, select the Product Group Name column from the source, and map it to the corresponding column in the sink.

Because Product Group Name must flow through the transformations, we also need to include it in the Aggregate transformation. This ensures the data is grouped by:

Product Name

Product Group Name

Without including Product Group Name in the group-by clause, it would not appear in downstream transformations.

We also revisit the Select transformation. Previously, only two columns were selected, so Product Group Name was excluded. We update the Select transformation to include Product Group Name as well. Some changes are always expected when handling slightly different table structures, but these changes are minimal and well contained.

After these updates, Product Group Name correctly flows through to the sink.

At this point, we publish the updated data flow. This is also a good opportunity to debug and validate the logic.

When we check the pipeline run status, we notice that the second data flow (Dim Market) has failed.

We immediately inspect the error message. The error says:

Invalid object name: reporting.dim_market_name

This clearly indicates that the wrong table name was passed as a parameter. Instead of passing dim_market, the value passed was dim_market_name.

This explains the failure.

We correct the parameter value to:

Table Name → dim_market

After fixing this, we publish the changes and rerun the pipeline.

Because the pipeline and data flows are designed to be idempotent, rerunning them does not cause any issues such as duplicate data or inconsistent state.

This time, the pipeline runs successfully.

Next, we validate the data in the database.

We start with the Dim State table, and the data is populated correctly.

Then we check the Dim Market table. To easily detect duplicates, we run a query with:

ORDER BY Market_ID

The data looks clean, with no duplicate surrogate keys.

To verify the volume of data, we run a simple count query on the Dim Market table. The result shows that 1,664 market records have been loaded successfully, which aligns with expectations.

At this stage, we have successfully loaded:

Dim State

Dim Market

Prepared the logic for Dim Product

The only remaining dimension table to load is Dim Variety.

In the next lesson, we will:

Clone the existing data flow for Dim Variety

Add it to the same pipeline

Run all data flows together

Confirm that existing dimension tables remain unaffected while the new table is loaded successfully

# **M) Reusable DATAFLOW Design - Reusing to Populate DIM_VARIETY Dimension Table**

Let’s now clone the data flow for the final dimension table, which is Dim Variety, and start making the required changes.

We clone the existing data flow and rename it appropriately. Inside the Select transformation, the only change required is to replace Market Name with Variety. No other logic needs to be modified.

Next, we go to the Sink transformation and select the Dim Variety dataset, which we already created earlier.

In the Mapping section:

Map SourceFileDimColumn to the Variety column

Map the New Surrogate Key ID to Variety_ID

With this, the data flow for Dim Variety is complete.

At this point, we have created data flows for all dimension tables except the Date dimension. The Date dimension is a special case and will be handled later using a one-time load.

For now, we focus on completing and validating all other dimension tables.

All of these data flows are independent and can run individually. If we do not connect them sequentially in the pipeline, they will run in parallel. This means that at any point in time, two data flows can execute together.

However, to avoid overloading the debug cluster, we choose a balanced approach:

Run two data flows in parallel

Then run the next two

This allows us to observe performance before running everything end to end.

When we try to publish, we encounter an error. This happens because, for the newly added data flows, the Settings and Parameters have not yet been populated.

For the Settings section:

We copy the values from an existing data flow

The only tricky part is the file name

The remaining values (container name and folder name) are already known:

Container: landing

Folder: daily-pricing

We repeat this for the other data flow as well.

Next, we move to the Data Flow Parameters section.

For the Dim Variety data flow, we pass the following values using the Data Flow Expression editor:

Schema Name → "reporting"

Table Name → "dim_variety"

Lookup Column Name → "variety"
(Note: the column name is variety, not variety_name, because that is how it exists in both the source file and the database)

ID Column Name → "variety_id"

After passing these values, we save and finish.

Next, we configure the remaining data flow. At first, there is some confusion with the table name, as Dim Market was accidentally reused. We correct this and switch to the Dim Product data flow instead.

For the Dim Product data flow, we encounter a validation issue. When this happens, we use the Validate option and then click Publish All.

After publishing, the Dim Product data flow appears correctly.

Now we provide the required values for the Dim Product data flow:

Settings:

Container: landing

Folder: daily-pricing

Source file name: existing pricing file

Parameters:

Schema Name → "reporting"

Table Name → "dim_product"

Lookup Column Name → "product_name"

ID Column Name → "product_id"

At this point, all required values are passed correctly for:

Dim State

Dim Market

Dim Product

Dim Variety

We publish everything again, and this time it works without any errors.

Now the pipeline is fully configured to load all four dimension tables using the same reusable logic.

In the next lesson, we will:

Run the pipeline end to end

Validate all four dimension tables

Confirm that the reusable design works exactly as expected across all dimensions

# **N) Reusable DATAFLOW Design - Debugging Run Of Loading All Dimension Tables**

Let us now start the pipeline.

You can see that two data flows start running in parallel. Once these two complete, the remaining two data flows will automatically start. We will wait until the entire pipeline run is completed.

All the data flows have run successfully. Now let’s validate that the data has been populated correctly into all dimension tables, and also ensure that none of the existing data was affected.

Dim State Validation

We start with Dim State.

The state count is always expected to be 25, and there are no additional records.
This looks good.

Dim Market Validation

Previously, the Dim Market table had 1,664 records.
After this run, the count remains the same, which confirms that no duplicates were introduced.

Everything looks correct here.

Dim Product Validation

Next, we validate Dim Product.

We run:

SELECT * 
FROM reporting.dim_product
ORDER BY product_id;


This makes it easier to check for duplicates.

The results look good—there are no duplicate records.
A quick count confirms that 215 products are present in the table.

Dim Variety Validation

Finally, we validate Dim Variety.

We run:

SELECT * 
FROM reporting.dim_variety
ORDER BY variety_id;


The data looks clean, and a quick count confirms that all expected records are loaded successfully.

Dim Date Load

I have also loaded the Dim Date table.

This is a one-time default load, so there is nothing complex involved. I will provide the insert script for this table separately.

For Dim Date:

We generated Date_ID values for the entire year 2023

The Date_ID is created using a YYYYMMDD-style concatenation

This is sufficient for our daily pricing data

Key Observation – Manual Parameters

If you closely look at the pipeline we are running, you will notice that there is still manual intervention required when passing:

Landing container name

Folder name

Source file name

The file name is especially important.

In a real production scenario:

There can be multiple files per day

Over a year, we could easily have 365+ files

Manually updating the file name is not scalable

What’s Next

To address this, we need to automate the file discovery and parameter passing process.

Before implementing this change in the main pipeline, we will:

Perform experiments in a working lab

Validate different automation approaches

Then integrate the best solution into our pipeline

That’s what we will start working on next.

# **IX) Incremental Load ( Delta Records Processing ) - Dimension Tables Load**

# **A) Incremental Load Overview**

One of the configurations we have currently implemented while calling the data flows is passing values to the source dataset parameters by hardcoding them inside the pipeline. While this approach works from a functional standpoint, it is not considered a best practice in real-time or production-grade projects.

Passing parameters to a data flow itself is acceptable, even if those parameters are hardcoded. This is because data flows are often highly specific in nature. In our case, this particular data flow is designed to work only for the Dim State table, so there is no immediate need to parameterize the entire data flow logic. From that perspective, keeping the data flow static is fine.

However, the problem lies in hardcoding the values passed to the source dataset parameters. This approach makes the solution non-automated and rigid. In a real-time project, such configurations should be dynamic and driven by metadata or runtime values rather than fixed inputs.

At the moment, the solution is also not automated with respect to incremental loads for the dimension table. This is a key gap we need to address. Currently, there isn’t just a single file present—there are nine files already available. If we schedule the ingestion pipeline again to load additional data, the existing metadata-driven ingestion pipeline will automatically bring the new files into the landing layer.

For example, earlier we configured the pipeline trigger to run on the 10th of 2023. If we now edit the trigger and change it to the 20th of 2023, the pipeline will ingest only the additional files generated during that period. This behavior confirms that the ingestion layer is already capable of handling incremental data arrival.

The challenge now is to extend this automation to the dimension table load, specifically by dynamically passing values to the source dataset parameters. We need a mechanism that can automatically identify and process only the incremental data without manual intervention.

To achieve this, we will temporarily switch to the working labs, particularly Lab 5, where we will explore techniques to automate parameter passing for source datasets. Once we understand and validate that approach, we will come back and enhance the main pipeline to make it fully automated and production-ready.

This end-to-end enhancement will ensure that the dimension table supports true incremental loading, aligns with real-world project standards, and eliminates the dependency on hardcoded configurations.

# **B) Incremental Load - GET METADATA Activity Overview**

The requirement here is to process all files that exist under the landing container, specifically inside the daily pricing folder, on a daily basis. These files need to be passed into the dimension table data flow that we have already developed. It is important to note that both the landing container and the daily pricing folder structure are fixed and will not change throughout the project.

To achieve this, the first step is to list all the files available inside this folder and then pass that list dynamically into the data flow responsible for loading the dimension table. Once this mechanism is in place, the dimension load will work seamlessly without requiring any hardcoded values.

Before applying these changes to the final, mainstream pipeline, we will perform a quick experiment under the Working Labs folder. This allows us to validate the logic independently and avoid impacting the production-ready pipeline. For this purpose, we will create a new pipeline, which we will name Lab4A. The goal of this lab pipeline is to explore how we can retrieve a list of files from a specific folder.

To list files from a folder in Azure Data Factory, we use an activity called Get Metadata. In this lab, we will explore the different components available within the Get Metadata activity and use them to fetch the list of files stored in a folder inside a Data Lake Storage account.

Once we add the Get Metadata activity, most of its configuration can be left at the default settings. The key configuration happens in the Settings tab, where it asks for a dataset. Here, we need to create a dataset that points only to the folder, not to any specific file.

I have already created a dataset named Lab4_Source_File_List. This dataset is configured using Azure Data Lake Storage Gen2 as the storage type and Delimited Text as the format. In the file path, only the folder names—landing/daily_pricing—are specified. No file name is provided. This is a critical point because we want to retrieve metadata for all files inside the folder, not for a single file.

Once the dataset is ready, we return to the pipeline and map this dataset to the Get Metadata activity. After selecting the dataset, we move to the Field List section. Metadata, by definition, is data about data, and in our case, file-related information such as file name, type, and last modified time qualifies as metadata.

The Get Metadata activity can return several attributes, including child items, item name, item type, and last modified time. For our requirement, Child Items is the most relevant option because it returns an array containing all the files present in the folder. We select this option and run a debug execution of the pipeline.

The pipeline runs very quickly, and when we inspect the output, we can see that the Child Items array lists all files present in the folder. In this case, it correctly identifies nine files, which matches the number of files currently available in the daily pricing folder.

Now comes an additional and very important requirement. On a daily basis, these files may get updated or new files may arrive. During the first run, it is expected that all nine files are picked up. However, during subsequent runs, the pipeline should skip the files that were already processed and only pick up the newly added or updated files.

To implement this behavior, we will leverage the Last Modified Time of the files. The Get Metadata activity provides an option to filter files by last modified date. This filter requires two parameters: Start Time and End Time, both of which must be provided in UTC (Universal Time) format.

Using this filter, the pipeline will pick up only those files whose last modified timestamp falls between the given start and end times. This approach ensures that only incremental files are processed in each run.

We have already used this UTC date-time format earlier in the ingestion pipeline. For testing purposes, we can copy the same format and pass sample date values to validate the behavior. In the next lesson, we will test this setup by providing specific date ranges and confirming that only the expected files are picked up.

This experiment in the Working Labs will help us confidently apply the same logic to the final pipeline, enabling a fully automated, incremental dimension table load without hardcoded parameters.

# **C) Incremental Load - GET METADATA Activity Filter Metadata Between Dates**

To make this solution fully reusable and production-ready, we are going to pass the filter-by-last-modified start time and end time as pipeline parameters. This allows us to reuse the same pipeline logic across multiple runs and dynamically replace the parameter values at runtime. Just like we did in the ingestion pipeline, these parameter values can later be populated directly from the trigger output.

For this purpose, we will create two pipeline parameters: one for the start date and another for the end date. Initially, we will assign default values to these parameters so that we can quickly test whether the filtering logic works as expected. The goal is to verify that the Get Metadata activity correctly filters source files based on the date range we pass.

To identify appropriate test values, we navigate to the Data Lake Storage account, go to the landing container, and then open the daily pricing folder. From the file properties, we observe that the earliest file has a last modified time of 31st January 2024 at 12:05:03, and the latest one is around 12:27:14. Using these timestamps, we can design our test cases.

We will use the UTC (Universal Date Time) format, which we have already used in the ingestion pipeline. Instead of retyping it, we simply copy the format from the ingestion pipeline and use it here. For the start date, we intentionally choose a time slightly earlier so that the first file is included. For example, we might use 12:05:00 as the start time and 12:05:30 as the end time. This should ideally pick up only two files that fall within that time window.

Once the parameters are created, we need to map them to the Filter by Last Modified option in the Get Metadata activity. This is done using Dynamic Content, where the Pipeline Expression Builder opens. We bind the start time field to the start date parameter and the end time field to the end date parameter. At runtime, the pipeline will automatically take the values passed to these parameters.

Since we have provided default values, we can simply debug the pipeline without manually supplying parameter values. During the first debug run, we intentionally use the same date values we configured earlier. After the pipeline runs successfully, we inspect the output of the Get Metadata activity and confirm that only the first and second of January files were picked up. This confirms that the filtering logic is working exactly as expected.

Encouraged by this result, we perform one more test by slightly adjusting the date range. This time, we move the start time forward and extend the end time so that three files should fall within the range. Instead of modifying the pipeline logic itself, we simply change the parameter values at runtime. This highlights the true power of pipeline parameterization—we do not need to edit or redeploy the pipeline to change behavior.

Initially, the pipeline fails due to an invalid datetime value. On closer inspection, we realize that we mistakenly passed 60 seconds in the timestamp, which is not valid. As soon as seconds reach 60, they roll over to the next minute. This is a simple human error, especially when things start working and excitement kicks in. After correcting the timestamp to a valid value, we rerun the pipeline.

This time, the pipeline executes successfully. When we check the output, we can clearly see that only the third, fourth, and fifth files—the ones that fall within the specified date range—are picked up. This confirms that Microsoft’s implementation is solid and that our configuration is correct.

At this point, the solution looks very promising. However, there is still one important edge case we need to handle. If a specific date range does not contain any files, the pipeline should not fail. Instead, it should gracefully handle this scenario. We will address this exception-handling logic in the next lesson.

Once that is complete, we will return to the main pipeline and integrate everything we have built here. At that point, we will have a complete, automated, incremental mechanism to dynamically identify source files and drive the dimension table data flow without any hardcoded values.

# **D) Incremental Load - IF CONDITION Activity Overview**

Now we will test another scenario by passing a date range that does not fall within the last modified timestamps of any files. For example, we pass a start time of 01:28:00 AM and an end time such as 02:08:00 AM, and then adjust the end time further to 02:29:30 AM. Since none of the files in the daily pricing folder were modified during this time window, the Get Metadata activity should not find any matching files.

As expected, when we run the pipeline with this date range, the Child Items output comes back as an empty array. If we expand the output, we can clearly see that no file names are returned. This confirms that the filtering logic is behaving correctly, but it also introduces an important scenario that we must handle.

In a real-world pipeline, when the Child Items array is empty, we should not perform any further processing. Specifically, we should not trigger the dimension table data flow when there are no files to process. On the other hand, if the array is not empty and contains one or more file names, then we need to proceed with processing.

Since the output is an array, and it can contain multiple file names, we will eventually use a ForEach loop to iterate through each file and pass it into the dimension table data flow. This is something we have already implemented earlier in the ingestion pipeline, so we are familiar with this pattern. However, before doing that, we must first check whether the array is empty or not.

To achieve this, we introduce an additional activity called the If Condition activity. This activity will be placed immediately after the Get Metadata activity. Its purpose is to evaluate the output of Get Metadata and decide whether the pipeline should continue processing or simply exit gracefully.

The specific output we are interested in from the Get Metadata activity is the Child Items array. This array represents the list of files present under the daily pricing folder for the given date range. Inside the If Condition activity, we need to pass this Child Items output as the input expression.

When we open the If Condition activity and click on Add Dynamic Content, we can see multiple outputs available from the Get Metadata activity. Among them, we select Child Items, as that is the property we want to evaluate. This value is passed as the input to the condition expression.

Now we need to check whether this array is empty or not. Azure Data Factory provides a very useful built-in function called empty(). This function returns true if the input object, array, or string is empty, and false otherwise. Since Child Items is an array, this function works perfectly for our requirement.

So, inside the expression builder, we use the empty() function and pass the Child Items array as the argument. If the function returns true, it means no files were found, and we do not need to perform any further actions. If it returns false, it means files are available, and we should proceed with processing them.

In our case, the false path is where the actual work will happen. That is where we will later add the ForEach loop and trigger the dimension table data flow. The true path can simply end the pipeline execution without doing anything.

For now, to validate that the logic is working correctly, we will configure temporary variables in both the true and false paths. This will help us confirm whether the pipeline is correctly identifying empty and non-empty scenarios during execution.

Once we validate this behavior in the Working Labs, we will return to the main pipeline and implement this logic as part of the automated, incremental dimension table load. In the next lesson, we will test these conditions in detail and finalize the implementation.

# **E) Incremental Load - IF CONDITION Activity For EXCEPTION Handling**

To verify whether the pipeline execution is going through the true or false path of the If Condition activity, we will use a simple validation approach by setting a variable. This helps us clearly understand whether the condition logic is working as expected during runtime.

When we click the Edit button on the If Condition activity, it opens a sub-window, similar to how the ForEach loop works. From this sub-window, we can configure the activities for both the True and False branches. At any point, we can return to the main pipeline by clicking the breadcrumb navigation, and similarly, we can revisit the If Condition sub-window by clicking the Edit button again.

Inside the True branch, we add a Set Variable activity. Since we have already used this activity earlier, it should be familiar. Here, we quickly create a pipeline variable named condition_output with the data type set to String. If the condition evaluates to true—meaning the Child Items array is empty—we set this variable’s value to "true". This confirms that no files were found for the given date range.

Similarly, inside the False branch, we add another Set Variable activity. We use the same variable, condition_output, but this time we set its value to "false". This indicates that the Child Items array is not empty and that files are available for processing.

Once both branches are configured, we rerun the pipeline to test the behavior. For this test, we intentionally pass a date range outside the last modified timestamps of all files—for example, a start time of 02:08:00 AM and an end time of 02:29:30 AM. Since no files fall within this range, the Get Metadata activity returns an empty Child Items array.

This output is then passed to the If Condition activity. As expected, the condition evaluates to true, and the pipeline executes the True branch. The variable condition_output is set to "true", confirming that the logic is functioning correctly.

This validation is important because, in our actual implementation, the False branch is where meaningful processing will occur. Only when files are available should we trigger the ForEach loop and run the dimension table data flow. If the array is empty and we skip this check, the pipeline would attempt to process non-existent files and fail with a source file not found error.

By introducing this conditional check, we are proactively handling the error before it occurs. This makes the pipeline more robust, reliable, and production-ready. With this validation in place, we can confidently move back to the main pipeline and integrate this logic into the incremental dimension table load process.

# **F) Incremental Load - ADF Single Pipeline Limitations & Workaround(Multi Pipeline)**

Once we have validated that the If Condition activity is working correctly, the next step is to process the files returned by the Get Metadata activity. For this, we need to use the ForEach activity. Since the Get Metadata activity outputs an array of files, the ForEach loop allows us to traverse this array one file at a time, passing each file individually into the dimension table data flow.

To demonstrate this, we first run the pipeline with a valid start date and end date that matches the last modified timestamps of actual files. Using our default test values, the Get Metadata activity returns two files, confirming that the Child Items array is not empty. Consequently, the pipeline follows the False branch of the If Condition, and the condition_output variable is set to "false". This is exactly the scenario we want, because files are available for processing.

Now, within the False branch, we need to call the ForEach activity to iterate over the array. It is important to note that we cannot directly pass the entire array to the data flow parameters in a single operation; each file must be processed individually. The ForEach activity allows this sequential or parallel processing.

However, Azure Data Factory has a limitation that we must be aware of: we cannot nest a ForEach activity directly inside an If Condition if that If Condition is in the same pipeline. Similarly, nested If Condition activities are disabled by default. This means that we cannot directly create a ForEach loop inside the False branch of an If Condition within the same pipeline.

To overcome this limitation, the recommended approach is to create an additional pipeline. The parent pipeline handles the Get Metadata and If Condition logic, and when files are available, it passes the file list as pipeline parameters to the child pipeline. The child pipeline can then safely iterate over the files using a ForEach activity and trigger the dimension table data flow for each file.

In the next lesson, we will implement this solution in detail, creating the child pipeline and passing the necessary parameters from the parent pipeline. This approach ensures that we handle multiple files efficiently while respecting the limitations of Azure Data Factory. For now, it is important to understand this design pattern as a standard way to process arrays conditionally in a modular and reusable manner.

# **G) Incremental Load - Calling and Passing Values Between Parameters**

During the testing process, we realized that some temporary variables, like source file name, were accidentally created and appeared as duplicates. Since these set variables were only used for testing the passing of values between pipelines, we deleted them to keep the pipeline clean. No set variable activities are needed in the main or new pipelines for the production workflow. Once the unnecessary variables were removed, we successfully published the pipeline changes.

The main pipeline now begins by reading the list of files in the landing folder. The Get Metadata activity retrieves the Child Items array, which contains the file names. If the array is empty, we do not perform any further actions. If it contains files, we would ideally process each file individually. However, due to Azure Data Factory limitations, we cannot directly use a ForEach activity inside an If Condition in the same pipeline.

To overcome this limitation, we created a sub-pipeline. The main pipeline passes the Child Items array as a pipeline parameter to this sub-pipeline. The sub-pipeline then iterates over each file using a ForEach activity, allowing the dimension table data flow to process each file individually. During testing, we confirmed that this approach works as expected: with two files in the landing folder, the If Condition evaluates to False, the main pipeline calls the sub-pipeline, and the ForEach activity in the sub-pipeline runs two iterations, processing each file separately.

This setup demonstrates a fully automated workflow:

Automatic identification of files in a folder using Get Metadata.

Conditional execution using the If Condition activity to handle empty or non-empty arrays.

Error handling, avoiding failures when no files are available.

Passing values between pipelines via pipeline parameters to work around ADF limitations with nested loops.

Iterative processing in the sub-pipeline using ForEach to call the dimension table data flow for each file.

In practice, this means the master pipeline reads the files from the landing folder, checks if any files exist, and passes them to the sub-pipeline. The sub-pipeline then uses a ForEach loop to run the data flows for the dimension table load. Only the file names change for each run; the container name and folder name remain constant.

This modular, multi-pipeline approach is crucial for real-time, production-ready ETL workflows, where multiple files must be processed dynamically. By splitting responsibilities across pipelines and using parameters, we can handle complex scenarios efficiently while keeping the design clean, reusable, and error-resilient. In the next lesson, we will implement this fully with the reporting dimension table load, completing the end-to-end incremental load process.

# **H) Incremental Load - Designing Reporting Tables Load Master Pipeline**

We will start by using the Fourier pipeline as a reference to create a new, master pipeline for the reporting table load. Initially, the goal was to run the dimension table load directly. However, during the development of the Fourier pipeline, we discovered a limitation in Azure Data Factory: we cannot directly implement a ForEach activity inside an If Condition. To handle this, we will create a parent (master) pipeline that will call the reporting dimension table load pipeline. All additional logic and checks will be implemented in this master pipeline.

To speed up development, we clone the data set we previously created, instead of creating it from scratch. We remove any lab-specific suffixes, so it can be used directly in the new master pipeline. After publishing these changes, we move the dataset from the Working Labs folder into the Transform folder, aligning it with our production structure.

The new pipeline is created and named RPL_Load_Reporting_Tables, which is designed to handle both dimension and fact table loads, since the same source files feed both types of tables. The first activity in this pipeline is the Get Metadata activity to list files in the landing folder. We ensure proper naming conventions and configure it to refer to the source file list dataset we cloned.

Next, we create pipeline parameters for start date and end date. These parameters allow us to filter files on a daily basis based on their last modified timestamp. We reuse the logic from the ingestion pipeline, which automatically passes trigger values to the pipeline parameters at runtime. The dynamic content for start date and end date is mapped to these parameters, enabling filtering without hardcoding values.

The Get Metadata activity now lists files from the landing container that fall within the specified date range. The output is captured in the Child Items array, which contains all file names that match the filter. If no files are found for the given date range, the array will be empty. To handle this scenario, we add an If Condition activity immediately after the Get Metadata activity. This condition evaluates whether the Child Items array is empty, preventing unnecessary failures or errors.

Inside the If Condition, we use the empty() function, which returns true if an array, object, or string has no values, and false if it contains data. We pass the Child Items array from the Get Metadata activity as input to this function. If the array is empty (true), the pipeline does nothing. If the array contains files (false), we proceed to the next step: calling another pipeline to process these files.

In the False branch of the If Condition, we add an Execute Pipeline activity to call the existing dimension table load pipeline. We pass the Child Items array as a pipeline parameter to this called pipeline, enabling it to iterate over the files and process them one by one. This modular approach ensures that each file is handled individually while respecting ADF’s limitations with nested loops.

In the next lesson, we will configure this Execute Pipeline activity in detail and complete the implementation for loading the reporting tables. By separating the master pipeline from the dimension table pipeline, we achieve a flexible, reusable, and production-ready workflow, capable of handling multiple files, dynamic dates, and incremental loads efficiently.

# **I) Incremental Load - Calling Reporting Dimension Load From Master Pipeline**

Inside the False branch of the If Condition activity, we add an Execute Pipeline activity to call the dimension table load pipeline. This step is necessary because we only want to process files when the Child Items array from the Get Metadata activity is not empty. To make it clear which pipeline is being invoked, we set the description of the Execute Pipeline activity to indicate that this is the actual pipeline being called. This helps avoid confusion when reviewing the pipeline later.

Before passing values to the invoked pipeline, we need to ensure that the called pipeline has the necessary pipeline parameter. In the dimension table load pipeline, we create a new parameter called pipeline_parameter_source_files_list and set its data type to array, as it will hold the list of files coming from the parent pipeline. Once the parameter is created, we publish the pipeline to make the parameter available.

Back in the master pipeline, we map the Child Items array from the Get Metadata activity to this newly created pipeline parameter using dynamic content. This ensures that the array of files retrieved from the landing folder is passed to the dimension table load pipeline. Opening the dimension table load pipeline confirms that the array is received correctly, containing all files to be processed.

To process each file individually, we use a ForEach activity inside the dimension table load pipeline. The input to the ForEach activity is the pipeline parameter containing the array of file names. Each iteration of the loop will process a single file. This allows us to map the individual file names to the parameters of the data flows that load the dimension tables.

At this stage, we organize the pipeline by moving all existing data flow activities inside the ForEach loop. This ensures that each file in the array is processed sequentially (or in parallel if configured), and the file-specific parameters are passed correctly to the data flows. In the next lesson, we will focus on mapping the ForEach iteration output to the data flow parameters, completing the incremental load process for the dimension tables.

# **J) Incremental Load - Using Master Pipeline GET METADATA output in Child Pipeline**

We have now included a ForEach activity in the dimension table load pipeline to iterate over the array of file names coming from the master pipeline, which in turn is the output of the Get Metadata activity. The pipeline parameter holding this array is mapped as the input to the ForEach activity, allowing it to process multiple files dynamically. In the settings of the ForEach activity, we specify the items property to use this pipeline parameter, which ensures that all array values—whether coming from metadata or another pipeline—are processed sequentially.

Inside the ForEach loop, we place all the data flow activities responsible for loading the dimension tables. When copying these activities into the ForEach loop, the connectivity between them needs to be re-established, which is straightforward. For each data flow, the landing container name and folder name are constant, so we create pipeline parameters for them to avoid hardcoding. The landing file name, however, comes dynamically from the current iteration of the ForEach loop, accessed via item.name in the dynamic content. This ensures that each file in the array is processed individually.

By parameterizing the container name, folder name, and source file name, we remove hardcoded values from the data flows, making the pipeline flexible and reusable. These parameters are mapped to the respective fields in each data flow. If any of these values change in the future, we only need to update the pipeline parameters rather than editing each data flow. This is a best practice for building scalable, maintainable ETL pipelines in Azure Data Factory.

Once all mappings are complete, we publish the changes and prepare for testing. Before executing the pipeline, only the pipelines currently being worked on are kept open to avoid confusion. During debug, the pipeline prompts for the start and end date parameters, which are used to filter files in the Get Metadata activity. The filtered list of files is then passed to the master pipeline, which invokes the dimension table load pipeline. The ForEach activity iterates through this list, and the data flows process each file individually.

This approach effectively handles dynamic, incremental file processing while respecting ADF’s limitations with nested loops and hardcoding. The next lesson will focus on testing the end-to-end flow and verifying that files are processed correctly through all layers of the pipeline.

# **K) Incremental Load - Debugging Dimension Tables Load Part 1**

I would like to start the testing with reading these two files. So I’m setting the start date and end date based on these two time values. When you click Debug, it will ask whether to use the Integration Runtime, and it will ask for the values for the start date. I am passing my start date value as 0120500, so it will pick up the first file, and the ending value as 2530 so it will pick up the second file. These two files will then be passed to the Reporting Dim Table Load pipeline, and the execution will kick off. We will be able to monitor how the run progresses and debug any errors that may occur.

The Get Metadata activity runs first and identifies the childItems, which includes the two source files. This is expected. Next, the If Condition activity evaluates whether the array of files is empty or not. Since the array is not empty, it evaluates to False and triggers the Execute Pipeline activity, calling the pipeline responsible for loading the dim reporting tables. If you want to see the run for this pipeline, you need to open it in a different window via the pipeline run ID link, as it runs separately from the master pipeline.

Inside the ForEach activity, the pipeline is processing the two files simultaneously. By default, the ForEach activity runs in parallel if the sequential setting is not enabled, which is why both files are being executed together. If sequential execution is required, this setting can be enabled to process files one after another. The data flows then begin processing, starting with the dim state tables. Each data flow is responsible for loading the specific dimension table data from each source file.

While monitoring, I double-checked the naming conventions and everything is correct. The first file (0102_2023.csv) is being processed alongside the second file (0101_2023.csv). The logging details show the exact file being loaded at each step. Given the amount of work being executed for each file, it may be better to run them sequentially to avoid overwhelming the system.

It’s important to note that the database is serverless, meaning it runs on-demand and is not tied to a specific server. Sometimes, when connecting for the first time, it may appear unavailable, but re-trying will start the server and allow the connection. This is normal behavior, so we don’t need to be concerned.

I have stored some of the SQL queries used during yesterday’s work. These can be reused to validate the data loaded into the tables or to truncate tables before re-running the pipeline. These queries will also be included in the resources section of the Udemy course for convenience.

For data validation, I am checking the counts of rows in each dimension table. For example, dim_market currently has 1664 records. This ensures that multiple pipeline runs do not corrupt existing data and that new markets, products, or varieties in these files are loaded correctly. Similarly, dim_variety has 417 records. After the pipeline run completes successfully, we can recheck these counts to ensure everything has been loaded correctly.

The pipeline run may take some time, so we will give it a moment to complete. Once finished, we will analyze the loaded data to confirm that everything is functioning as expected and no existing data has been affected.

# **L) Incremental Load - Debugging Dimension Tables Load Part 2**

As expected, the pipeline run failed. That’s okay. Going through these errors during this training is valuable because it makes you future-proof—you’ll know what to look for and where to investigate if similar issues occur later. Both of the data flows failed, and the error message indicated that the path daily pricing/<file_name> does not exist.

On closer inspection, the issue is with the folder name. In the container, the folder is actually named daily-hyphen-pricing (with a hyphen). This is a simple fix, and because we used pipeline parameters for the folder name, the change is minimal. I just needed to update the pipeline parameter to match the correct folder name.

Additionally, I decided to run the ForEach activity sequentially. Previously, it was running all four data flows for the two files in parallel, which was overloading the debug cluster. Running sequentially reduces the workload on both Data Factory and the SQL server. For testing, I set the default start and end values to 20500 and 2530, respectively.

After making these changes, I reran the pipeline using the integration runtime. The Get Metadata activity successfully picked up the two files, and the If Condition evaluated to False, which correctly triggered the sub-pipeline. I monitored the sub-pipeline, and it ran through all the activities without any issues. The four data flows executed sequentially for the two files—one for the 1st of January 2023 file and the other for the 2nd of January 2023 file.

Everything is looking very promising now. Since the sub-pipeline is being called from the main pipeline, we only need to include a trigger for the main pipeline to automate the load. The sub-pipeline does not need a separate trigger.

Finally, I checked the database tables to validate the data. Both files were successfully loaded. The counts in the dim_market and dim_product tables remained unchanged, which confirms that the existing data was not disturbed. Some new data was loaded into the dim_variety table, as expected. In the next lesson, we will configure the tumbling window trigger to automate this process further.

# **M) Incremental Load - Configure Tumbling Window Trigger**

Let's start creating the new tumbling window trigger for the main pipeline we developed today. I am going to include a tumbling window trigger because the date values in the existing files are in the past, and we cannot use the schedule trigger here. I will name it tumbling_window_trigger_daily_reporting_tables_load.

I want to start processing from the third file, because the first two files have already been processed. This avoids wasting resources. The start time will be set to 31st January 2024, 01:00 AM to 05:30 AM. This ensures that the trigger picks up the remaining files and loads the data into the dimension tables.

For the duration, I initially considered running it for one day, but to cover all files, I will set it for a 24-hour window. The end date is set as 1st February 2024, 21:00, because we do not have any files after 31st January 2024 yet. Later, we can extend the end date as more data becomes available.

In the advanced settings, I set the trigger to run sequentially because running multiple windows concurrently can overload the debug cluster and data flows. This ensures that each data flow runs one after another, reducing system load. Once I set the start and end date values using the trigger system variables (WindowStart and WindowEnd), the trigger will pass these values to the Get Metadata activity. This will determine the list of files to process and start loading them accordingly.

After publishing the trigger, it will start running immediately in the Monitor section. Since the date range is in the past, it will process all files within the given 24-hour window. The pipeline will start reading the files beginning from the first file (20:500), which means the first file may get reprocessed, but the data flow protections prevent duplicates.

While this pipeline is running, I will go back to the ingestion pipeline to start loading any remaining data files from the HTTP web server. This will ensure the two processes can run simultaneously without conflicts. Once this run completes, we can check the logs to confirm that all files have been processed without errors.

In the next lesson, we will review the run details of this pipeline and begin ingesting additional data into the landing layer. We will also discuss performance tuning options, because loading around 12,000 records currently takes about 10 minutes, which is slower than desired. We will explore ways to optimize the data flow performance.

# **N) Incremental Load - Test Tumbling Window Trigger Run**

I went back quickly to check on our trigger. It’s running fine, and the trigger run has completed successfully. The total load time was about 19 minutes, which is reasonable considering that almost 9 or 10 files ran through together. I was a little surprised at the speed—it ran very smoothly. Using the integration runtime ensures that everything processes correctly and efficiently.

Next, I checked the database to verify the results. The record counts are consistent, and new records have been loaded correctly. For example, the dim product table received a few new records, and the dim market table had minimal changes. Most importantly, the dim variety table got updated with the new files, which is expected. There were no discrepancies or unexpected changes in the data.

Overall, everything is working fine. The pipeline and the tumbling window trigger are processing files correctly, and the data is loading as intended. We are now ready to move on and load additional files into the landing layer using the ingestion pipeline in the next lesson.

# **O) Incremental Load - Fixing Data Quality Error on DIM_VARIETY Table Load**

I realized that there was an issue with the dim variety table. Although the table was loading, it was inserting empty strings into the variety values after yesterday’s run. These were not null values, but actual empty strings.

To fix this, I included an additional filter condition in the pipeline. Since we were already checking for not null values in the joiner, there was no chance of null values coming through. Along with that, I added a condition to check that the length of the source column value in the dim file is greater than one. This ensures that any empty strings are discarded.

I then reran the pipeline specifically for the dim variety load. After this change, the issue was resolved, and no new empty records were loaded into the table.

# **P) Loading DIM_DATE Dimension Table - Using INSERT STATEMENTS**

Just gave a query to load "DIM_DATE Dimension Table" using INSERT Statement

# **Q) Data Ingestion Pipeline - HTTP Source Full Load Using Tumbling Window Trigger**

Okay, let's start by removing the existing trigger. Before removing it, I want to copy one value that I will need to pass back later. When removing the trigger from the pipeline, note that we are detaching it, not deleting it completely.

We are going to create a new tumbling window trigger and call it tumbling_window_trigger_daily_pricing_ingest_new. This trigger needs to start from January 10th, 2023, at 12:00 a.m., and run up to December 22nd, 2023, because these are the dates for which source files are available.

I adjusted the start and end times to 00:00:01 a.m. for January 10th and the appropriate end time for December 22nd, 2023. I also set the concurrency to 10 files, so it will process ten days’ worth of files simultaneously into the landing layer.

After publishing, the trigger started running immediately. It is initiating ten instances of the pipeline at the same time, which means that within the next 1–2 hours, all files available in the HTTP web server should be copied into the landing layer.

Once the files are copied, we will trigger the dimension table load to process this data into the dimension tables. Before that, we will focus on loading the fact table. Note that the data flow for the fact table (PAC table) load has not been developed yet, and we will cover that in the next section.

# **X) Fact Table Load DATAFLOW Design**

# **A) Fact Table Load Transformation Overview**

Let's start by looking into loading the fact table. If you ask me, the easiest way to load data into the reporting database is probably through the fact table load. This is because loading dimension tables requires many checks before making any decisions. Fact table data, on the other hand, needs to be inserted every day as it captures mostly changes in the source data, such as quantity of arrival, minimum price, and maximum price. The fact table is loaded on a daily basis, and you mainly need to insert records without worrying about whether the record already exists or not. Those types of existence checks are not needed here.

We will quickly produce the source-to-target mapping document for the fact table and then move into the data flow development. After that, we will create a new pipeline and include it in the incremental load pipeline that we developed for loading the reporting tables.

The columns with a blue background come from the source file, and our source for the fact table is the same as for the dimension tables. So for four columns, we can copy the source location and source file details directly. The column names are exactly the same as the ones defined in the dimension tables, so mapping is straightforward. There are no transformation rules for these columns, as they have a 1-to-1 mapping from source to target.

The main focus, however, is on the ID columns. One ID column that was initially missed is date_id, which also needs to be included in the fact table. In the original modeling, we created the date dimension by default but forgot to include date_id. The values for this ID already exist in the dimension tables.

There are two sources for these columns, but the main one is the source file. For instance, the state_name column from the source will be used to look up the dim_state table in the reporting database to identify the surrogate key ID created in the dimension table. This lookup approach will be applied to all dimension tables, with only the source column name and the ID column being extracted changing for each case.

We will follow the same process for all remaining ID columns. Most of the columns will be read from the source, such as state_name, market_name, and product_name. The state_name column is already copied, so next we will copy the market_name and product_name columns.

For date_id, the source column data_pricing will be read and looked up against the dim_date table. A similar operation will be applied for other IDs, such as market_id, product_id, and variety_id, using their respective dimension tables. Only the source column name and the dimension table used will change for each case.

Finally, the last two columns, dw_created_date and dw_updated_date, are derived from the system date value. Once the transformation rules are clear for each ID column and the remaining columns, we can start creating the data flow. In the next lesson, we will also identify the datasets needed to build the data flow for this fact table load.

# **B) Fact Table Load DATAFLOW - Configure Source File**

Switching over to Azure Data Factory, the source file for the fact table will be the same one used for loading the dimension tables. In ADF, navigate to the Data Flows section under the actual folder and start developing the data flow there. Begin by creating a new data flow and name it load_reporting_fact_daily_pricing_table.

Next, we will include the source. The proper source file is already available under the transform folder, pointing to the landing source. Copy the complete dataset name carefully because we have multiple datasets now. Make sure the source is properly parameterized and ready to read daily pricing data.

When reading the source, the only column to exclude is origin, as it does not have proper data across source files and does not carry any significance. Apart from that, almost all other columns are required to load the fact table. To exclude the column, select the fact table columns and deselect the origin column.

The next important step is to identify the ID column values from the dimension tables. For example, the dim_state table needs to be included in the same data flow to look up source state_name values against the state_name values in the dimension table.

We will create the necessary datasets for these dimension tables in the next lesson to complete the data flow.

# **C) Fact Table Load DATAFLOW - Configure Dimension Table Source & LOOKUP SurrogateID**

We already have the dataset for the dim_state table, but it is currently used as a sink in the existing data flow. A key rule to remember in Azure Data Factory is: if a dataset is used as a sink, do not use it as a source. This is because the properties you set for a dataset when using it as a sink may not apply correctly if you try to use the same dataset as a source. So, never try to use a sink dataset as a source.

To handle this, we can clone the dataset. I created a new dataset named dim_state_lookup, which will be used in the data flow to look up data from the dimension table. I then added a second source to the data flow using this new dataset. This ensures that we have only one dataset dedicated for lookup purposes.

Once the dataset is selected, the projection automatically includes all columns from the dimension table. However, for the fact table load, we only need the state_name column. We could write a query to select only that column, but since there are minimal transformations, we can use a simple Select transformation to keep only the required column. No other columns are needed for this fact table because each fact table may have different architecture and components, so we want to keep it clean.

With the state_name column ready, we perform a lookup transformation. The lookup matches the state_name coming from the source with the state_name from the dimension table. To avoid confusion, I renamed the column from the dimension table to lookup_state_name. This consistent naming ensures clarity in mapping.

From this lookup, we extract the state_id. Initially, there was a small mistake where I only mapped the state_name, but without extracting the state_id from the lookup, we wouldn’t be able to populate the ID in the fact table. After fixing the mapping, the column is renamed to lookup_state_id for consistency. The lookup now matches the source state_name with lookup_state_name and returns both lookup_state_name and lookup_state_id. Before loading into the final target fact table, we can exclude the lookup_state_name column since it’s not needed in the target.

This process is completed for the dim_state table. A similar operation is required for dim_market, dim_product, and dim_variety. Additional datasets will need to be created for these three tables. In the next lesson, we will create those datasets and make the necessary transformations to bring in all the ID column values as defined in the transformation rules so that the fact table can be fully loaded.

# **D) Fact Table Load DATAFLOW - Configure All Dimension Tables & LOOKUP SurrogateIDs**

Let's start by creating the source datasets for the remaining dimension tables. We can use the clone feature in Azure Data Factory to simplify this. At the end of each cloned dataset name, we include the word source to indicate that it will be used as a source in the fact table data flow. This is done for the product and variety dimension tables as well, so now we have three additional source datasets ready: dim_market_source, dim_product_source, and dim_variety_source.

Next, we return to the data flow to create the additional sources. We start with market_source. Select the dim_market_source dataset and check the projection, which brings in market_name and market_id. To clean up, we use a Select transformation to exclude unnecessary columns such as created_date and deleted_date. We then rename the columns to lookup_market_name and lookup_market_id to avoid confusion with columns in the main source file.

After that, we create a lookup transformation for market name. The logic is straightforward: the primary stream comes from the main source file, and the lookup stream comes from the market lookup dataset. The lookup matches market_name from the source against lookup_market_name and brings back lookup_market_name and lookup_market_id. The lookup_market_name column will not be mapped to the final fact table and can be excluded in the final select transformation.

Next is the product dimension. We add the dim_product_source dataset as a new source. The projection includes product_name, product_group_name, and product_id, but for the lookup, we primarily need product_name and optionally product_group_name for accuracy. Using a select transformation, we rename the columns to lookup_product_name and lookup_product_group_name. We then add a lookup transformation to match the product name and product group name from the source against the lookup dataset, returning lookup_product_name, lookup_product_group_name, and lookup_product_id. Proper naming conventions here are crucial to avoid errors and make debugging easier since the same column names appear across multiple sources.

Finally, we handle the variety dimension. Add the dim_variety_source dataset as a new source. The projection includes the relevant columns, and we use a select transformation to keep only variety_name and variety_id, renaming them to lookup_variety_name and lookup_variety_id. A lookup transformation is then used to match variety_name from the source against the lookup dataset, returning the required lookup columns.

At this stage, all the ID columns required for the fact table, except for date_id, have been brought in through the lookup transformations. The date_id column will be included in the fact table in the next lesson, as it was not yet added to the data flow.

# **E) Fact Table Load DATAFLOW - Configure DATE Dimension Table & LOOKUP SurrogateID**

If you notice, we never created the dataset for the date dimension because it is outside the existing data flow; it was uploaded manually. I will provide the data for the dim_date table, but to load the fact table, we need the date_id. To handle this, we can quickly replicate the dim_state dataset and re-import the date_name columns. I created a new dataset named dim_date_source and updated the source table name to the dim_date table instead of dim_state. Then, I cleared the schema and imported the schema from the dim_date table. This dataset will be used in the data flow to match the data_pricing values coming from the source against the dim_date table.

Next, in the data flow, we added the dim_date_source as a new source named dim_date_lookup. We only have one source column for this table. Using a Select transformation, we keep only the relevant columns, renaming data_pricing as lookup_data_pricing and date_id as lookup_date_id, while deleting the unnecessary columns.

It is important to note that the column data_pricing coming from the source file is in string format, whereas the lookup value in the dim_date table is in date format. To avoid errors during the lookup transformation, we need to convert the source data_pricing value into a proper date format before joining with the dim_date table.

To do this, we add a Derived Column transformation. We create a new column named data_pricing_formatted and use the date conversion function to convert the string value from the source into a date. When specifying the format in ADF, note that the month is represented by a capital M in the function. Based on the data preview from the debug cluster, the source data_pricing is in ddMMyyyy format.

After converting the column, we can use data_pricing_formatted for the lookup with the dim_date table in the data flow. While debugging, it is important to ensure that the correct parameters are passed to the data flow debug cluster. If the wrong parameter is passed, you may need to disable and re-enable the debug cluster to reset the values.

Once the conversion and debug are complete, the data_pricing_formatted column can be used in the lookup transformation to retrieve the date_id from the dim_date table. The actual lookup transformation and mapping will be handled in the next lesson.

# **F) Fact Table Load DATAFLOW Debugging and Fixing Data Issues**

I quickly identified the Reset Debug Settings option in Azure Data Factory. By going there, you can access the saved parameters and correct any values that were passed incorrectly. After updating the parameters, the data preview should work properly. Now, the pipeline tries to bring the full source data from the source file, including all the transformations applied so far.

At this stage, we have converted the source data_pricing column into the proper date format so that it can be joined with the dim_date table. The derived column is part of the main stream, and we use it to look up the data_pricing values against the lookup column in the date dimension to retrieve the date_id. Initially, the data preview did not show any errors, but the lookup did not return the expected date_id values.

On inspecting, we realized that the issue was with the date format in the derived column transformation. Originally, we used ddM as the format, but the source file provides the date in Mddyyyy format. This mismatch caused all date_id values to come as null. By correcting the derived column format to MMddyyyy, the lookup started returning the correct date_id values. This highlights the importance of ensuring the source format matches the expected format for lookups.

Next, it is critical to ensure that none of the ID column values returned from the lookups are null. For example, some lookup_market_id values were null because of extra spaces in the source or lookup table. To fix this, we used the Trim function in the Expression Builder to remove any leading or trailing spaces from both the source and lookup columns. This ensures proper matching between the source values and the dimension table values.

After applying the trim function and checking the derived column, all lookup ID values, including lookup_date_id, lookup_state_id, lookup_market_id, and others, are correctly populated. This confirms that the pipeline transformations are working as expected, and the fact table can now be loaded without missing or null ID values.

# **G) Fact Table Load DATAFLOW - Configure SINK Transformation**

It looks like the issue with some market names was intermittent, because when I selected those specific market names from the dim_market table, the lookup returned the correct market_id and market_name. I checked other records as well, and everything appeared fine. Therefore, we don’t need to worry too much about this; running the end-to-end pipeline will likely resolve such intermittent issues.

Now we can map all the values into the fact table. There are two columns we need to derive: dw_created_date and dw_updated_date. Both can be mapped using a derived column transformation with the current date value function. For the fact table, we don’t need to perform a lookup because each day’s file contains all pricing information. Every day’s data should be fully loaded into the fact table without checking if it already exists.

Next, we create a select transformation to exclude unnecessary columns. Only the fact table mapping columns should remain. We remove the extra columns coming from the lookup tables, such as lookup_state_name, lookup_market_name, lookup_product_name, product_group_name, lookup_variety, and data_pricing_formatted. Some columns like lookup_date_id are still needed. Keeping unnecessary columns during debugging is useful, but they can be excluded in the final pipeline once everything works correctly.

After that, we create the sink for the fact table. I duplicated one of the dimension table datasets, renamed it to fact_daily_pricing, and updated the actual table name in the schema. All columns, including date_id, are now available. In the data flow, we include this sink to load the fact table. In the sink settings, we choose Insert only and leave other options as default.

In the mapping section, we uncheck auto-mapping to manually map all columns. Some columns like state_id and lookup_state_id required manual mapping because their names did not exactly match. This is a good exercise to practice manual mapping, similar to what we’ve done previously for missing columns. The source columns for minimum, maximum, and modal pricing are coming from the source file correctly.

Finally, we ensure that dw_created_date and dw_updated_date are included and properly renamed in the select transformation. Any changes to column names prior to the select transformation need to be reflected within the select transformation itself. Once all mappings are correct, the data flow is ready. We can publish the changes and run the pipeline in the next lesson.

# **H) Fact Table Load DATAFLOW Testing Part 1**

We are going to use the same pipeline that loads the reporting tables to also run the fact table data flow. This works well because the pipeline already has proper logic to identify new files from the landing folder and check whether the folder is empty or not. It also calls the dimension table load pipeline and uses a ForEach activity to iterate through each file and load it into the dimension tables.

To run the fact table load, I created a new pipeline by cloning the dimension table pipeline. In this new pipeline, I replaced the data flow with the fact table data flow that we just created. All parameters, including container name, folder name, and item names from the ForEach activity, remain the same because we are using the same source files. This allows the fact table load to work with the same logic for identifying source files as the dimension table pipeline.

Next, I included the fact table load pipeline in the main master pipeline, which previously only called the dimension table load pipeline. I added a new Execute Pipeline activity for the fact table load and passed the necessary parameters, especially the source file list coming from the Get Metadata activity. The logic for processing files is identical to the dimension table load pipeline.

Since the dimension table load has already been run, I deactivated that activity temporarily to test only the fact table load. After publishing the pipeline, I started debugging it. I configured the debug to start from the first files (from January 1st, 2023) because no data has been loaded into the fact table yet. The debug run successfully called only the fact table data flow.

The Get Metadata activity confirmed that the correct files are being processed in order, and the fact table load ran as expected. After the debug run, we can check the output in the fact table. Initial checks showed that the data is loaded properly, but some market_id values were null in certain rows. This mirrors the behavior we observed during the data flow debug.

Before enabling the tumbling window trigger to load a year’s worth of data, we need to investigate the null market_id values. Running a query like SELECT COUNT(*) FROM dim_market WHERE market_id IS NOT NULL shows 158 valid records, but many others are null. This issue needs to be resolved before the end-to-end load can be executed to ensure data integrity in the fact table.

# **I) Fact Table Load DATAFLOW - Add Tumbling Window Trigger**

The fact table load ran successfully. As suspected, the earlier issue was intermittent, because no market_id values were null in the target table this time. The fact table now contains two days’ worth of data and is ready to be scheduled via a tumbling window trigger.

Next, we went to the main pipeline to review the existing tumbling window trigger. I disabled the data flow debug and edited the trigger that was previously used for daily reporting loads. The earlier trigger had a start time of January 31, 2024, at 1:25 a.m. Since changing the end date didn’t work properly, it was better to create a new tumbling window trigger with the same start date so that all historical data would be processed correctly.

The landing container already contains one year’s worth of data, ingested from the HTTP web server. Each file is approximately 1–1.22 MB, and all files are ready to be loaded into the fact table. The new tumbling window trigger ensures the fact table load runs end-to-end without affecting previously loaded dimension tables.

We stopped the previous trigger for reporting table loads to avoid duplicate execution. In the main pipeline, the old trigger was detached, and a new trigger was created, named tumbling_window_trigger_daily_reporting_table_load_new. The start time was set to January 31, 2024, at 1:25 a.m., and the end time was set to the current time. Initially, the frequency was set to run every 15 minutes, but it was later reduced to every 5 minutes because a large number of files were copied within a short window.

In the advanced settings, concurrency was set to one to avoid processing multiple files simultaneously. This ensures stability when hundreds of files are being ingested at the same time. Additionally, the pipeline parameters were set to pass the tumbling window trigger outputs, using the trigger’s start time as the pipeline start date and the trigger’s end time as the pipeline end date.

Finally, the trigger was published. This setup will load the fact table for all historical files without modifying the dimension tables, which remain unchanged with the same product names, states, varieties, and market names. Monitoring confirms that the fact table load has started, and over time, all files up to December 22, 2023, will be processed and loaded into the fact table.

# **J) Fact Table Load DATAFLOW - Testing End to End Reporting Database Load**

The fact table trigger run has been completed successfully. Over the course of this run, we managed to load around 350 days’ worth of files into the reporting database. Querying the fact table shows that nearly half a million records have been inserted, which is impressive for this volume of data. All ID columns are populated properly, except for a few known issues with the variety ID, the date ID, and the state ID, which we investigated further.

When checking for null values in the ID columns, everything is coming through correctly, except for the variety ID. This is expected because some records in the source have empty spaces, which cause the null values. Importantly, the key IDs that are crucial for reporting—product, market, and state names—are all populated correctly. The date ID is also populated properly, and only a very small fraction of records (around 2,000 out of 400,000) have missing variety IDs. This is an acceptable percentage, considering it stems from the source data quality, not the ETL process.

All dimension tables have been loaded with a year’s worth of source data, and the fact table is also fully loaded with year-long data. The reporting database is now fully prepared for end users to start analyzing and generating reports. This is a significant milestone and marks the completion of the development for the reporting database.

The next steps involve making configuration changes and code adjustments to ensure that the ETL code can be deployed to subsequent environments. This will be covered in the coming sections. Successfully reaching this point in the project is a major achievement—it completes a key part of the course objectives and sets the stage for the next phase.

The next phase will focus on designing and loading the data lake, which will be explored in the upcoming sections. This will build upon the reporting database work and expand the data architecture for more advanced analytics.

# **XI) Data Lake Design - Medallion Architecture**

# **A) Data Lake Design Overview**

We took a significant amount of time to build our reporting layer as part of the data analytics project.

We began the project by ingesting product pricing data from a web service. As part of developing the ingestion pipeline, we learned how to design metadata-driven ingestion pipelines and how to use Azure Data Factory automated trigger mechanisms to schedule these pipelines. We also implemented incremental data loading, where changes in the source data were automatically captured and loaded into the data analytics platform.

After ingestion, we designed the reporting layer using dimensional data modeling techniques. As part of this approach, we created a dedicated reporting database. The dimensional data modeling output consisted of dimension tables and fact tables. To support this, we created an Azure SQL Server database and implemented the required dimension and fact tables.

We then developed Azure Data Factory pipelines to load the dimension tables, handling both scenarios—with history (slowly changing dimensions) and without history. In addition, we developed ADF data flows to load the fact tables into the reporting database. Once again, we applied change data capture (CDC) mechanisms so that only changed records from the source were processed and loaded.

To ensure automation, we implemented scheduling mechanisms in Azure Data Factory, allowing the pipelines to run automatically. As a result of this entire process, we successfully loaded almost 350 days’ worth of data from the source system into the reporting database.

We also briefly touched upon performance tuning in Azure Data Factory, specifically focusing on tuning the ADF data flow clusters. However, there is still more to learn regarding performance optimization in the SQL Server database, which we plan to explore next.

With the reporting layer in place, we can now move on to building the next layer of the architecture: the Data Lake. This layer is intended to support the AI and machine learning components of the data analytics project.

When we talk about a Data Lake, we are clearly stepping into the modern data engineering era. While traditional reporting databases follow strict rules and conservative design principles—such as dimensional modeling techniques that have existed for decades—the Data Lake represents a more flexible and modern approach to data storage and processing.

So far, we have built a reporting database that follows strict modeling rules. Dimensional modeling has been around for more than 20 years and is still widely used today, especially for reporting and analytics. While it is essential to understand this approach, the Data Lake introduces a completely different mindset.

The Data Lake does not impose strict restrictions on the type of data that can be ingested. You can bring any type of data into the Data Lake without worrying about rigid schemas upfront. To manage and organize this data, the Data Lake is typically divided into three logical layers: Bronze, Silver, and Gold.

The Bronze layer stores source data in its raw format. This is the landing zone where data is ingested exactly as it is received from the source systems.

The Silver layer is where the data from the Bronze layer is transformed into a cleaner, more structured format. For example, if the source data is stored as JSON files with nested arrays in the Bronze layer, those nested structures can be flattened in the Silver layer to make the data more accessible and usable for downstream processing.

The Gold layer represents the final, refined data that is ready for consumption. Unlike traditional dimensional modeling, the Data Lake layers do not enforce strict rules such as eliminating duplicate records or adhering to predefined table structures. This flexibility allows the Data Lake to deliver powerful outputs to end users.

Although the Data Lake is commonly used for AI and machine learning workloads, it can also support reporting layers built on top of it. Since the Data Lake can store nearly all data related to the project, it becomes a comprehensive and versatile data source.

Another key advantage of the Data Lake is that there are no practical restrictions on data size or schema definitions. You are not forced to carefully define column lengths or optimize storage space upfront. Cloud infrastructure makes this possible by providing virtually unlimited resources.

This shift in mindset is significant. Earlier in my career, designing database tables required careful consideration of data types and column lengths. Even today, when designing reporting databases, we still analyze source column lengths to determine optimal data types. However, when it comes to the Data Lake, this traditional way of thinking is largely unnecessary due to the flexibility and scalability of cloud storage.

That said, it is important to be mindful of these habits, as they are deeply ingrained from years of working with traditional databases.

Now, we are ready to start building our Data Lake architecture. We will use a combination of Azure Data Lake Storage and Azure SQL Database. Primarily, the Bronze and Silver layers will reside in the Azure Data Lake Storage account. For the Gold layer, we may create a new schema in the Azure SQL Server database and load the processed data into SQL tables.

To build these layers, we will also introduce additional data sources, such as third-party APIs. These sources will provide data entirely in JSON format, allowing us to work with a new type of source system.

Before ingesting this new data, we will first set up the Bronze, Silver, and Gold layers within the Data Lake Storage account. We will use a single storage account and create a root container for the Data Lake. Inside this container, we will create three subfolders: bronze, silver, and gold.

The ingestion process will start by loading source data into the Bronze layer. From there, we will build transformations to populate the Silver layer, followed by processing that produces the Gold layer, which will be ready for predictive modeling.

Our primary focus at this stage will be predictive modeling, and this Data Lake design will serve as the foundation for that work.

With this plan in place, the next step is to create a new container in the Azure Data Lake Storage account and set up the Bronze, Silver, and Gold folders, before proceeding further with the Data Lake design and implementation.

# **B) Data Lake Design - Setup Container and Folder Structure**

We are going to store the Data Lake data in the same Azure Data Lake Storage account that we have already used for our reporting purposes.

Within this storage account, we will create a brand-new container dedicated specifically to Data Lake–related data. We will name this container Pricing Data Lake.

Inside the Pricing Data Lake container, we will create three folders to represent the three logical layers of data in the Data Lake architecture.

The first layer is the Bronze layer. This layer is used to store all raw data exactly as it is received from the original source systems, without applying any transformations.

The second layer is the Silver layer. In this layer, we will transform and refine the data that was ingested into the Bronze layer, converting it into a more structured and usable format.

The final layer is the Gold layer, which represents the curated and business-ready data. This data can be directly consumed by end users and is specifically designed to support AI and machine learning services.

Now that we have created the Data Lake structure along with these three layers, we can take a quick look at the setup.

In the next lesson, we will explore the different types of additional data that we plan to bring into the Data Lake, which will help make this architecture fully ready for AI and machine learning workloads.

# **C) Data Lake Design - Additional Source Data Requirements**

We have already ingested product pricing information from a web service into our landing layer. Based on this data, we designed the reporting database and successfully populated it with the pricing information of the products.

Now, we are moving to the next phase of our data analytics project: building the Data Lake. This Data Lake will support pricing prediction algorithms for these products. At this stage, our focus is on preparing and enriching the data so that it can be effectively used by AI and machine learning models.

To support these prediction algorithms, we need additional data that directly influences product prices on a global scale. Therefore, we must identify and ingest external data sources that have a clear impact on pricing.

From a common-sense perspective, if there is high demand for a product, its price is likely to increase. Based on this understanding, the first additional dataset we are going to ingest is demographic data. This data will come from a demographic API and will include population data along with market location information.

By market location, we mean geographical details such as longitude and latitude provided by the API. This is the first external dataset we are bringing in, as we plan to merge this information with existing pricing data and make it available for prediction algorithms. While AI and machine learning developers will determine how much weight to assign to this factor, our responsibility is to identify and prepare the relevant data that affects product prices.

Among all demographic attributes, population size in a market is one of the most significant factors influencing product demand and pricing. Therefore, this will be the first dataset we ingest from the demographic data API.

The next dataset we plan to ingest is weather data, as weather conditions also play a critical role in influencing product prices. Weather not only impacts pricing but also affects production levels, supply chains, and availability of products. For this reason, we will bring in weather data from an open-source system that allows non-commercial usage.

With the free API account, we can retrieve weather data for approximately 100–200 markets, which is sufficient for our use case. Since most of our pricing data relates to the past year, we also require historical weather data, and fortunately, the selected API supports historical data retrieval.

The third dataset we will ingest is country policy data. Government policies can have a significant impact on global product prices. For example, when India imposed a ban on rice exports at certain times, rice prices changed globally. Such policy-related information is available as open-source data.

We will ingest this country policy data into the Data Lake, transform it, and integrate it with our pricing data. The final, enriched dataset will be stored in the Gold layer, making it available for AI and machine learning developers.

It is important to clarify that building AI and machine learning models is not within the scope of this project. Our objective is to prepare and deliver high-quality, enriched data that can support AI and machine learning services.

In addition to these datasets, we will also ingest global pricing data from the same HTTP web services. The pricing data currently loaded into the reporting database contains only India-specific pricing information. To support global price prediction, we need pricing data from other regions as well.

To achieve this, we will develop a proper ingestion pipeline to load global pricing data into the Data Lake. While doing so, we will begin exploring the Parquet file format, which is widely used in modern data platforms. Until now, we have preserved source data formats—for example, delimited text files remained delimited text files in the landing layer.

However, for global pricing data, we will convert the delimited text format into Parquet format, particularly in the Silver layer. Learning how to read and write Parquet files using Azure Data Factory is a valuable and important skill. Along with this, we will also work with JSON data, which introduces more complex structures.

From our databases, we have already ingested some reference data such as country codes, country names, market names, exchange rates, and commodity codes. This reference data will be very useful when building the Silver and Gold layers.

In the Bronze layer, we will store all incoming data in its raw format. The only exception is the global pricing data, which will be converted into Parquet format in the Silver layer. At this stage, we will apply transformations to handle complex data structures.

Unlike pricing data, some of the incoming JSON data contains nested arrays and dictionaries, making the structure more complex. We need to flatten this raw data before we can merge it with other datasets. Once flattened and standardized, the data can be integrated to create the final Gold layer, which will be ready for AI and machine learning services.

In the next lesson, we will take a quick look at the structure of the additional datasets we plan to ingest. After that, we will begin the ingestion process with demographic data.

Although global pricing data is also required, we have already explored how to ingest data from HTTP web services. Therefore, we can reuse the same pipelines and scheduling mechanisms for global pricing data ingestion.

What we will focus on next is something new—ingesting data from external APIs, which is a very common approach in modern data analytics platforms. Today, APIs are frequently used to bring external data into analytical systems.

I’ll see you in the next lesson, where we will review the structure of the additional data sources and start ingesting the demographic data.

# **D) Data Lake Design - Additional Source Data Format Overview**

Let’s start by going through each of the additional source datasets that we are planning to bring into the data analytics platform and load into the Data Lake. This will give us a clear understanding of the types of data we will be working with and how they contribute to the overall solution.

The first additional dataset is demographic data. This data captures population information for each market that we already track in our daily pricing data. Since pricing is analyzed at the market level, population data helps us understand how price changes correlate with demand in those markets.

Along with population data, this dataset also provides geographical information, such as latitude and longitude. These geographic coordinates will later be used to fetch weather data for each market. In addition, the demographic data includes attributes such as country ID and local administrative divisions for each market. This is important because the same market name can exist across multiple states or cities. To handle this, we retrieve at least five possible matches per market, allowing us to accurately map demographic data to the correct market captured in the daily pricing data. This makes demographic data the first dataset we will ingest.

The second dataset is weather data, which captures weather conditions for each market within a coverage radius of approximately 25 miles. This dataset is more complex in structure, as it contains nested dictionaries and arrays within the JSON response. We will explore how to handle this complexity using Azure Data Factory.

Each JSON response contains one month’s worth of weather data, whereas our product pricing data is captured at a daily level. Therefore, we need to split the monthly weather data into individual daily records so that it can be aligned with daily pricing data.

The third additional dataset we plan to ingest has an even more complex structure, containing multiple nested arrays. However, since Azure Data Factory provides robust transformation capabilities for handling complex JSON data, we will tackle this dataset last. The idea is to start with simpler JSON ingestion, gradually move to more complex structures, and finally handle the most complex dataset once we are comfortable with the transformations.

In addition to these datasets, we also need to ingest global pricing data. This data is slightly different from the pricing data we have already captured. While it contains similar pricing information, it is collected across multiple countries. It includes country names and country-specific product codes, which are universally recognized. These codes allow us to map product names across different countries, enabling global price comparison.

One important difference is that global pricing data is captured at a monthly level, whereas our existing pricing data is captured daily. Before merging these datasets, we need to aggregate daily pricing data into monthly-level data. This aggregation will be performed using Azure Data Factory transformations.

At this point, we still have a lot of work to do, but we already have a strong foundation. Most of the logic and components used while building the reporting database will be reused here. In fact, around 70% of the components and logic will remain the same, making this phase a valuable revision of previously learned concepts.

For example, we previously used the Aggregator transformation to identify unique records while loading dimension tables. In the Data Lake context, the same aggregator can be reused to aggregate daily pricing data into monthly-level data. Without this aggregation, we would not be able to compare local pricing data with global pricing data.

Once this comparison is possible, we can derive additional insights and recommendations. For instance, by analyzing which products are cultivated or produced in a specific country, we can compare that list with the products available in our dataset. If certain products are not produced locally, it indicates potential import dependency, allowing us to identify export opportunities for other countries.

As mentioned earlier, the Data Lake is highly flexible and does not impose strict requirements. It can be used to support reporting, recommendation systems, and advanced analytics. We can build reporting databases on top of the Data Lake, identify potential business opportunities, and also predict future product prices.

Our objective is to design the Data Lake in a way that it remains open, flexible, and extensible, supporting multiple use cases related to product pricing analytics, both now and in the future.

# **XII) Data Lake Bronze Layer Data Ingestion - Demographics Data REST API**

# **A) Demographics Data Ingestion Overview**

We are currently working on building our data lake architecture. As part of this design, we need to create three layers in the data lake: Bronze, Silver, and Gold.

At this stage, our focus is on building the Bronze layer. The Bronze layer is responsible for ingesting raw source data exactly as it is received, without any transformations. It serves as the first landing zone in the data lake.

For this implementation, we will ingest data from a demographic API. The data retrieved from this API will be stored directly in the Bronze layer of our data lake storage account.

The process begins by reading data from the API and ingesting it into the Bronze layer, establishing the foundation for downstream processing in the Silver and Gold layers.

# **B) HTTP Request Vs REST API REQUEST RESPONSE Overview**

We have already completed HTTP data ingestion. During that process, we provided two key values in the dataset to read the actual source data.

The first value is the source base URL, which we configured in the linked service. The second value is the source relative URL, which points to a specific resource under that base URL. This relative URL was parameterized in the dataset.

At runtime, Azure Data Factory concatenates the base URL with the relative URL, sends a request to the HTTP web server, reads the data from the source, and ingests it into the data lake storage account.

In this scenario, we are going to ingest data from a REST API. Even though this is a REST API request, we will still use the same HTTP connectivity for this ingestion. Azure Data Factory also provides a dedicated REST API linked service, which we will use for subsequent API ingestions. For this use case, however, we will continue with the existing HTTP linked service approach.

We will now configure a new HTTP linked service that points to a different URL, but follows the same overall mechanism as the earlier HTTP ingestion.

The key difference between HTTP file ingestion and REST API ingestion is that, in HTTP ingestion, a physical file exists on the HTTP web server, and Data Factory simply reads that file. In the REST API case, there is no physical file present.

Instead, we are making a request to a REST API endpoint via a URL. If you look at the portion of the URL after the question mark (?), you will notice that we are passing a set of parameters. These parameters are commonly referred to as the search string or query string in REST APIs.

The source API application receives our request along with the search string parameters, uses those values to search its own internal data store, and then fetches the matching results. It returns the data dynamically in the response format we requested, which in this case is JSON.

This is the main distinction: there is no static file involved in REST API ingestion. Instead, a software application accepts the request from Azure Data Factory, queries its own data store based on the provided parameters, and returns the results dynamically at runtime.

Our goal is to ingest this dynamically returned data into the Bronze layer of our data lake storage account.

To achieve this, we will now create a new linked service in Azure Data Factory to connect to the REST API URL and configure the ingestion accordingly.

# **C) Demographics Data Ingestion - Configure Linked Service**

By now, I expect you to be very familiar with opening Azure Data Factory and Data Factory Studio. If I ask you to create a dataset, you should not need any additional help or reference material to locate where dataset creation happens, because we have already done this multiple times.

You can navigate to the Author tab, go to Datasets, right-click, and create or open a dataset. Earlier, we created linked services directly while creating datasets. However, as a standard best practice, linked services should ideally be created under the Manage tab after understanding the different components, rather than creating them implicitly at the beginning.

So, our first step here is to create a new linked service.

For this ingestion, we are going to use HTTP, similar to how we handled HTTP data ingestion earlier. Although this is a REST API, this specific API does not support the REST connector, so we are using the HTTP linked service as a workaround. The remaining two REST APIs in this project will use the native REST data store. Even though we are using HTTP here, the final outcome will be the same.

Since we already know how to create an HTTP linked service, we’ll follow the same steps. To differentiate this linked service from the previous HTTP one, we will name it HTTP Geolocation Service.

You are already familiar with the Integration Runtime. At runtime, the integration runtime is responsible for connecting to this HTTP web service and reading the data.

For the Base URL, we will provide the value up to a certain point in the endpoint so that Data Factory can connect to the service. The remaining part of the URL—specifically the search string parameters—will be passed dynamically as the relative URL property in the dataset. This is similar to how we handled HTTP file ingestion, but in this case, we will dynamically construct the search string. We’ll explore that in more detail in subsequent lessons.

For authentication, we will use Anonymous, because all the URLs selected for this course are open-source. In real-time projects, you will most likely need some form of authentication, such as basic authentication using a username and password, client certificates, or other security mechanisms depending on how the API is protected. For now, anonymous authentication is sufficient.

After configuring the linked service, we test the connection. Once the test succeeds, the linked service is created and we can publish it.

Our next task is to create the dataset to read the data dynamically. In this case, we are not reading a physical file. Instead, we are creating a dataset that can pass a search string to the API, receive the response in JSON format, and store that data in the Bronze layer of our data lake storage account.

To achieve this, we need to create a parameterized source dataset. The dataset will accept multiple parameters, and we will pass values for these parameters from the pipeline.

We already know several ways to pass parameter values in Azure Data Factory. These values can come from metadata files, be derived dynamically using expressions, or be passed directly within the pipeline. We have explored multiple approaches earlier, but this scenario requires a slightly deeper understanding, which we will cover while building the pipeline.

The next step, therefore, is to create the source dataset, parameterize it to connect to this API, and enable it to accept dynamic values for the search parameters.

# **D) Demographics Data Ingestion - Configure Source and Sink Datasets**
Let us begin by creating the dataset required to connect to the geocoding REST API.

At this point, we are not going to perform any experimental labs, because we are already familiar with most of the components in Azure Data Factory. We will directly proceed with creating the required datasets.

We will create the source dataset under the Ingest folder. I select New Dataset, and since this is customer source data returned by the API, and the response format is JSON, I choose JSON as the dataset format.

I will name the dataset as mds_ctp_source_geocoding_data. Since this dataset represents geolocation information, I update the dataset name to align with the actual source we are reading from.

At this point, Data Factory asks for the relative URL. I am not going to hardcode the relative URL here because this API requires search string parameters, which we want to pass dynamically. Therefore, we will parameterize the relative URL as part of the dataset configuration.

Once that is done, I click OK, and the source dataset is created.

Next, I will create a dataset parameter for the relative URL. As we know, parameters can be defined at the dataset level and then mapped to connection properties. I map this parameter to the Relative URL field using dynamic content.

At this stage, we are not connecting to the actual REST API yet. We are simply creating the dataset structure. Later, when we build the pipeline, we will see how to dynamically pass values to this relative URL parameter.

Now, we need to create the sink dataset as well.

The sink will be Azure Data Lake Storage Gen2, and since the API response is in JSON format, the sink dataset format will also be JSON. This dataset represents the Bronze layer of our data lake.

I name the dataset in line with the source naming convention, using geolocation as part of the name.

For the linked service, instead of using an existing one, I create a new linked service specifically for the data lake. I name it ls_adls_datalake. Although it points to the same storage account, this naming convention makes it clear that this linked service is intended for data lake ingestion pipelines. This helps with clarity and reuse when building multiple pipelines.

I create the linked service on the fly, which is absolutely fine.

For the file path configuration, I do not provide any static values. Instead, I parameterize the path at the dataset level, as we usually do. This allows the pipeline to dynamically control where the data is written.

I then create three dataset parameters:

Data lake container name

Data lake folder name

Data lake file name

These parameters are mapped to the corresponding connection properties using dynamic content. We have done this many times before, so the process should be familiar. Later, the pipeline will supply values for these parameters.

At this point, both the source dataset and sink dataset have been created, along with all required parameters.

The final step here is to publish the changes.

In the next lesson, we will start building the pipeline to read data from the REST API and load it into the Bronze layer of the Data Lake.

# **E) Demographics Data Ingestion - Create Ingestion Pipeline**

We have now created all the datasets required to build our pipeline, so the next step is to create the pipeline.

While naming the pipeline, we follow a clear naming convention that reflects the layer being processed. Since we are loading data from the demographics data API into the Bronze layer of the data lake, the pipeline name includes bronze.

Earlier, we referred to this layer as the landing layer when designing reporting databases. However, in the context of a data lake architecture, this layer is referred to as the Bronze layer.

Next, we add a Copy Data activity to the pipeline. We do not need a data flow at this stage because we are simply reading data from the REST API and storing it in the same format. There are no transformations performed in the Bronze layer.

I give the Copy Data activity a meaningful name based on the action it performs—loading geolocation data.

Source Configuration

For the source, we select the geolocation source dataset that we created earlier. Since this is an HTTP-based API, the source type is HTTP.

Because we parameterized the relative URL at the dataset level, the pipeline now asks for a value for that parameter. Ultimately, this value should be passed dynamically. However, since this is our first time testing the API integration, we hardcode the search string for now to validate the setup.

We can quickly use Preview Data to confirm that the API call is working and that data is being returned correctly in JSON format. The preview works without any issues, confirming that the source configuration is correct.

Sink Configuration

Next, we configure the sink.

We select the Bronze geolocation sink dataset. This dataset also contains parameters, so we provide temporary hardcoded values to validate the pipeline execution.

Container name: pricing-datalake
This is the new container created specifically for our data lake. We are no longer using the landing container.

Folder name: bronze
This folder stores raw data ingested from source systems.

File name: For now, we use the same market name that we are querying, just to confirm that everything is working correctly.

Pipeline Execution

With both source and sink configured, we run the pipeline.

The pipeline executes successfully, which confirms that:

Data is being read from the REST API

The JSON response is being written to the Data Lake Bronze layer

To verify, we navigate to the Bronze layer in the Data Lake. Initially, the folder is empty. After refreshing, we can see the JSON file created for the selected market. Opening the file confirms that the data has been ingested correctly from the geolocation REST API.

This confirms that our end-to-end ingestion pipeline is working as expected.

Next Step

The final task is to remove all hardcoded values and make the pipeline fully dynamic.

We already know multiple approaches to achieve this:

Pipeline parameters

Metadata-driven pipelines

In the next lesson, we will explore the best approach for dynamically passing values to:

The REST API relative URL

Data Lake container name

Folder name

File name

# **F) Demographics Data Ingestion - Configure Pipeline Parameters**

Now, we need to find a way to parameterize the relative URL value used in the REST API call. To clearly understand what parts of the URL change and what parts remain constant, it is helpful to look at the full URL in a notepad first.

The first part of the URL is the base URL, which we have already defined. The second part, which starts with v1, is also tied to the base URL. This represents version 1 of the API, and the search endpoint is the default value. These components of the URL never change when making the REST API search call. Similarly, the question mark (?) is fixed and does not change.

The next part of the URL contains a parameter name, which is an actual value expected by the API. Here, we are passing the market name. This is the key part of the URL that changes dynamically, as it needs to be replaced with a different market name for each API request. The count parameter specifies how many results should be returned. Although the example shows 110, the maximum allowed value is 10, so we do not need to worry about this part for now. The remaining parameters—language set to English and format set to JSON—are constant and look fine.

From this analysis, we can clearly see that the only changing value in the source relative URL is the market name.

We already have a list of market names available from our dimension table. There is more than one market name in the source file—there are actually a large number of them. The query is running, and based on the data, there are approximately 1,664 distinct market names in total.

Because of this large number, we cannot create pipeline parameters for each market name. Creating over a thousand pipeline parameters is not practical or manageable. So the next logical option is to use a metadata file.

We are already familiar with metadata files from earlier work, where we used them to load data from HTTP web servers for reporting purposes. We have previously created two metadata files and understand their structure. This approach fits perfectly for this requirement.

The key decision rule here is simple:

If the value you are parameterizing has too many possible values, you should use a metadata-driven pipeline.

If the value has only one or very few possible values, then a pipeline parameter is sufficient.

In this case, the market name has thousands of values, so it should be handled through a metadata file. On the other hand, parameters like the result count (which will always be 10) are good candidates for pipeline parameters, since they are single, stable values. Even if they change slightly in the future, parameterizing them keeps the pipeline flexible and avoids hard-coding.

Similarly, the result format, which is currently always JSON, can also be parameterized as a pipeline parameter because it has only one possible value at the moment.

However, we cannot parameterize market names like “Kovilpatti” directly in the pipeline, because there are too many such values. Instead, we should store all market names in a metadata file, read that metadata during pipeline execution, and pass each market name dynamically to the Copy Data activity to make API requests.

In the same way, the sink details—such as the data lake container name, folder name, and file name—can also be stored in the metadata file. Since the file name changes for each market, handling this dynamically through metadata makes the pipeline fully automated and eliminates manual intervention.

By reading the metadata file and passing its values into the Copy Data activity, the pipeline can dynamically process each market without hard-coding anything. This makes the solution scalable, maintainable, and flexible.

We will proceed with creating the metadata file in the next lesson.

# **G) Demographics Data Ingestion - Create and Upload Metadata File**

We have decided to create a metadata file to store the market name along with all three required parameters for the sink: the data lake container name, folder name, and file name. Since the data already exists in the SQL Server database, creating this parameter file is a very straightforward task.

We already know the required values: the market name, the data lake container name, and the data lake folder name. For the file name, we can simply use the market name itself, because that aligns with how we plan to create the folder structure in the bronze layer. That is exactly what we have implemented.

If you look at the sink mapping, you will notice that the file name is set as market_name.json. We are storing data from multiple sources into the bronze layer, and this particular dataset is related specifically to geo-location data. Therefore, it makes sense to include geo-location information in the metadata file itself.

To make the structure clearer and more maintainable, we also include the bronze folder name in the metadata so that we can easily differentiate files related specifically to geo-location. To implement this, we quickly updated the metadata file by replacing all folder names from bronze to bronze/geolocation, ensuring that all geo-location-related data is stored under a dedicated folder in the Data Lake storage account.

Using a simple tool like Notepad, we were able to make these updates very quickly and efficiently. Once the changes were done, the metadata file was saved.

Next, we need to upload this metadata file into the same metadata folder in the Data Lake. Even though we are using the same Azure Data Factory, we have created two different containers in the Data Lake to differentiate between data ingested for reporting purposes and data ingested for the data lake. Despite this separation, it is best practice to keep all metadata files in a single metadata folder, so they can be reused easily by multiple developers in real-time projects.

If you are working on a single project, it is always recommended to keep the metadata in one consolidated location rather than creating multiple folders, which can unnecessarily complicate the design and cause confusion later.

The metadata file was first created on the local machine, and then uploaded to the Data Lake storage account. This is necessary because Azure Data Factory cannot read files directly from a local machine unless additional configuration is done, which is neither necessary nor relevant in this case.

To read this metadata file in ADF, we will use a Lookup activity. Whenever we need to read data from a file or dataset inside ADF, the Lookup transformation is the correct choice. In the next section, we will configure the Lookup activity to read the metadata file and pass the values dynamically to the source and sink parameters of the Copy Data activity.

Once this is configured, the pipeline should be able to load all geo-location data into the Data Lake storage very quickly.

It is important to note that this is a one-time or infrequent ingestion. Population and geo-location data—such as latitude and longitude—do not change very often. In most cases, population data is updated only once every ten years. Because of this, this particular pipeline does not need to be scheduled. It can be run on an ad-hoc basis whenever there are changes in the source data.

This pipeline serves as a simple and quick starting point for working with REST APIs. That is why we began with this example while building our data lake. As we move forward, we will ingest more relevant datasets that affect the business, such as pricing data and product data.

We will continue in the next lesson by creating and configuring the Lookup transformation.

# **H) Demographics Data Ingestion - Configure LOOKUP and FOREACH Activity**

Let us now start by including the Lookup activity in the pipeline. First, search for the Lookup activity in the activities pane, then drag and drop it onto the pipeline canvas. This Lookup activity will be used to read the market names metadata file.

Once the Lookup activity is added, go to its Settings tab. At this point, we do not yet have a dataset created for this metadata file, so we will quickly create one. Choose Azure Data Lake Storage Gen2 as the data store, since the metadata file already exists there and is stored in JSON format.

Next, provide a logical and meaningful name for the dataset. For example, you can name it something like
ds_adls_datalake_geolocation_marketnames_metadata.
Select the appropriate Linked Service, which will point to the Data Lake Storage account. Even though multiple datasets may point to the same storage account, that is perfectly fine.

For this dataset, we do not need to parameterize anything, because metadata files for this ingestion are not expected to change dynamically. So we can keep the dataset configuration static and proceed.

Now that the dataset is created, it is successfully linked to the Lookup activity in the pipeline. Before running it, recall one important setting: we must uncheck the “First row only” option. If this option remains checked, the Lookup activity will fetch only a single row from the metadata file, which is not what we want. We need all rows.

No other changes are required in the Lookup activity configuration. As we already know, the output of a Lookup activity always comes as an array.

At this point, we can run a debug execution to quickly verify the Lookup output. Since the pipeline parameters have default values, we can use them as-is. After running the debug, we can see that the output of the Lookup is indeed an array, where each element contains the market name, container name, folder name, and file name coming from the metadata file.

Since the output is an array, the next logical step is to process each element individually. To do this, we need to pass the Lookup output into a ForEach activity. So, add a ForEach activity to the pipeline and connect it to the output of the Lookup activity.

Give the ForEach activity a meaningful name, such as Iterate Market Names, so it is clear that this loop is iterating through each market name from the metadata file.

In the ForEach settings, we must connect the value array output of the Lookup activity to the Items field of the ForEach activity. Although the Lookup activity provides multiple outputs, we are only interested in the value array, because that is where the actual metadata records are stored.

You will also notice that the Disable option needs to be unchecked. For some reason, this sometimes needs to be done twice before it actually gets disabled—this is just something to note, even though the reason is unclear.

Now, inside the ForEach activity, we need to execute the Copy Data activity. To do this, we can either use the Edit activities option or drag the Copy Data activity into the ForEach container. In this case, we simply cut and paste the existing Copy Data activity into the ForEach loop.

Next, we need to configure the values that will be passed dynamically into the Copy Data activity from the ForEach iteration. To make this easier, we can copy the existing REST API URL into Notepad so that we can clearly identify which parts of the URL need to be replaced dynamically and which parts can be reused as-is.

Some parts of the URL will remain constant. Other parts must be replaced using:

Values coming from the ForEach output (read from the metadata file)

Values coming from pipeline parameters

This will be handled using the Pipeline Expression Builder, where we will build the full URL using a string concatenation expression. Up to a certain point, the URL remains the same. After that, the market name is replaced using the ForEach output, and the count and format values are replaced using pipeline parameters.

This process is fairly straightforward once we identify which values come from where. At this point, we have completed a good revision of how Lookup, ForEach, and Copy Data activities work together in a metadata-driven pipeline.

We will implement this expression building and parameter replacement in detail in the next lesson.

# **I) Demographics Data Ingestion - Pass Dataset Parameter Values From Metadata File**

Now we can start forming our relative URL using the Pipeline Expression Builder. The first part of the search string is a constant value—it will not change for any request. So, we click on the Relative URL field and open the Expression Builder. As discussed earlier, we will use the concat() function to construct the full relative URL dynamically.

The first search string remains the same for all requests, so we pass it directly as a constant value inside the concat() function. The second part of the URL, which is the market name, needs to come from the metadata file output. Since this value is being iterated inside the ForEach activity, we can access it using item() followed by the exact key name used in the metadata file.

To ensure accuracy, we open the geolocation market names metadata file and check the exact key name used for the market name. The value is stored under the key market_name. We do not replace the actual market name value itself; instead, we reference the key that holds this value. We copy this key carefully and use it in the Expression Builder as item().market_name.

Next, we return to the full URL structure in Notepad to identify the next section. After the market name, the next portion of the URL—up to count=—is again a constant string. This portion does not change across requests, so we add it directly to the concatenation expression as a fixed value.

The next value is the result count, which is set to 10. While we could hard-code this value, we want to keep the pipeline as clean and flexible as possible. Therefore, we use the pipeline parameter created earlier for the REST API result count and concatenate it instead of hard-coding the number.

Following this, the URL includes language=English. Since we do not expect the language to change, this part remains a constant. The final part of the relative URL is the format, which we have also parameterized as a pipeline parameter. By concatenating this value as well, the entire relative URL becomes fully dynamic, with no hard-coded values that may need changes later.

At this point, the relative URL configuration is complete and correct.

Next, we configure the sink dataset parameters. The container name comes directly from the metadata file, so we access it using item().data_lake_container_name. We intentionally use the term Data Lake here, because we are building the data lake layer, not the reporting layer of the analytical platform.

The folder name also comes from the metadata file and is accessed through the ForEach activity using the corresponding key. Since the ForEach is looping through the metadata file read by the Lookup activity, all metadata values are available through item().

The final sink parameter is the file name. We use the market name itself as the file name, which again comes from the metadata file. Since this value is already being used in both the source and sink configurations, there is no need to create an additional parameter for it.

However, there is one important detail to address: the file name must end with .json. We cannot directly use the market name alone, so we use the concat() function again to append .json to the market name. The dot (.) is included explicitly in the expression, and the format value is taken from the pipeline parameter. Copying and reusing the concatenation logic helps avoid mistakes.

With this, the sink configuration is complete.

Now the pipeline is fully ready to load geolocation data for all markets into the bronze layer of the data lake. Before publishing, there is one final consideration. Since we have around 1,000+ market names, we do not want to process all of them in parallel. To control this, we set the batch count in the ForEach activity to 10, so that only ten markets are processed at a time before moving to the next batch.

At this stage, the pipeline is complete and ready. We are dynamically making REST API requests, retrieving JSON responses that are not stored anywhere in the source system, and loading them into the bronze layer of the data lake.

In the next lesson, we will debug the pipeline and verify that the data is being ingested correctly.

# **J) Demographics Data Ingestion - Identifying and Fixing The Errors**

Now we can debug the pipeline straight away. When the pipeline prompts for pipeline parameter values, we do not need to change anything, because all required parameters already have default values. So we simply proceed by using those defaults and run the pipeline.

Our expectation is that the pipeline will load all the data into the bronze layer, specifically under the geolocation folder. The folder structure will be created automatically. Under the pricing data lake’s bronze layer, a geolocation folder should be created, and within that folder, a JSON file for each market name should be populated.

Once the pipeline starts running, we wait for a moment. At this point, we need to cancel the wait option and observe the pipeline execution. The pipeline fails—but that is actually a good thing. Failures give us an opportunity to understand what went wrong and improve our implementation. In fact, this particular error turns out to be very interesting and even helps refresh some important concepts.

This is the first time encountering this specific error. It turns out that there was a small mistake in the metadata file. As a standard practice, we copy the error message into Notepad so that we can review it calmly and clearly without getting overwhelmed by the UI. Expanding and formatting the error text helps us read it more easily.

The error message clearly states that “pricing data lake contains invalid characters”, and it also highlights the exact invalid characters. Spending a little time carefully reading the error message gives us the clue we need. Although at first glance it may not seem obvious—because the pricing data lake definitely exists and was working earlier—the error becomes clearer once we inspect the value closely.

The issue is related to the metadata file that was created. While creating the pricing data lake metadata file, extra characters were mistakenly included—specifically single quotes. The same issue appears in the folder name as well. These invalid characters cause the pipeline to fail once parameterization is applied, even though it worked earlier when values were hard-coded.

To fix this, we directly update the metadata file. This is also a good opportunity to demonstrate how to use Find and Replace within the editor. Using Ctrl + F, we search for the single quotes and replace them with nothing. Clicking Replace All removes all the unwanted characters in one step.

It is important to note that double quotes must remain, because they are required for valid JSON formatting. After removing the single quotes, the metadata file looks correct.

With the issue fixed, we rerun the pipeline. At this stage, it is important to remember that simply reading the error message carefully—especially the part mentioning invalid characters—was enough to identify the root cause. The presence of extra single quotes around the pricing data lake value was the key clue.

Now, after rerunning the pipeline with the corrected metadata file, the Copy Data activity starts successfully. Since the pipeline needs to process around 1,200 market names, it will take some time to complete. We allow the pipeline to continue running for a few minutes.

Although this was expected to be the simplest ingestion, it still provided valuable learning. Errors are often the best teachers—without them, we would not gain these insights.

Once the pipeline completes execution, we will review the run details in the next lesson to confirm that all market geolocation JSON files have been loaded successfully into the bronze layer.

# **K) Demographics Data Ingestion - Identifying and Fixing User Errors**

Before the pipeline completed, I did a quick check to see how the data was being loaded. At that point, I noticed something unexpected. The pipeline was creating strange file names inside the geolocation folder. The first part of the file name—the market name—looked correct, but after that, it was getting extended with the pipeline parameter value for the API result format. This clearly indicated that something in the code was not behaving as expected.

Because of this, we needed to cancel the pipeline execution. Although this may feel like a setback, it is actually a very good thing. The more errors you see and debug during this course, the more confident and solid you will become with Azure Data Factory. I always try to share every error, whether it is something I already know or something I encounter for the first time. This particular issue was not something I expected, which made it even more interesting.

The problem occurred while passing the data lake file name parameter. We used a concatenation expression where the market name was concatenated with the pipeline parameter for API result format. However, instead of replacing the parameter with its value properly, it was being appended as a literal string, which caused incorrect file names to be generated.

If you look closely, you can identify the issue fairly quickly, although it is a bit complex at first glance. This is one of those errors that is absolutely worth spending time on, because it strengthens your understanding. Importantly, this is a user error, not a system issue.

To explain this clearly, we used the same API result format parameter in the source configuration as well. I copied the expression from the source so you could compare both places. In the source relative URL, the parameter was used correctly. However, in the sink configuration, the parameter was mistakenly hard-coded inside the expression instead of being referenced properly as a pipeline parameter.

In other words, the last parameter in both the source and sink expressions looked similar, but only the source was configured correctly. In the sink, because the pipeline parameter was not referenced properly, it was treated as a plain string, which is why the sink file name was getting created as
marketname.<pipeline_parameter_name> instead of marketname.json.

Since the files were created incorrectly, we deleted the specific folder that was generated during the failed run. This itself is a valuable learning experience—for you and for me as well.

To fix the issue, we updated the sink configuration and replaced the incorrect code with the actual pipeline parameter reference. Once this correction was made, the file naming logic became correct.

At this point, we also revisited the parallelism settings in the ForEach activity. Earlier, we had set the batch count to 10, which meant only ten market names were processed in parallel. Since the data volume for each market is very small—sometimes just a single line of JSON—we can safely increase the parallelism. I decided to increase the batch count to 50, which significantly reduces the overall runtime. Running 50 parallel Copy Data activities is completely fine for this small dataset.

After making these changes, we debugged the pipeline again. There was no need to pass any parameter values, as defaults were sufficient. This time, after the first successful Copy Data execution, we quickly verified the output to ensure everything looked correct.

Now, the files were being created properly with the correct naming convention:
marketname.json. Everything looked good.

We let the pipeline continue running until completion. At this stage, we have successfully loaded all market-wise geolocation JSON data into the bronze layer of the data lake, under the geolocation folder.

This marks the successful completion of our first REST API ingestion using JSON. We have dynamically fetched data from an API, handled metadata-driven processing, debugged real-world errors, and loaded the data into the data lake correctly.

Next, we will move on to another REST API in JSON format and continue building on this foundation.

# **XIII) Data Lake Bronze Layer Data Ingestion - Weather Data REST API**

# **A) Weather Data Ingestion Overview**

We have completed one REST API data ingestion earlier. Even though it was a REST API, we used the HTTP Linked Service to connect to the URL. We parameterized the market name and dynamically looped through each market, loading the data into the Bronze layer of the Data Lake.

Now, we are going to work on another REST API to fetch weather data. This is again an open-source API, and we will be using it in our pipeline. First, we will quickly review the API URL to understand which values need to be passed dynamically. Based on that, we will create a pipeline to load weather data for all market names.

Starting with the first part of the Weather API, there is not much difference in structure. This API uses a specific version, and instead of using a search endpoint, it uses an archive endpoint because we are trying to retrieve historical weather data. As discussed earlier, after the question mark (?) in the URL, we need to identify the list of query parameters that must be passed and understand how to dynamically construct them within the pipeline.

The first required parameter is latitude. This API requires geographical coordinates rather than market names. It does not directly accept market names as input. However, in our project design, the output of the previous ingestion can be reused as input for the next request.

If you look at the output files generated during the geocoding ingestion, each file already contains the latitude and longitude information for its respective market name. When you open one of these files, you can clearly see the latitude and longitude values. However, this information currently exists across multiple JSON files.

Now, we need to consolidate these latitude and longitude values into a single place so that they can be reused for the weather data ingestion. This consolidation is completely feasible and does not pose any major challenges.

The new weather API requires latitude and longitude as mandatory input parameters. In addition to that, it also asks for a start date and an end date, specifying the period for which historical weather data is required. Since the data volume can be quite large, the plan is to retrieve data month by month. This approach will improve performance and speed.

By fetching data monthly, we can retrieve an entire year’s data using 12 files, instead of creating too many small daily files. Creating data on a daily basis would result in a large number of small files, which is not ideal. Therefore, a monthly approach is preferred as it is faster and more efficient.

Another important parameter is the list of weather variables (columns) that we want to include in the response. In our case, we are interested in:

Maximum temperature at 2 meters

Minimum temperature at 2 meters

Rainfall recorded for that specific market on a given day

The final parameter is time zone. Since this API supports global weather data, we need to ensure it works correctly for markets in India. Setting the time zone to auto ensures that the API automatically adjusts based on the location.

So overall, we need to dynamically construct the weather API URL within our data ingestion pipeline. This URL must be built for each market, using latitude, longitude, date range, required weather parameters, and time zone.

Before developing the final pipeline, we need to perform some preparatory tasks. Specifically, we need latitude and longitude values for all market names we are interested in. These values already exist as output from our previous geocoding ingestion, stored in the Bronze layer of the Data Lake.

To achieve this, we will quickly develop a pipeline in Work Lab that reads all the geocoding output files from the Bronze layer. From each file, we will extract the latitude and longitude values associated with each market name.

Once extracted, we will consolidate this information into a single dataset. This consolidated dataset will then act as metadata for driving the weather data ingestion process.

In summary, this process will be completed in two steps:

Read and consolidate latitude and longitude information for all market names from the geocoding ingestion output.

Use this consolidated metadata to dynamically call the weather API and ingest the weather data into the Bronze layer of the Data Lake.

# **B) Weather Data Ingestion - Dynamic Metadata File Creation Configure Source**

So, first, we need to retrieve the latitude and longitude information that we previously loaded as part of the geolocation data ingestion. This information will be used to load weather data from the new weather API that we have identified.

To achieve this, we are going to quickly develop Lab 5 Data Flow under the Working Labs section. The purpose of this data flow is to extract only the latitude and longitude information from the geolocation data. We will be transforming this data into a flattened format.

Although the geolocation data will eventually be loaded into the Silver layer of the Data Lake, this step is mainly for practice and preparation. It demonstrates the best practice for reading complex JSON data and flattening it before moving into the Silver layer. Since we only need this data for metadata purposes, we are doing this work inside the Working Labs.

The latitude and longitude information is not part of our final output. It is only required to drive the weather API ingestion. Therefore, we are creating a quick data flow just to understand how to read a JSON file and flatten the structure.

Previously, we did not properly organize the Working Labs folder under Data Flows. We had created a sample data flow while loading a dimension table, but it was not well structured. Now, we are placing everything under Working Labs, and later it can be moved or cleaned up as needed.

Next, we create a new data flow specifically to transform the geolocation data. The goal of this data flow is very clear: extract only latitude and longitude from the geolocation JSON file. This information is required by the new weather API that we will use to load weather data.

For this data flow, we need two datasets:

One dataset for reading the geolocation data

Another dataset for writing the transformed latitude and longitude output

So, again, under the Working Labs area, we quickly create two new datasets. For reading the geolocation data, the dataset can point to any one of the source JSON files, which is fine for now. At this stage, our requirement is to read all JSON files and identify the latitude and longitude information.

To save time, we will clone an existing dataset instead of creating a new one from scratch. Previously, we used this dataset to load similar data, so cloning makes the process quicker. We also move this dataset into the Working Labs folder to avoid any confusion or dependency issues.

At the same time, we make sure that Lab 5 is opened and active. Working with too many datasets at once can be confusing, so keeping everything focused within a single lab helps. We also retain the same parameters so that values can be passed dynamically, allowing us to read all files from the source folder.

Once the source dataset is ready, we then create an output dataset to store the transformed latitude and longitude values produced by the data flow. This will be done later during the transformation stage. We strictly follow the naming conventions used across the project.

We intentionally avoid using existing or inconsistent names. Since this code will eventually be deployed to higher environments using a CI/CD pipeline, naming conventions are extremely important. If naming standards are not followed, the CI/CD pipeline may fail. That is why everything is kept very clean and structured.

At this point, our source dataset for reading geolocation JSON files is ready. This is the first major task completed.

Next, we enable Data Flow Debug so that we can see the data coming from the JSON files. We go to the Source Settings, and for now, there is nothing additional that needs to be configured.

However, in the Projection tab, we notice that no column names are visible. This is because the schema has not yet been imported from the source file. To resolve this, we need to import the schema so that the projection columns appear in the data flow.

Once the schema is imported, we will be able to explore the data and see exactly what information is coming through from the geolocation JSON files. We will continue analyzing and transforming this data in the next lesson.

# **C) Weather Data Ingestion - Dynamic Metadata File Creation Configure Source Schema**

We start by importing the schema for the geolocation files that we have already loaded. We select one file that has the correct path and valid data. Since everything is parameterized, importing the schema from a single file is sufficient.

When we import the schema from the connection store, it asks for all the required values. The container name is Pricing Data Lake, and the folder path is branch/geolocation. The final input required is the file name. Since the structure is identical across all files, importing the schema from one file will apply to all geolocation files.

Once the schema is imported, all the data inside the JSON file becomes available in the data flow. This is the first time we are encountering an object data type, because the JSON structure is slightly complex. It is not highly complex, but it is more structured than a simple flat JSON. Compared to other JSON files that we will work with later, this one is relatively simple.

If we take a closer look at the structure, the actual values are stored inside an array called results. Within this array, the data is stored as a map element. To reference specific fields such as latitude and longitude, we need to use:

results.latitude

results.longitude

This is how we access those values in the data flow.

Once the schema is imported, we can check the Projection tab and see that all column names are now visible. All the fields exist under the results array. When we move to the Data Preview, the data should be displayed accordingly.

At this point, an error occurs stating that no value was provided for the parameter dst_prm_data_lake_container_name. This happens because we are using parameters in the dataset but have not yet passed values to those parameters. Since the parameters are not populated, the data flow is unable to connect to the source and retrieve the data.

We have already learned how to handle this. To pass parameter values, we go to the Debug Settings after enabling Data Flow Debug. Here, all parameters used in the dataset and the data flow are displayed.

In this case, we are not using data flow–level parameters. We manually provide the values:

Container name: Pricing Data Lake

Folder path: branch/geolocation

File name: we can reuse the existing file name that was previously copied

After verifying the folder structure and confirming that the path is correct, we apply the values. This allows the data preview to load successfully.

At this stage, it is very important to continuously use the Data Preview option. Since we are working with new transformations and a new data structure, the preview helps us understand how the data is flowing and how it can be converted.

This may be the first time we are seeing data displayed in an array format. The results field is an array that holds the complete data. To view the actual records, we need to expand the array in the data preview.

Once expanded, we can see fields such as:

results.id

results.name

results.latitude

results.longitude

and other geolocation attributes captured earlier

Our primary goal is to extract latitude and longitude. However, we also need to include administrative information such as admin1 and admin2. If we only store latitude and longitude, it will be difficult to identify which market the data belongs to when extracting weather information later.

Therefore, along with latitude and longitude, we will include some textual attributes in the sink. This additional context will help us reuse the data while passing inputs to the weather API.

In the next lesson, we will explore how to extract and flatten this information from the complex data structure and transform it into a usable format for the weather data ingestion.

# **D) Weather Data Ingestion - Dynamic Metadata File Creation FLATTEN Complex JSON**

Now we are going to extract information from the complex data type present in the geolocation JSON file. To do this, we need to use a new transformation that we have not used before. This transformation is called Flatten, and it is specifically designed to flatten complex JSON structures.

The Flatten transformation is available with the same name, and we will use it to flatten the complex data type in our JSON file. The two configuration options that we are particularly interested in here are Unroll By and Unroll Root.

As soon as we select the Flatten transformation, it displays the available complex data types present in the incoming data. In our case, the complex data type is results, which is an array.

We set Unroll By to results, and the Unroll Root is also set to results. At this point, the data preview may show only two records: one coming from the results array and another from the generation timestamp, which is a normal data type.

Once these settings are applied, the Flatten transformation splits all the fields inside the results array into individual columns. To make this effective, we reset the input columns. As soon as we do that, we can see that the complex array structure has been converted into simple, individual column values.

This approach works perfectly for a single-level array. If the JSON structure contains multiple nested arrays, we would need to use multiple Flatten transformations to fully flatten the data.

When we check the Data Preview at this stage, the data is displayed in a completely flattened format. The complex results array no longer exists; instead, all values appear as plain columns.

At the moment, only one market name is displayed because we have mapped only one source file. We will update this configuration later to include all geolocation files.

The next step is to map the required fields from this flattened data into the sink file. Essentially, we are dynamically generating a metadata file. Since the data volume is large and manual creation is not feasible, we are using Azure Data Factory to automate the entire process.

Now, let us review the columns:

The name field represents the market name

The ID field comes from the geolocation API, but we do not need it, so we remove it

The name column is retained and renamed to market_name

Latitude and Longitude are the most critical fields, so we definitely keep them

We do not need fields such as elevation and feature code, so those are removed. We decide to keep the country code after latitude and longitude.

This metadata file will be used later in the actual weather ingestion pipeline. The Weather API does not accept market names as input; instead, it requires latitude, longitude, and date range. That is why this metadata file is essential.

Next, we evaluate the remaining fields:

Admin codes are internal to the geolocation API and are not required

Country name is useful, so we keep it

Admin1 represents the state name

Admin2 represents the district name

We keep country name, state name, and district name, as these fields help resolve ambiguity if the same market name exists in multiple states or districts.

Fields such as timezone, population, country ID, and admin ID values are not required, so they are excluded.

After completing the Select (mapping) transformation, we check the data preview again. Now, only the columns required to build the metadata file are present, and the output looks clean and correct.

At this stage, we plan to store this output in a JSON file, but we temporarily hold off on writing it. This is because we still need to add three more parameters that are required to fully build our pipeline.

It is better to include these parameters now rather than adding them later. Ultimately, we are trying to create a metadata file similar to the market name metadata file that was previously created manually. That manual metadata file contained fields such as:

Market name

Latitude

Longitude

Data lake container name

Data lake folder name

If we include the data lake container name and data lake folder name here itself, it will make the pipeline implementation much easier later.

At this point, we are still not working on the actual weather data ingestion pipeline. Our focus is only on dynamically generating the metadata file that will drive the weather ingestion process.

Now we face a small challenge. So far, the source dataset is pointing to only one geolocation file. However, in reality, we need to process all geolocation files available under the geolocation folder.

To do this, we need to set the geolocation folder as the root path and use a wildcard file path so that all files inside this folder are read automatically. We will configure this wildcard logic in the next lesson.

# **E) Weather Data Ingestion - Dynamic Metadata File Config Additional Params and SINK**

Let’s first take a quick look at the source data that we are trying to read. This data is stored under the geolocation folder and exists as multiple JSON files. At the moment, our source dataset is parameterized, but it is still pointing to only one source file, based on the value we provided in the debug settings.

However, our requirement is to read all geolocation files, because we need to extract latitude and longitude information for every market. This is necessary since we will later retrieve weather information for all of these markets. Therefore, we need to configure the source to read all files instead of just one.

To achieve this, we use one of the very useful features available in Azure Data Factory Data Flow. In the Source Settings, we leave everything as it is and move to the Source Options section. Here, we can use the wildcard path option.

The wildcard path does not require the container name. It only needs the folder path and file pattern. In our case, the folder path is branch/geolocation. Under this folder, all files are JSON files, so we use a wildcard pattern of *.json.

By specifying branch/geolocation/*.json, the data flow will now attempt to read all JSON files present in that folder instead of a single file.

Once this configuration is done, we quickly validate it using the Data Preview option. We click the refresh button to ensure that the settings are working correctly. The preview confirms that data from all market files is being read and displayed under the complex data type.

This is expected behavior, because the data is still in its original structure. However, we have already applied the Flatten transformation, and we have identified the required columns that need to be included in our metadata file.

In addition to the existing columns, we now want to include three more fields that were present in the previous metadata file. These include:

Data Lake container name

Data Lake folder name

Including these fields here will allow us to generate a complete metadata file that can be directly used in the weather data ingestion pipeline.

The idea is to generate all required metadata in a single automated step, so that we can reuse this file when calling the weather REST API. This approach saves a lot of manual effort and ensures consistency.

At this stage, the data volume we are working with is quite large. Because of that, automation becomes critical. This pipeline is not intended to be deployed to production. Its purpose is to speed up development and help us generate metadata quickly and reliably.

Before writing the output, we add two more columns using a Derived Column transformation. These additional metadata parameters will be used later in the downstream pipeline.

The first derived column is data_lake_container_name, and its value is set to pricing_data_lake.

The second derived column is data_lake_folder_name. We verify the correct value, and in this case, it is set to branch/weather_data, because the purpose of this metadata file is to load weather data into the Data Lake.

Next, we configure the Sink. The sink points directly to the metadata folder, because this entire data flow has been created specifically to generate metadata.

In the Sink settings, we create a new dataset. This dataset uses Azure Data Lake Storage Gen2 as the storage type and stores the output in JSON format.

We ensure that the dataset name aligns with Lab 5 naming conventions, so that it remains easy to track and reference later. Consistent naming helps us understand which pipeline or lab the dataset belongs to.

For the file name, we follow the same pattern used earlier. Previously, we had a file named something like market_names.json. Since this metadata is now for weather data and contains geocoordinates, we rename the file accordingly.

The new file name reflects its purpose clearly. It contains market names, but more importantly, it includes geo-coordinates, which are the key inputs for the weather API.

At this point, when the data flow attempts to validate the sink schema, it throws an error indicating that the target file does not exist. This is expected behavior, because the file has not yet been created.

We acknowledge this error and proceed. The pipeline should still allow us to publish successfully. Any remaining errors or validation issues will be reviewed and addressed in the next lesson.

# **F) Weather Data Ingestion - Dynamic Metadata File Creation & DATAFLOW Partitioning**

The error we encountered is very straightforward. I initially assumed that string values could be passed without single quotes, but in Data Flow expressions, string literals must always be enclosed in single quotes. If we do not do this, the expression will fail.

This happens because Data Flow expressions use a different execution engine compared to pipeline expressions. Once the single quotes are added correctly, the validation succeeds and everything looks good.

With that fixed, we go ahead and publish the changes.

Now, we quickly develop a pipeline to run this data flow under the Working Labs. We create a new pipeline and name it based on the data flow. Since the data flow name starts with DF, we replace it with PL to follow naming conventions.
So the pipeline name becomes something like PL_Trans_Geolocation_JSON_Lab5.

At this point, many panels may be expanded, which can be confusing. To keep things clean, we close unnecessary tabs and then drag the DF_Trans_Geolocation data flow into the pipeline.

The pipeline will again ask for dataset parameter values. That is completely fine. We can hardcode them because this pipeline is not meant for final production delivery. This pipeline is only used to generate the metadata file required for ingesting weather data.

We provide the folder name as bronze/geolocation. For the file name, even though we have configured a wildcard path inside the data flow, the dataset still expects a value. So we provide any one valid file name. The actual reading of all files is handled by the wildcard configuration inside the data flow.

We perform a quick validation, confirm that everything looks good, and then publish and run the pipeline.

This time, we are dynamically generating the metadata file. Creating this kind of metadata manually is practically impossible. Situations like this will come up in real projects as well. Instead of trying to manually create metadata, it is always better to build a quick ADF pipeline to generate it automatically.

This pipeline does not need to be deployed to production, but the metadata file it produces must be deployed to production. That is the key objective of this exercise.

The pipeline runs successfully, so we go ahead and refresh the metadata folder to check the output.

We see some files that were already created earlier. Along with those, we now see new metadata files. Initially, this may look unexpected, but when we inspect any one of the JSON files, the content looks correct. It includes latitude, longitude, data lake container name, and all required fields.

However, we notice that the output is split into multiple files instead of a single file.

This behavior is expected. Data Flow runs on an Apache Spark cluster, which uses distributed processing. The compute cluster consists of multiple machines, and each machine processes a portion of the source data. Each machine then writes its output independently, resulting in multiple files.

This is controlled by the partitioning behavior of the Spark engine. By default, Data Flow uses current partitioning, which leads to multiple output files.

If we want to generate a single output file, we must change the Sink settings. There is an option called “Output to single file”. When we enable this option, Data Flow automatically changes the partitioning to single partition.

At this point, we can also specify the output file name. Even though we provided a file name in the sink dataset earlier, that name is ignored when the data flow runs in clustered mode. In cluster mode, file names are automatically generated by Spark unless we explicitly force single-file output.

Before re-running the pipeline, we delete the previously generated multiple files. While lookup activities can technically read files using wildcard paths, metadata files should ideally be maintained as a single file for better control and simplicity.

Now, with the sink configured for single-file output, we run the pipeline again.

This time, the pipeline completes successfully and generates only one metadata file in the metadata folder.

When we open and inspect this file, everything looks correct. The structure is clean, and all required metadata fields are present.

Now, we can confidently use this metadata file as the input to build the Weather Data REST API ingestion pipeline.

At this point, the complexity level has increased significantly, and that is actually a good thing. As long as you are able to follow everything happening here, it means your understanding is solid. If anything feels confusing, go back and revisit the components we have worked on so far. Once you connect all the pieces, everything will start to make sense.

With the metadata file ready, we are now set to begin building the weather data ingestion pipeline.

# **G) Weather Data Ingestion - Configure Source and Sink Datasets**

Now let’s start by creating the Linked Service in Azure Data Factory.

First, we need the base URL. I may have mentioned earlier that we would be using a REST API this time. However, please excuse the confusion here. Although we are making REST-style requests, the historical weather APIs are not working with the REST data store in Azure Data Factory.

Because of this limitation, we still need to use the HTTP data store to fetch the data. We are not downloading files directly; instead, we are making REST API requests using the HTTP connector to retrieve the data from the API.

So we create a new HTTP Linked Service and name it something like http_weather_source, and we provide the base URL.

Next, we select the Integration Runtime. This is the execution engine that runs all of our ADF pipelines, so it’s important to understand its role.

For authentication, we choose Anonymous, since this is an open-source API. We then click Test Connection, confirm that the connection is successful, and create the Linked Service. After that, we publish the changes.

The next step is to create the source dataset for the weather data. We go to the Author section and start creating a new dataset.

Again, this dataset will be based on the HTTP connector. Even though we are making REST API requests, ADF does not support this API directly using the REST data store, so we use HTTP instead.

We select the Linked Service we just created for weather data. We do not provide the relative URL at design time, because we want to parameterize it and pass the actual URL dynamically at runtime.

We quickly create the source dataset and add a parameter named something like dst_prm_relative_url. By now, some of these parameter names should feel familiar. Repeating these patterns is actually beneficial—when you become a data engineer, you will be doing these same steps repeatedly in real projects.

With the source dataset created, we move on to creating the sink dataset.

This new dataset will store the weather data in Azure Data Lake Storage Gen2, inside the Bronze layer. The file format will be JSON.

We follow the standard naming conventions for the dataset name, making it clear that it represents weather data stored in the Bronze layer.

Although both Linked Services might technically work, we explicitly choose the Data Lake Linked Service. This is important because, in production environments, the Data Lake storage account is usually different from other storage accounts, and this separation becomes critical during deployment.

For the file system, we do not hardcode any values. As usual, we parameterize everything. We create three dataset parameters:

Data lake container name

Data lake folder name

Data lake file name

Once the parameters are created, we map them to the appropriate connection properties in the dataset.

At this point, both the source dataset and the sink dataset are ready.

With these components in place, we are now ready to start developing the pipeline that will load weather data into the Bronze layer of the Data Lake. We will begin building that pipeline in the next lesson.

# **H) Weather Data Ingestion - Configure LOOKUP and FOREACH Activity**

We will create a new ingest pipeline under the ingest folder and follow proper naming conventions. Naming conventions are extremely important for keeping the project maintainable, especially when working with huge volumes of data. If naming and structure are not clean, at some point in the course you may get stuck and find it difficult to proceed further. That is why consistency and clarity in naming are very critical from the beginning.

In this pipeline, we are going to ingest weather data from the EPA into the Bronze layer of our data lake. As usual, we will use the Copy Data activity, because we are not transforming or changing the structure of the source file. The activity can be named something like Copy Data – Weather Details.

Next, go to the Source section of the Copy Data activity. Search for the dataset that contains the string weather, so you can select the HTTP source weather dataset. At this stage, it will ask for the Relative URL path for testing purposes. For now, copy the required part of the actual API URL—from the starting point up to the end—and paste it here. Later, we will parameterize this value using the metadata file that we already created.

Then move to the Sink section and search using the string weather to select your ADLS dataset. It will ask for the container name and sink path. This will point to the Pricing Data Lake, which is where we created our new data lake. For now, the folder name will be bronze. For testing purposes, we will manually pass an actual market name as the file name. In this example, the hometown name Kovilpatti.json is used.

Before parameterizing everything using the metadata file, we will do a quick debug run to make sure the pipeline works correctly. The pipeline should run very quickly. Once it succeeds, we will check the data lake to confirm that the new JSON file has been created. The file may appear directly inside the bronze folder rather than a subfolder. There may also be an older file present, such as one created earlier for geolocation data, which can be deleted to avoid confusion.

Open the newly created file and inspect its contents. You can see that the weather information is being fetched correctly. The data includes details such as temperature and rainfall for each market on a daily basis for a month. The API response is very fast, and the data is returned correctly, which confirms that the setup is working as expected.

Now that the basic pipeline is validated, we can start parameterizing the dataset values using the metadata file. To do this, we first need to read the metadata file. We will add a Lookup activity again. Since we are reusing the same activities repeatedly, this repetition helps strengthen your understanding and skills.

Create a new Lookup activity, for example Lookup – Read Weather Metadata Files. The source will be ADLS Gen2, and the file type will be JSON. At this point, the metadata dataset may not have been created earlier because the pipeline was first built to verify functionality. Now we will follow standard naming conventions for metadata datasets as well, such as RDS_ADLS_JSON_Weather_Metadata.

You can use either Landing or Data Lake linked services, as both will point to the ADF metadata container. Inside that container, select the metadata file that we created dynamically earlier. This metadata file is already structured properly, which is very useful.

In the Lookup activity settings, make sure to uncheck the “First row only” option, because we want to read all rows. No other special options are required. The output of this Lookup activity will be an array.

Since the Lookup output is an array, we need to pass it into a ForEach activity. This is exactly what we have learned before. We are replicating the same ingestion logic multiple times—once for each metadata entry. In the ForEach activity, set the Items value to the Lookup output array.

If the Lookup output is not visible initially, make sure the Lookup activity is properly connected to the ForEach activity. Once connected, you will see the value array, which will act as the input source for the ForEach loop.

Next, move the Copy Data activity inside the ForEach loop. Cut the Copy Data activity and paste it inside the ForEach. This allows the pipeline to execute the ingestion logic dynamically for each metadata record.

At this point, the pipeline structure is complete. The remaining task is to pass the source and sink dataset parameters dynamically from the metadata using expressions like @item(). This parameterization will be handled in the next lesson.

# **I) Weather_Data_Ingestion-Configure_Pipeline_Parameters_and_Variables**

Transcript Not Available

# **J) Weather Data Ingestion - Pass Dataset Parameter Values Using Pipeline Expression**

Transcript Not Available

# **K) Weather Data Ingestion - Configure Dynamic Subfolder Creation in Sink Storage**

We have provided the data lake container name as Pricing Data Lake and the folder name as bronze/weather_data. When the pipeline runs, it will create an additional folder called weather_data, and inside that folder it will store the weather files in the same structure that we used earlier for the geolocation data—one file per market name.

At the moment, this setup works only for one month of data. However, our requirement is to schedule the pipeline for an entire year. If we run the pipeline again for a different month, for example from 2023-02-01 to 2023-02-28, the pipeline will overwrite the existing files in the bronze layer. This happens because we are not changing the folder name dynamically for each month. To prevent overwriting previous data, we need to enhance the pipeline logic.

To solve this, we need to introduce an additional subfolder for each month. For example, we can create a folder like 202301 to represent January 2023. When loading data, the pipeline should create a monthly subfolder inside the weather_data folder, so that each month’s data is stored separately. This ensures that data from previous months is preserved and not overwritten.

To implement this, we go back to the pipeline level and create a new pipeline variable. This variable will hold the weather month value. We name the variable something like pipeline_variable_weather_month, and its type will be string. The value of this variable will be derived from the pipeline parameter start date.

We only need the year and month format for the folder name, so we use the formatDateTime function. We pass the pipeline start date and format it as yyyyMM. This variable will then be reused in the sink folder path so that a new folder is created for each month automatically.

Now, instead of hardcoding the sink folder name, we modify it using concatenation. Earlier, the folder name was coming directly from the metadata file, something like bronze/weather_data. We remove the static value and replace it with a concat expression.

The concatenation logic includes three parts:

The root folder name coming from the metadata file (for example, item().data_lake_folder_name)

A forward slash /

The weather month variable that we just created

While doing this, we realize that the metadata folder name did not originally include a trailing slash. So we add the forward slash explicitly in the concatenation to ensure the path is formed correctly. This guarantees that every month’s data lands in a separate folder under weather_data/yyyyMM.

With this approach, the structure becomes consistent. Inside weather_data, each month gets its own folder, and inside each monthly folder, there will be one JSON file per market. This prevents overwriting and keeps historical data intact.

Next, we also ensure that the output file format is parameterized. We create a pipeline parameter called something like pipeline_parameter_sink_output_format and set its value to json. This way, if the format ever changes in the future, we only need to update it in one place.

In the Copy Data activity sink file name, we again use concatenation. The file name is built using:

The market name coming from the metadata file

A dot .

The output format parameter (json)

This results in filenames like Kovilpatti.json. This time, we are careful not to repeat the earlier mistake of missing quotes around string values. Everything is properly formatted and validated.

Once all expressions look correct, we publish the changes. Before scheduling the pipeline for an entire year, we decide to run it for one month to validate the logic.

During validation, we notice that the weather month variable contains extra trailing spaces. We quickly inspect the Set Variable – Weather Month activity and open its settings. The formatDateTime expression looks correct, but there may have been an accidental space entered earlier. We correct the expression and make sure the format is exactly yyyyMM.

After fixing this, the variable value looks clean and correct. We publish the changes again. Now the pipeline is ready to run for a single month without overwriting data.

In the next lesson, we will run the pipeline for one month to confirm that everything works as expected before scheduling it to run automatically for an entire year.

# **L) Weather Data Ingestion - Pipeline Debugging and Known Error on Activity Name**

Let us start running the pipeline. While starting the run, we encounter a strange error. This is one of those horrible pipeline errors that can occur in any data factory pipeline. The tricky part is that although the root cause is very simple, it is not obvious from the error message itself, and you usually cannot identify the issue just by looking at the error details.

This is an important precaution to keep in mind. In this case, the fix is very simple. When setting the weather month variable, an extra space was accidentally included in the value. That small additional space is the actual root cause of the failure. Because of this, the pipeline is not even allowed to start execution.

So whenever you face this kind of error, always check your pipeline variables, parameter values, and naming conventions carefully. In most cases, the issue is not with your logic or code but with unexpected spaces or formatting issues in variable values. Since ADF performs validations before running the pipeline, it fails during validation itself and does not proceed further.

After fixing the extra space issue, we proceed to run the pipeline again. This time, we plan to run it for one month of data only, before executing it end-to-end for a longer duration. This is a good practice to validate the pipeline behavior incrementally.

We copy the required datetime values and pass them as parameters. The pipeline is configured to run from 2023-01-01 to 2023-01-31. This allows us to load one complete month of weather data and confirm that everything works as expected before scaling it further.

Once the pipeline starts running, it takes some time to complete. The reason for this is the volume of data involved. We have approximately 1,200 market names, and for each market, the pipeline needs to fetch 31 days of weather information from the API. This results in a significant number of API calls and data writes.

Because of this, we allow the pipeline to continue running until it completes successfully. Once the pipeline finishes execution without errors, we can be confident that the logic is working correctly.

With this successful run, we are ready to proceed further. In the next lesson, we will continue after the pipeline has completed successfully and move ahead with the next steps.

# **M) Weather Data Ingestion - Additional Source Column on COPYDATA and Setup Trigger**

The weather data ingestion pipeline is running fine and ingesting the data correctly, but there is one important change that I forgot to implement. We will make that change now and then proceed to schedule the pipeline using a scheduler.

The missing piece is that the market name is not included in the response file. The weather API response does not return the market name because the API fetches data using latitude and longitude. However, we already have the market name available in our metadata file, so we can easily include it in the final output.

To fix this, we open the bronze layer weather data ingestion pipeline. This is also a good opportunity to learn a new technique—how to include additional columns directly in the Copy Data activity source. Instead of modifying the API response, we enrich the data during ingestion itself.

In the sink, we are already passing values dynamically from the metadata file. We can use the same approach in the source by adding an additional column. At the bottom of the source settings, there is an option called Additional Columns. This allows us to dynamically derive new columns and add them to the output.

Here, we add a new column called market_name. For the value, we use Add Dynamic Content. Since the Copy Data activity is inside a ForEach loop, we already have access to the metadata fields. We can simply use item().market_name from the metadata file. This ensures that the market name is included in every output file, making it much easier to reference in later layers.

Apart from this additional column, nothing else in the source settings needs to be changed. There are other default options such as file name and file path that can also be added, but we do not need them for this use case. Our requirement is only to include the market name.

Once this is done, if we check the mapping, we can see that the market name is now included in the sink output. Earlier, this column was missing, and it was a good catch to notice it at this stage. We publish the changes.

Now we move on to setting up the tumbling window trigger. Since we want to load historical weather data month by month, a tumbling window trigger is the best choice. This allows us to process fixed time windows sequentially without overlap.

We create a new trigger and name it something like Weather Monthly Load. The trigger type is Tumbling Window. Our pricing data starts from January 2020, so we set the trigger start date as January 1st, 2020, at 12:00 AM to ensure the full day is included.

The frequency is set to 1 month, meaning the pipeline will run once per month. We also define an end date, which we set to December 31st, 2023, since that is the latest data we want to ingest. The time is again set to 12:00 AM.

For concurrency, we set the value to 1. This is important because the data volume is large, and each monthly load is heavy. Running multiple months in parallel is unnecessary and could impact performance.

Once we confirm the trigger settings, we proceed. The trigger now asks for pipeline parameter values. We already know how this works. The tumbling window trigger automatically provides the window start time and window end time, which we map to the pipeline’s start date and end date parameters. The file format parameter is set to JSON.

Before publishing, we go back to the bronze layer and delete the previously loaded January 2020 data, because that data does not include the market name. Since having the market name is crucial for downstream transformations and merges, it is better to reload everything cleanly using the trigger.

While setting the trigger, we briefly encounter a range error related to invalid time values. This happens occasionally due to time formatting issues. We simply reset the start and end times, verify them again, and proceed.

After fixing the issue, we publish the pipeline and the trigger successfully. The error disappears, and the tumbling window trigger starts running automatically.

At this point, the trigger will load one year (and more) worth of weather data, month by month, into the bronze layer, with each month stored in its own folder and each file containing the market name.

With this complete, the next task is to transform the bronze weather data into the silver layer. The weather data is still in a complex nested JSON structure, so we will need to flatten it, similar to what we did for the geocoding data. That transformation will be covered in the next section.

# **XIV) Data Lake Silver Layer Data Transformation - Demographics Data**

# **A) Demographics Data Transformation - Configure Source and Sink Datasets**

Please make sure that if any of the datasets have not been moved into the proper folders, they are moved accordingly. The idea is that once we complete the development, we should be able to delete the Working Labs folder from each section and apply the final code directly. That approach is perfectly fine.

I noticed that some datasets were not properly cleaned under the datasets section earlier, so I went ahead and cleaned them up now.

At this point, we are moving into the transformation stage of our geo-location data. We have already loaded all the geo-location data for all market names. The next step is to transform this data and make it available for the subsequent gold layer. In the gold layer, we will merge this transformed geo-location data with the actual pricing data that has already been loaded into the reporting database.

Our main requirement here is to extract the population data for each market from the geo-location data and merge it with the pricing data. This merged output will produce a final dataset of roughly 500,000 records, which will then be used for AI and machine learning services.

To start this process, we go to Azure Data Factory and begin creating the datasets required for the transform (silver) layer. Wherever possible, I would like to reuse datasets that were already created. After making these changes, I will ensure everything is published so the updates are applied.

Next, I will close all the open items and open the shared workspace.

We already created the geo-location dataset for the bronze layer, but now we need to use this dataset as a source in the transformation pipeline. Originally, this dataset was created as a sink. As a best practice, we should never mix sink datasets as sources or source datasets as sinks.

Because of this, we will create a copy of the existing dataset. This copied dataset will point to the same location in the Data Lake. While using a Common Model (CM) dataset, the behavior for source and sink is slightly different, but everything still points to the same Data Lake container, and the configuration looks correct.

Although the data still physically exists in the bronze layer, I want to move this dataset definition into the transform folder, because it will now be used in the transformation pipeline.

Similarly, we need to create one more dataset to store the output of the transformed data. For this, we will again reuse an existing dataset and simply change its naming convention from bronze to silver. This allows us to create the dataset quickly without changing much configuration.

All these datasets will continue to exist in the same Data Lake storage account, so nothing significant changes at the storage level. If there are any schema differences between the source and sink, we can handle and correct those during data flow development or pipeline development.

At this stage, we have successfully created the two datasets required for building the transformation data flow.

Now, we move on to using a data flow to transform the source data into the sink data. The reason for this transformation is that the source geo-coding data is stored in a complex structure. Specifically, the source files contain a result array, and inside this array, the data is represented using dictionary (key-value) data types.

However, after transformation, all the fields must exist as flattened, plain columns in the output file. We have already partially implemented this logic while developing the ingestion pipeline for the weather data, where we extracted latitude and longitude values from this same geo-location data.

If you look at the source projection, the data appears in an array format, with values nested inside it. But in the sink, all columns are flattened and appear as individual fields. This is exactly what we aim to achieve again in this transformation.

We will largely reuse the same transformation logic, but this time we will build a proper transformation pipeline to fully prepare the geo-location data for merging with the pricing data.

The final objective is to add the population column to our pricing dataset. This enriched dataset will then be used by AI and machine learning services to analyze how population impacts pricing behavior.

With this understanding in place, we will start creating the transformation pipeline in the next lesson.

# **B) Demographics Data Transformation DATAFLOW Source Wildcard Paths Configuration**

We need to create a data flow because we are changing the structure between the source and sink. The source data exists in a complex data type, whereas in the sink we want to store the data in a flattened format.

So, we navigate to the Transform folder and start creating a new data flow. We follow the same naming conventions that we have consistently used earlier. This data flow is responsible for loading data into the silver layer in the Data Lake, which comes after the bronze layer.

This is no longer raw data. We are transforming the data into a flattened and structured format. Therefore, we name the data flow as Silver Geolocation Data.

Next, we add the source, which is the geolocation data from the bronze layer. We have already created the dataset for this. To make it easier to locate, you can search using the keyword bronze, which will limit the number of datasets shown.

We include the HCM source here, which is the bronze geolocation dataset. If you are unable to find it easily, a helpful approach is to click on the dataset, copy its full name, and search using that exact name. This ensures only one dataset appears, making selection easier. In this case, two datasets may appear—one from Lab 5 and another from the complete implementation.

Once the source is added, if you look at the projection screen, you will see a default schema defined in the dataset. However, the schema has not yet been imported, which is why no fields are displayed initially.

We proceed to import the schema. Since this dataset is parameterized, it is not pointing to any source file by default. During schema import, it will prompt us to supply values for the parameters. We already know that the container name is pricing data lake, the folder name is bronze/geolocation, and for the file name, we can select any one file that contains valid data.

Some of the files may not have data if the API did not return any results. In such cases, there is nothing we can do, and we will discuss that separately. For now, we focus on importing the schema correctly.

After importing, we can see that the schema contains an array data type, and inside that array there are multiple columns. There is also a generation time in milliseconds, which captures the timestamp of when the API request was made. This is useful metadata and good information to retain.

If you look at the projection window now, the schema appears correctly. At this point, we can move to the data preview. To preview the data, we may need to start a debug cluster. This allows us to inspect the data and determine the next transformation steps.

The next major transformation we need is to flatten the array data type, since the values currently exist inside an array. In the data preview, you can clearly see the complex structure that needs to be flattened.

At this point, you might encounter an error that looks familiar. We saw this same issue while developing the lab earlier. The error occurs because the source dataset is parameterized, but we have not yet passed values to those parameters.

We can quickly fix this by passing the parameter values. This needs to be done only once and can then be reused for subsequent runs against the pricing data lake. While entering these values, it is important to ensure there are no typing mistakes. In this case, the file name has already been copied correctly.

Once we save the parameters, the data preview works successfully. Now the data is displayed in its complex data type format.

The ultimate goal of building the silver layer is to make the data easy to merge with the existing pricing data. The pricing data does not exist in this nested format. In the database table, it exists with ID-based columns, and our goal is to merge population data into that pricing dataset.

That is why we are building this silver layer—so that when we populate the gold layer, we can seamlessly merge the pricing data with the population data.

At the moment, the data preview shows only one row because it is pointing to a single market file. This happens because we supplied only one file name during schema import. However, our requirement is to extract data from all source files present in the geolocation folder, not just one file.

To achieve this, we use an additional option in the source settings. Instead of pointing to a single file, we configure the source to use a wildcard path.

It is important to note that the wildcard path does not include the container name. The container name must already be specified in the dataset itself, either as a parameter or as a hardcoded value. In the data flow, we only specify the folder path and wildcard pattern.

We choose Wildcard Path (or Dynamic Content), which opens the Data Flow Expression Editor. The expression is very simple—we do not need to use any special functions. Since all market data files are stored as JSON, we specify the folder path and use a wildcard to read all JSON files from that folder.

After saving and finishing, we go back to the data preview. Initially, it may look like no data is returned. If that happens, we simply refresh the preview from the source.

Once refreshed, the preview displays data from all market JSON files present in the geolocation folder. Now we can see values for all market names.

The final step at this stage is to flatten the result column so that all nested values become individual columns. We will perform this flattening operation in the next lesson.

# **C) Demographics Data Transformation DATAFLOW - FLATTEN Complex JSON Structure**

Now we are going to learn a new transformation that we have not covered before. This transformation is called Flatten. It is used to flatten complex data type columns, not only from JSON sources, but from any source where the data is coming in the form of an array or dictionary structure. Whenever data is nested, the flatten transformation can be used to convert it into a tabular format.

In our case, we will name this transformation Flatten Geolocation Data, as it is specifically applied to our geolocation dataset.

To configure the flatten transformation, we need to set two important options. First, we specify the column that needs to be flattened. When you click on the selection, it displays all complex data type columns that are not grayed out. Any column that is not grayed out means it can be flattened. If a column is grayed out, it cannot be unrolled.

Here, we select the results column. When we move to the Unroll By option, we see that only one unroll route exists. In cases where multiple unroll routes exist, they need to be applied one after another. However, in our scenario, only one route is present. In other datasets, such as weather data or country profile data, multiple unroll routes may exist.

At this point, the preview still shows only one row, which is expected because it is showing the source output. As soon as we apply the Unroll By operation and reset the input columns, the system automatically converts each value inside the array into individual columns. This completes the flattening step.

If we refresh the data preview, we can now see all the data displayed in a fully flattened format. Every nested field has been converted into a separate column.

Although we may not need all of these columns to merge with our pricing data, it is a best practice in a data lake architecture to store all incoming data as-is. Whatever data we ingest, we store it in the data lake. This is very important, as it allows flexibility for future use cases.

When we inspect the flattened data, we notice that some records do not have population values. This is an interesting observation. The geocoding API we used is a global API, which means it returns market names that exist in multiple countries. For example, the same market name might exist in both India and the Philippines, so we receive data from multiple countries.

At this stage, we do not need multi-country data in the silver layer. We can keep the full raw data in the bronze layer, and if required later, we can always refer back to it. For now, we only want to retain records related to India.

Another important observation is that population data is reliably available mainly for India. Some countries do not provide population data globally. For example, we may see records coming from France, including towns with similar names, but population data may be missing. Since our pricing data is also India-specific, we do not need to include population data from other countries for this project.

Therefore, we apply a filter transformation to keep only records where the country is equal to India. In the filter expression, we use the double equals (==) operator to check equality. Once this condition is applied and saved, refreshing the data preview shows only Indian records.

Before loading the data into the silver layer sink, we need to apply one more important filter. Some Indian records still have null population values. Records without population data do not add any value for our use case, so we filter them out as well. This ensures that the silver layer contains only clean and usable data.

Even though these records are filtered out in the silver layer, the raw data still exists in the bronze layer, so no information is lost. The purpose of the silver layer is to clean and standardize data so it can be safely used in the gold layer without data quality issues.

It is important to note that this is open-source data, and data quality is not fully under our control. The primary objective here is to expose you to large datasets and show how to handle them in the best possible way. Some data quality issues are expected, and we have to live with them as part of this project.

Now that we have filtered the data correctly, the final step before loading into the silver layer is to rename the source columns to more meaningful and business-friendly names. We will take care of that in the next lesson.

# **D) Demographics Data Transformation DATAFLOW - Naming Conventions & Configure SINK**

Before loading the data into the sink, we need to apply proper naming conventions so that the dataset is easily readable and understandable by everyone.

We start by renaming the columns using silver-layer–friendly names. The ID column is coming directly from the geolocation API, so we rename it to something meaningful like geolocation_id. Wherever possible, we include the geolocation context in the column name.

The name column actually represents the market name used in our project, so we rename it accordingly. The latitude and longitude columns are standard geolocation attributes, so we keep their names as they are.

The elevation feature code is also kept unchanged. The country code remains the same as well. For the admin1 ID, instead of leaving it as a short technical name, we rename it to administration_id, which is more descriptive. This represents the government or administrative division responsible for that specific area.

The population column is clearly named already, so we leave it as population. The country ID looks good as it is. The country column is renamed to country_name to make it more intuitive.

The admin name column represents the state-level administrative division. In most cases, this maps to a district name, though for some markets it may differ. That variation is acceptable, so we leave it as is.

With the naming conventions finalized, we can now add the sink to the data flow and start loading the transformed data into the silver layer.

We select the sink dataset for the geolocation silver layer. Since we already created this dataset, we can simply copy the dataset name and search for it. Only one matching dataset appears, making the selection straightforward.

Next, we look at the error handling (linked service for errors). If any errors occur during the data flow execution, we could redirect erroneous records to a separate linked service. However, for now, we do not need this functionality. We may consider it later when populating the gold layer.

In the mapping section, auto-mapping is enabled by default. If we uncheck auto-mapping, we can see that the source columns are already correctly mapped to the sink columns based on the renamed fields. Since everything is aligned, no additional manual mapping is required.

Moving to the settings, we review the partitioning options. The data flow supports partitioning, where the debug cluster splits the source data into multiple chunks and processes them in parallel.

For now, we leave the default partitioning settings unchanged. The dataset size is relatively small, and based on the data inspection and preview, the performance looks reasonable.

At this point, everything looks good. We can publish the data flow changes. In the next lesson, we will create the pipeline to execute this data flow and load the transformed geolocation data into the silver layer.

# **E) Demographics Data Transformation DATAFLOW - Configure Pipeline & Pass Parameters**

Let’s start by creating the pipeline under the Transform folder, since this pipeline is responsible for transforming the geo-location data and loading it into the silver layer of our Data Lake.

The easiest and most recommended way to execute a data flow is to drag the data flow directly into the pipeline. When we do this, the pipeline automatically picks up the data flow name, fills in the activity name, and connects the pipeline to the selected data flow without any extra configuration.

Once the data flow is added, it immediately asks for values for the source and sink dataset parameters. In reality, these values are mostly static. For example, the Data Lake container and folder names do not change between runs. Even the sink file name is actually determined internally by the data flow debug cluster. So technically, the values we pass here may not always be used, but without supplying them, the pipeline will not run.

To handle this properly and avoid hardcoding, we create pipeline parameters and pass those parameters into the data flow. This makes the pipeline generic, reusable, and clean. As a best practice, when developing pipelines, never hardcode values unless there is absolutely no alternative.

In this case, we create pipeline parameters for:

Data Lake container name

Data Lake folder name

Data Lake file name

Although we are passing a file name parameter, the source uses a wildcard path, so the actual file name will be ignored during execution. Still, the parameter is required at runtime.

Since the pipeline runs only once and reads all files from the bronze geolocation folder and writes them to the silver layer, pipeline-level parameters are the best approach.

The source and sink parameters look very similar, so while creating them, we clearly distinguish them by naming conventions—either by prefixing them as source and sink, or by using bronze and silver to differentiate them. This naming strategy will also be useful for future pipelines.

To speed things up, we copy the bronze-related parameters and modify them for the silver layer. Instead of recreating everything, we simply change the folder and container references from bronze to silver.

At this point, we realize that the file name parameter is not actually required for either the source or the sink, because:

The source uses a wildcard path to read all files

The sink does not require a fixed file name

To avoid confusion, we go back to the datasets used in the transform layer and remove the file name parameter from both the source and sink datasets.

We open the transform source dataset and remove the file name parameter. Since the wildcard logic already exists in the data flow, this parameter is unnecessary. We repeat the same step for the sink dataset and remove the file name parameter there as well.

After removing these parameters, the pipeline will no longer ask for file name values, reducing complexity and preventing runtime confusion.

Now, we return to the pipeline parameters and map only the container name and folder name parameters to the data flow. We carefully map each pipeline parameter to the correct dataset parameter, paying close attention to the naming because the parameters may not appear in the exact order we expect.

We pass:

The bronze container name and bronze folder name for the source

The silver container name and silver folder name for the sink

Once everything is mapped correctly, we validate the pipeline. The validation completes successfully without any errors.

With that, we publish the changes. In the next lesson, we will run the pipeline and verify that the geo-location data is successfully transformed and loaded into the silver layer of the Data Lake.

# **F) Demographics Data Transformation DATAFLOW Pipeline Debugging And Testing**

Before running the pipeline, we first need to make sure that there is no existing data in the silver folder of our Data Lake. We check the silver/geolocation folder and confirm that it is empty. This ensures that we are loading fresh data and avoiding any duplication or confusion.

Once that is confirmed, we start the pipeline and run it in debug mode. When the pipeline starts, it prompts us to provide values for the pipeline parameters. We pass those values again to ensure the pipeline has all the required inputs.

For the source parameters, we provide the container name as pricing data lake. The bronze folder name is set to bronze/geolocation, which is where the raw geolocation data exists.

For the sink parameters, we pass the folder name as silver/geolocation. This is the location where the transformed files will be generated. The container name remains the same in our case, so we pass pricing data lake again.

After supplying all parameter values, we click OK, and the pipeline starts running.

The pipeline runs smoothly and completes successfully in about one minute. This highlights the power of using the Data Flow Debug Cluster with partitioning enabled. With partitioning turned on, the source data is split across multiple cluster machines, and each machine processes a portion of the data in parallel. This significantly improves performance and speeds up the data loading process.

This behavior is controlled by the default partitioning settings that we configured earlier at the data flow level. Using default partitioning for both the source and sink works well for this dataset.

At this point, the pipeline execution is complete, and the geolocation data has been successfully loaded into the silver layer.

In the next section, we will apply a similar transformation approach for the weather data. There is a lot of data being processed in this project, and if you notice the pipeline history, you may see that some pipelines have failed, some are still running, and many have completed successfully. This is expected when working with real-world data pipelines.

Over the past seven days, we have completed a significant amount of data loading. First, we ingested 365 days of daily pricing data into the landing layer. Then, we loaded the entire dataset into a SQL Server database, including dimension tables and fact tables.

After that, we started loading data into the Data Lake, including geolocation data and weather data. We still need to load the country profile data, which will complete the ingestion process. All of this data is coming in real time from actual source systems.

As part of this process, we also transformed complex data structures. For example, geolocation data originally arrived in nested JSON format, which we flattened and stored as structured files. These flattened files can now be easily merged with the pricing data because they contain market name, state name, and administrative division information.

This prepares us to build the gold layer in the Data Lake, which will be ready for AI and machine learning processing.

In the next section, we will move on to transforming the weather data that was loaded into the bronze layer of our Data Lake. I’ll see you there.

# **XV) Data Lake Silver Layer Data Transformation - Weather Data**

# **A) Weather Data Transformation - Configure Source and Sink Datasets & DATAFLOW**

Now that we have loaded our weather data into the Bronze (branch) layer of the data lake, we can see that the structure of this data is more complex compared to the geo-location data we worked with earlier. This data is not flat and contains nested and array-based structures, which means it cannot be directly consumed for analytics or downstream use cases.

Specifically, within the daily time section, the data is stored in arrays for multiple months, and for each date, there are associated values such as temperature, rainfall, and other weather metrics, along with their corresponding units. These values are represented in complex data types, making the structure harder to work with in its current form. Therefore, similar to what we did for geo-location data, we need to flatten this data and simplify it so it can be used effectively.

To do this, we will start by creating datasets that read the weather data from the Bronze (branch) layer. Once the datasets are ready, we will build a data flow to apply the necessary transformations to flatten the data. The weather data is stored in JSON format, so we will work with JSON datasets.

First, we will clone the existing Bronze weather dataset and rename it by appending “source” at the end, following the same naming convention we used earlier for branch geo-location data. This dataset will continue to point to the Bronze layer, as it represents the source of our transformation process.

Next, we will move this dataset into the Transform folder, since all transformation pipelines are developed there. After that, we will create another copy of the weather dataset, this time aligning it with the Silver layer folder structure. This dataset will act as the sink (target) for our transformation and will point to the Silver layer. While creating this dataset, we will remove the word “source” from its name to clearly differentiate between source and sink datasets.

It is important to note that all data exists in ADLS, which allows us to easily clone datasets instead of creating them from scratch. Although we could create new datasets from the beginning, cloning saves time and ensures consistency. Both the source and sink datasets still point to the same underlying storage, but their logical roles in the pipeline are different.

At this point, we have successfully created the source dataset (Bronze weather data) and the sink dataset (Silver weather data). With these in place, we can now begin building the data flow that will read the weather data, flatten it, and load the transformed output into the Silver layer.

The ultimate goal of this transformation is to merge the weather data with pricing information that already exists in an Azure SQL Server database. Since the weather data is captured at a daily level, it can be easily associated with existing pricing data based on date and market. This enriched dataset will later be used for analytics and machine learning services.

Now, we create a new data flow under the Transform folder. Before applying any transformation logic, it is important to inspect the data to understand its structure. We name the data flow based on the layer and data type, for example: Silver Weather Data Flow.

Inside the data flow, we add a source transformation and select the Bronze Weather Data Source dataset that we created earlier. Since we now have many datasets, copying and pasting the dataset name helps avoid confusion. Once selected, we verify that the dataset connection works correctly.

Initially, when we look at the projection, we may not see any schema information. This is because the dataset is parameterized, and the schema has not yet been imported. To fix this, we go to the Schema tab and choose Import Schema from Connection Store. At this point, Azure Data Factory (or Synapse) will prompt us to provide values for the dataset parameters.

We provide one of the existing weather JSON files from the Bronze layer. Since weather data is loaded monthly and continuously, we select a representative file (for example, from a specific month or year) to infer the schema. This is different from geo-location data, which is usually static and does not change frequently.

Once the schema is imported, we move to the Data Preview to examine the actual structure of the data. Here, we can clearly see that some fields are available as plain columns, while others—such as daily weather values and units—are stored in separate arrays. Additionally, we have included attributes like latitude, longitude, and market name.

Including the market name is especially important because it makes the data easier to reference and join in downstream analytical platforms. While latitude and longitude are useful, the market name is required for consistent integration with other datasets. This aligns with the purpose of the Silver layer, where we standardize and confirm data so it can be reused across the data lake.

At this stage, the data is ready for transformation. In the next lesson, we will focus on flattening the daily rates, daily units, and daily weather values using appropriate transformations so that the final output can be written to the Silver layer in a clean, analytics-ready format.

# **B) Weather Data Transformation - FLATTEN Nested JSON ARRAY Values Level1**

Transcript not available

# **C) Weather Data Transformation - FLATTEN Nested JSON ARRAY Values Level2**

Now we proceed to the next level of flattening, where we focus on flattening the weather code array coming from the source JSON. The number of flatten levels you create always depends on the nested structure of the source JSON file. Since this weather data contains multiple nested arrays, we must flatten them step by step, one level at a time.

At this stage, if you look at the structure carefully, the weather code is the next array that needs to be flattened. In the flatten settings, we choose the weather code array, and specifically select daily weather code. Once this is applied, if you check the data preview, you will notice that the weather code is no longer present as an array. Instead, it now appears as an individual column.

However, even though the weather code is flattened at this level, if you go back and look at flatten level one, you will still see that weather code originally existed as an array. This confirms that the flattening process is working layer by layer. The array existed in one level, and in the next level, it is converted into a proper column.

Next, we create flatten level three. In this level, we flatten the next available array from the source. Here, we unroll based on the time array, the weather code, and the temperature (2 meters max). Once this flattening is applied, these values automatically become common column names instead of remaining inside complex structures.

It is important to understand that all arrays cannot be flattened in a single level when the data is highly complex. Because the JSON contains multiple nested arrays at different depths, Azure Data Factory (or Synapse Data Flow) requires us to flatten them across multiple levels. Each flatten level is responsible for handling one layer of complexity.

After this, we move on to flatten level four. In this step, we flatten the minimum temperature, which is also captured at the 2-meter level. Once this transformation is applied, we quickly verify the output using data preview to ensure that the values are coming through correctly as plain columns.

At this point, we observe that there is only one more nested array remaining. That final array corresponds to rain sum. So, we create flatten level five and apply the flattening logic to the rain sum data. The total number of flatten levels required is completely dependent on how deeply nested the source JSON structure is. If the source contains more nested arrays, additional flatten levels would be required.

Now, when we check the data preview after flatten level five, we can clearly see that the data is fully flattened. All columns are now in a simple, tabular format, and none of them are of complex or array data types. This is exactly what we need before storing the data in the Silver layer.

Before writing the output, we quickly review the column names to check whether any renaming is required. We examine columns such as daily weather, daily temperature, daily rain sum, and market name. Everything looks acceptable and follows the naming conventions required for downstream consumption.

Our primary focus is on the daily time column, because this will be used to join with the pricing date from our pricing dataset. All weather information is associated with a market name, which allows us to combine and enrich the pricing data accurately.

While reviewing the flattened output, we notice that duplicate column names and duplicate records are appearing. This is a common issue when flattening deeply nested arrays, especially when multiple arrays are unrolled independently.

To address this problem, instead of fixing it immediately, we decide to handle it in the next lesson by applying an Aggregator transformation. The aggregation logic will help eliminate duplicate records and ensure that the final dataset contains one consolidated record per market per day, which is exactly what we need for analytics and machine learning use cases.

# **D) Weather Data Transformation - Remove Duplicates and Create Transform Pipeline**

I have now quickly added an Aggregator transformation to the data flow. While working with this transformation, we need to be very careful, because this data flow is resource-intensive. We are processing a large volume of weather data, and it is already in a complex structure before flattening. Because of this, even performing a data preview takes noticeable time.

Since the weather data comes in nested and complex data types, the processing overhead is quite high. However, after applying the Aggregator, we can already see an improvement in the output. Some of the duplicate records are now avoided. For example, if we look at the market count, the same market name was appearing 286 times for the same date earlier. This clearly indicates duplication, and that is why applying aggregation becomes necessary.

Because of this heavy processing, we also need to be careful while scheduling the pipeline. Originally, I thought of scheduling this data flow for one full year, but after observing the resource usage, I am a bit worried. Running this for a year could consume a lot of compute resources and significantly increase the cost.

In fact, while just experimenting with this processing, I noticed that my pricing pipeline cost already went up to around £95. So this is a clear warning sign. We need to be cost-conscious and careful while running such transformations, especially in a real subscription where billing happens automatically.

Also, it is important to understand that we are not directly using this weather data as a final product. Instead, we are preparing and enriching data. Along with pricing information, we are also planning to include population data and weather data, because all of these factors influence price fluctuations of products. That is the main reason we are investing effort into this transformation.

Given the cost and complexity, it makes more sense to process only one month of data, rather than a full year. If we can produce a correct and clean final output for one month, that is more than sufficient for learning and demonstration purposes.

Coming back to the Aggregator transformation, all I have done is apply a group by on the columns required in the final output. This ensures that the data contains unique records only. The columns we are specifically interested in are:

Daily time

Weather code

Temperature (2-meter maximum)

Temperature (2-meter minimum)

Rain sum

Market name

This aggregation guarantees that we get one consolidated record per market per day.

Once this is done, we map the output to the sink dataset that we already created earlier. I select the Silver Weather Data dataset as the sink. The dataset type is correct, and the settings, error handling, and mappings all look fine. I also verify auto-mapping to ensure that every column is mapped correctly. Everything looks good at this stage.

Now, before running the pipeline, we need to adjust the source settings. Since there are multiple files in the Bronze weather data folder (nearly 5000 files per month), we should use a wildcard path. However, for now, we will not load the entire folder. Instead, we will test the pipeline using only one file.

This is a deliberate decision to avoid unnecessary cost and heavy compute usage. By running it with just one file, we can clearly understand:

Whether the pipeline works correctly

How long it takes to run

How resource-intensive the transformation is

To execute the data flow, we create a transform pipeline. Instead of building everything from scratch, I simply copy the existing geolocation pipeline and replace the name with weather data. This new pipeline is clearly identified as a Silver Weather Data pipeline, not geolocation.

As mentioned earlier, we will run it only for one day’s worth of data, not a full month or year. This is because I do not want you to accidentally consume a large amount of money. Remember, we have provided credit card details, and Microsoft automatically bills the subscription. So we must be extremely careful.

While configuring the source parameters, we pass only one file name, not the entire folder path. This ensures the cluster processes only a small dataset. Even though the execution happens on a cluster and can handle large volumes, the data preview performance already indicates heavy processing, which is why we are cautious.

The data lake container name remains the same, and for now, we hard-code the Silver folder path, for example:

Silver/weather_data/2023/01

The file name will be passed through parameters, but since it runs on the cluster, it will process it correctly.

At this point, everything looks good. We publish the changes and ensure that all validations pass. During publishing, we notice a warning related to ForEach iterator settings in the weather metadata pipeline. This is unrelated to the current transformation pipeline and is due to a separate configuration change (iteration count adjustment). We close that and proceed.

Now the pipeline is published successfully. We start the debug run and observe how long it takes to execute. Based on the success or failure of this run, we will analyze the behavior and performance in the next lesson.

# **E) Weather Data Transformation - Removing Unwanted Source Columns & Set Parameters**

We now reopen the data flow and make an important optimization step. The first thing we do is remove the daily unit weather code and daily weather code from the transformation. These two columns are the primary cause of the massive duplication we were seeing in the final output.

The reason for this duplication is that the weather code captures multiple weather conditions across a month. When this data is flattened, it multiplies aggressively—effectively combining 30 days × multiple weather codes, which results in roughly 180 records per market per day. For our use case, this level of granularity is unnecessary and creates both performance and cost issues.

To fix this, we delete the weather code at the very first flatten level. Once it is removed there, we must also delete the dependent flatten level immediately, otherwise the weather code will continue to propagate forward. However, even after doing this, the weather code can still reappear in later flatten levels, so it is critical to remove it consistently at every flatten stage—both at the daily unit level and the daily weather code level.

This cleanup significantly improves the pipeline performance. As mentioned earlier, our goal is simply to bring weather information at the market and daily level into the final output. That is all we need. Weather codes represent very specific conditions and are not required for the pricing and analytical use cases we are building.

We also double-check the sink mappings. If the weather code is still mapped there, we explicitly unmap it. Once this is done, the remaining columns—daily date, temperature (2-meter max), temperature (2-meter min), rain sum, and market name—look correct and aligned with our requirements.

When we run the data preview again, the improvement is obvious. Earlier, the preview took a very long time to return. Now, it comes back within a minute, which is very promising. This confirms that removing the weather code has dramatically reduced data explosion.

Next, we rerun the pipeline for one market again. The execution is still many times faster than the previous version. Even when considering cluster startup time, the data flow completes in roughly one minute, which is completely acceptable.

To be safe, we run it again for one day’s worth of data. This helps us verify that there are no hidden performance bottlenecks. The execution time gives us a good benchmark and helps answer the question: Should we run this monthly or yearly? Based on the results, monthly execution looks reasonable, while yearly execution would still be risky from a cost perspective.

Since the performance now looks stable, we can start automating the transformation pipeline. The plan is to schedule it for one month first, observe the cost and execution behavior, and then decide whether to run it for subsequent months. There is still some concern about cost, but with the optimizations in place, it should be manageable.

To enable automation, we now need to parameterize the dataset values being passed into the data flow. One parameter, such as 202301, represents the weather month (January 2023). This parameter must be derived dynamically, because each run will process a different month. The remaining parameters can be passed directly as pipeline parameters.

We have already implemented similar logic in the ingestion pipeline, so we can reuse that approach here. All we really need is a single dynamic variable that represents the weather month.

We create a pipeline variable called weather_month. During setup, we notice that two variables appear due to copy-paste behavior. To avoid confusion, we delete the duplicate and keep only one clean variable. We then add a Set Variable activity and assign the dynamic value to weather_month.

After checking the settings, we confirm that only one variable exists and that the dynamic content is correctly configured. Everything looks clean and consistent.

Next, we map these values into the data flow parameters. Inside the data flow, we only need to pass values for the folder paths. To do this, we create pipeline parameters such as:

Data lake container name

Bronze folder name

Silver folder name

The container name is the same for both Bronze and Silver layers. The Bronze folder path is:

bronze/weather_data

And the Silver folder path is:

silver/weather_data

These folder paths are then concatenated with the weather_month variable, allowing the pipeline to dynamically process the correct month during execution.

At this point, the pipeline is optimized, parameterized, and ready for monthly execution. In the next lesson, we will pass these values into the dataset parameters and complete the automation setup.

# **F) Weather Data Transformation - Dynamic DATAFLOW Parameter Passing From Pipeline**

Now that we have configured all the variables properly, we can start mapping them into the pipeline parameters. First, we map the container name. We intentionally created only one container name parameter, because the same container is used for both Bronze and Silver layers. Unlike earlier pipelines where we used separate container parameters, here a single container name is sufficient.

Next, we configure the Bronze (branch) folder name. This folder name must change every month, so it cannot be hardcoded. Instead, it needs to be a concatenation of the Bronze folder base path and the variable month. We use the concat() function for this purpose. The first argument is the Bronze folder name, followed by a comma, and then the pipeline variable that contains the month value. This ensures that every monthly run automatically points to the correct folder.

We apply the same logic to the Silver folder name. Again, we use the concat() function, selecting the Silver folder base path and appending the pipeline variable for the month. This keeps both the source and sink paths aligned and dynamic across monthly runs.

Even though the file name parameter is not actively used during execution, we still pass it. The pipeline expects a value, so we provide it to avoid validation issues, even though it does not affect the actual processing.

At this point, we need to make one important change in the data flow. Earlier, the source was reading a specific file name passed through the dataset. Now that we are running monthly loads, we want to load all weather data files within the folder. So we go back to the data flow source settings.

In the source settings, we remove the file name parameter, because it is no longer required. Instead, we switch to using a wildcard path. This allows the data flow to read all files in the specified folder, rather than a single file.

To support this, we must create a data flow parameter. When we loaded geo-location data, the folder path never changed, so we hardcoded it. But for weather data, the folder path changes every month, so a parameter is mandatory. We create a data flow parameter called something like sink_weather_month_folder_name.

For the first run, this parameter value would look like:

silver/weather_data/202301


This parameter will later be used inside the wildcard path configuration in the data flow source.

Now we return to the pipeline and pass the correct value to this data flow parameter. To do this, we use the Pipeline Expression Builder. The value is constructed using:

The pipeline parameter for the Silver folder base path

The dynamically derived month value

A trailing slash (/) to ensure the wildcard path works correctly

This ensures the data flow receives a fully qualified folder path and does not fail due to formatting issues.

Once the expression is configured, we validate the pipeline again. Initially, we might see an error like “No value provided for parameter sink_weather_month_folder_name”, but once the expression is correctly added, the error disappears.

All values are now coming dynamically from:

Pipeline parameters

Pipeline variables (derived month)

Concatenation logic

So the configuration is clean and consistent.

We publish the changes and make sure everything is saved. Before adding any trigger, we decide to run a manual debug execution. This step is very important, because this pipeline is still resource-intensive, and we want to be absolutely sure that it behaves correctly.

I want to be very careful here. I do not want to waste your money by running something too large or too long. So we debug it with one month of data only.

For the debug run:

Weather start date is set to the first day of the month (for example, 01-01)

Weather end date is set to the last day of the month (for example, 01-31)

This ensures the pipeline runs exactly once per month, which aligns with how it will be triggered later.

Based on our earlier one-file test, execution time was very reasonable. So this run should complete without issues. We monitor the execution closely and observe how long it takes, how the cluster behaves, and whether any errors occur.

Once this debug run completes successfully, we will be confident enough to attach a trigger and fully automate the monthly execution.

We will review the results and performance in the next lesson.

# **G) Weather Data Transformation - Identifying and Fixing User Errors**

The job has failed, but this is actually a very good opportunity to understand the root cause of the error. The error message is very clear, and this is where proper naming conventions become extremely valuable.

The failure message shows:

Job failed at source source_bronze_weather_data_read

This immediately tells us where the issue is occurring—at the source. Because we followed meaningful naming conventions, it becomes very easy to identify the exact step that is failing and why.

The error message also clearly shows the path:

/silver/weather_data/202301


Now this is the key problem. We are reading data from the Bronze layer, but the pipeline is trying to read from the Silver layer. There is no such folder in the Silver layer at this point, because Silver is the target, not the source. Logically, this is a big mistake.

When reading data, we should always point to the Bronze (branch) folder, not the Silver folder. So the fix is straightforward.

We go back to the data flow parameters. This is exactly why we created data flow parameters in the first place. Anything that needs to be dynamically passed and used inside data flow expressions or settings must be a data flow parameter. Dataset parameters alone cannot be accessed inside data flow transformation settings.

Inside the parameters section, we notice that the folder name being passed is incorrect. Instead of passing the Silver folder name, we must pass the Bronze folder name, because the source transformation reads from Bronze.

So we update the data flow parameter value to:

bronze/weather_data/202301


This immediately resolves the logical issue. This mistake also strongly reinforces why clear naming conventions are so important—they help us detect and fix issues very quickly.

We start the pipeline again, confident that this change should fix the problem.

However, we encounter one more error, and again, this is due to a small but important oversight. After the folder path, we must specify a wildcard pattern:

*.json


Earlier, we only provided:

.json


Without the wildcard (*), the data flow cannot read all the files in the folder. The correct wildcard path should be:

*.json

As soon as you see this type of error, you should immediately know where to go and what to fix. If you are able to diagnose and correct these issues on your own, that means your understanding is becoming solid.

This is exactly why I intentionally show these mistakes. These are real errors that occur in real projects, and learning how to debug them is far more valuable than seeing only perfect runs.

We correct the wildcard path and debug the pipeline again.

This time, the pipeline starts running successfully. We are loading last year’s weather data, which will later be used for future predictions, and that is completely fine.

The pipeline has now been running for about 13 minutes, which indicates that it is actively processing the data. Most importantly, all earlier errors are gone.

When we navigate to the Silver layer, we can see that the weather data is being written. Multiple files are being created, corresponding to weather data for different markets. This confirms that the pipeline is working as expected.

Everything looks very promising at this stage. Once the pipeline completes successfully, we will verify that all data has been correctly loaded into the Silver layer.

We will review the final output and validations in the next lesson.
