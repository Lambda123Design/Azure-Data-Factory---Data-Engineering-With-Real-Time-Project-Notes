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
