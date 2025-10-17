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
