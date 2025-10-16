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
