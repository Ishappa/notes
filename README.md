	
wifi pass:C0d!l@r$Trainee
--

https://rmg.codilar.in/
Popup credential
Username : rmg-live
Pass: rmgliveaA@123



Setup IntelliValt in Intellije:
===================================
-->jdk 11.0 install  (sudo apt-get install default-jdk  )--> latest one will install

 (to remove all related jdk 11 version in ubuntu : sudo apt remove openjdk-11-* )
 
 
 
--> sudo rm -r jdk-11 (open terminal specific path delete the folder by using folder name(jdk-11))


-->Drive--> Shared with me -->AEM

-->download files -->intelivalt.Jar and intelli.cli file(extract the file) 

-->Intellij->settings->plgins-> setting-> install plugin from disk-> intelivalt.Jar file

-->Intellij->settings->tools->intellivalut->browse -->extracted cli lib file-> then select cli 3.2.2 file which will be inside li lib file

-->we have to install maven 

Set up enivironment varible jdk and maven in Ubuntu  
======================================================

home->.bashrc

#Setting JAVA_HOME
JAVA_HOME=/usr/lib/jvm/jdk-11
export JAVA_HOME

export PATH=$PATH:$JAVA_HOME/bin

#Setting MAVEN_HOME
MAVEN_HOME=/opt/apache-maven-3.9.3/apache-maven-3.9.3

export MAVEN_HOME
export PATH=$PATH:$MAVEN_HOME/bin



Run instance by using command 
===========================

java -jar aem-author-form--p4502.jar


MySQL for Ubuntu
==================
https://www.devart.com/dbforge/mysql/how-to-install-mysql-on-ubuntu/


Learn about SLing OSGI 
==========================================
https://aemcq5pedia.wordpress.com/2018/01/04/osgi/
https://felix.apache.org/documentation/subprojects/apache-felix-maven-scr-plugin/scr-annotations.html


1. cq:allowedTemplates    --> /conf/wknd/settings/wcm/templates/category-template  --> this prop should give to page jcr:content node
it is use for when creation of page only this template will show other templates will not show.

2.allowedPaths  --->  /content/wknd/us/category-page(/.*)?  -->this prop should give to template jcr:content node
it is use for restrict the template or it will show or this template will available only under category-page

ADOBE EDGE DELEVERY SERVICES
======================================

Steps to create and configure Edge Delivery Services Project and Site.
1. Create new  repository using use this template option from Repo - https://github.com/adobe/aem-boilerplate
2. Install the AEM Code Sync GitHub App on your repository. Open below in browser and install - https://github.com/apps/aem-code-sync

Preview: https://main--{repo}--{owner}.hlx.page/
Live: https://main--{repo}--{owner}.hlx.live/

CLICK THE DRIVE COPY CONTENT CREATE G DOCS IN DRIVE

3. Copy the starter content to your Google Drive.
4. Share docs with helix@adobe.com
5. Use your own Google Drive. Update Google Drive path in fstub.yaml configuration file.
6.download adobesideKick extension.
7.add files to prject using extentions.



DEVELOPMENT FRONT END
================================

created a local branch copied from master

codilar@codilar-HP-ZBook-15-G3:~$ mkdir eds 								----> CREATED eds FOLDER
codilar@codilar-HP-ZBook-15-G3:~$ cd eds								----> chnaged drtry to eds
codilar@codilar-HP-ZBook-15-G3:~/eds$ git clone https://github.com/IshappaN/demo1.git		-----> pulling/cloning the all data from demo1 repo
Cloning into 'demo1'...
remote: Enumerating objects: 58, done.
remote: Counting objects: 100% (58/58), done.
remote: Compressing objects: 100% (53/53), done.
remote: Total 58 (delta 1), reused 34 (delta 0), pack-reused 0
Unpacking objects: 100% (58/58), 122.75 KiB | 2.23 MiB/s, done.

codilar@codilar-HP-ZBook-15-G3:~/eds$ ls
demo1

codilar@codilar-HP-ZBook-15-G3:~/eds$ cd demo1							--> chnaged drtry to demo1
codilar@codilar-HP-ZBook-15-G3:~/eds/demo1$ git branch

codilar@codilar-HP-ZBook-15-G3:~/eds/demo1$ git branch						--> currently i am in main brnach 
* main
codilar@codilar-HP-ZBook-15-G3:~/eds/demo1$ git checkout local					---> changed to local branch
Branch 'local' set up to track remote branch 'local' from 'origin'.
Switched to a new branch 'local'
codilar@codilar-HP-ZBook-15-G3:~/eds/demo1$ git branch
* local
  main


by vscode i modified some code 

codilar@codilar-HP-ZBook-15-G3:~/eds/demo1$ git status						--> modified the code and I need to stag/ add and commit
On branch local
Your branch is up to date with 'origin/local'.

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
	modified:   styles/styles.css

no changes added to commit (use "git add" and/or "git commit -a")

codilar@codilar-HP-ZBook-15-G3:~/eds/demo1$ git commit -m 'first changes'				---> I staged the file 


If cant able to push all data to git so I need to push through VSCODE
=====================================================================

codilar@codilar-HP-ZBook-15-G3:~/eds/demo1$ git status    
On branch local
Your branch is ahead of 'origin/local' by 1 commit.
  (use "git push" to publish your local commits)

nothing to commit, working tree clean
codilar@codilar-HP-ZBook-15-G3:~/eds/demo1$ git branch
* local
  main
codilar@codilar-HP-ZBook-15-G3:~/eds/demo1$ git push -u origin local                               -----> BY USING THIS CMD I PUSHED THE CODE TO GIT

---> then we can check in local brach chnages occured .

----> in console we need to veryfy by   --      https://local--demo1--ishappan.hlx.page/           ----> i jus chnaged main to local   


Local development setup and First code change in Edge Delivery Services project
======================================================================================
- To install aem cli ---> npm install -g @adobe/aem-cli

- To start server 
   Go to repo folder on local machine and execute (in terminal)
    aem up

  ex:  
    codilar@codilar-HP-ZBook-15-G3:~/eds/demo1$ aem up       -->open terminal our repo folder

    
    Note:
We can change the style to our website on live without push to git after compolted out style or functionality they at a time we can push all code to git.


===================================================================================================================

Icons import
==================

https://fontawesome.com/icons --> for search icons
https://cdnjs.com/libraries/font-awesome --> cdn links for import the libraries


Adobe Popfessional Certi:
==========================

https://express.adobe.com/page/wmEF6wQ6rjrQX/

https://solutionpartners.adobe.com/content/solution/us/en/solution-partners/news/2022/06/adobe-certi...

https://express.adobe.com/page/wmEF6wQ6rjrQX/

https://solutionpartners.adobe.com/solution-partners/home/applications/experience_cloud/experience_m...


https://github.com/adobe/htl-spec/blob/1.4/SPECIFICATION.md


under mentioned tags we have to paste on top of our html file for font
======================================================================
css
====
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.1/css/all.min.css" integrity="sha512-DTOQO9RWCH3ppGqcWaEA1BIZOC6xxalwEsw9c2QQeAIftl+Vegovlnee1c9QX4TctnWMn13TZye+giMm8e2LwA==" crossorigin="anonymous" referrerpolicy="no-referrer" />  


js
===

<script src="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.1/js/all.min.js" integrity="sha512-GWzVrcGlo0TxTRvz9ttioyYJ+Wwk9Ck0G81D+eO63BaqHaJ3YZX9wuqjwgfcV/MrB2PhaVX9DkYVhbFpStnqpQ==" crossorigin="anonymous" referrerpolicy="no-referrer"></script>     



cmd:qstartcloud instance: java -d64 -Xmx2048M -jar aem-author-p4502.jar -gui

Project-Installation:(for cloud version aemVersion="cloud" and change version from parent pom refer about of aem tool(version no) )
==============================================================================================================

mvn -B archetype:generate -D archetypeGroupId=com.adobe.aem -D archetypeArtifactId=aem-project-archetype -D archetypeVersion=39 -D appTitle="ISH Sites Project" -D appId="ish" -D groupId="com.adobe.aem.guides" -D artifactId="aem-guides-ish" -D package="com.adobe.aem.guides.ish" -D version="0.0.1-SNAPSHOT" -D aemVersion="cloud"



mvn -B archetype:generate -D archetypeGroupId=com.adobe.aem -D archetypeArtifactId=aem-project-archetype -D archetypeVersion=39 -D appTitle="WKND Sites Project" -D appId="wknd" -D groupId="com.adobe.aem.guides" -D artifactId="aem-guides-wknd" -D package="com.adobe.aem.guides.wknd" -D version="0.0.1-SNAPSHOT" -D aemVersion="6.5.0"


querydebug : 
=========

libs/cq/search/content/querydebug.html

AEM Start
================================================
 java -Xmx1024m -jar jar file name -gui
	or
java -jar aem-author-form--p4502.jar


http://localhost:4502/crx/de/index.jsp#   

http://localhost:4502/sites.html/content

http://localhost:4502/system/console/bundles

===============================================================================================================================================

TOPICS:
====================================
*components
*HTL, Sightly
*Project creation 
*Package management 
*Template
*CQ dialogue
*Rich text box
*page policy,
*client lib- category, allowProxy, embed
*Inheritence 
->slingResourceSuperType- inheriting the content and structure
->slingSuperType- inheriting the content
*Content-Fragment
*Experience-Fragment


WORKFLOWS: 
========================================================

AEM includes a robust workflow system for automating content approval processes. Workflows define a series of steps and actions that content must go through 
	before publication.  0r

In Adobe Experience Manager (AEM), workflows and schedulers are both tools used to automate tasks, but they serve different purposes and are used in different contexts. Here's a detailed comparison between the two:

Purpose:
-----------

Workflows are designed to automate complex processes that involve multiple steps and possibly multiple users. They are often used for content creation, review, approval, and publishing processes.
Features:

Multi-step processes: Workflows can include multiple steps that need to be performed in sequence. Each step can be assigned to different users or groups.

User interaction: Steps in a workflow can require human interaction, such as approvals or edits.
Conditional logic: Workflows can include conditions that determine the path of the process based on certain criteria.

Integration: Workflows can integrate with other AEM services and third-party systems to perform a variety of tasks.

Examples:
-------------

Content approval processes: Submitting a piece of content for review, getting feedback, making revisions, and finally publishing the content.


* Container step
*Participent step
*design step
*process step

Launcher: when you want to automate the trigger of the workflow.

ex: when new page creation some task wants to perform.


Q: Explain the architecture of Adobe Experience Manager.
===============================================================================================================================================

Two Environments:
=================
Author and Publish. The Author environment is where content is created and managed,
while the Publish environment serves content to end-users.

Content Repository:
==================
AEM uses a Java Content Repository (JCR) as its content repository, providing a scalable and hierarchical structure for storing content.

Modular Components:
=====================
AEM follows a modular architecture with components. Components represent reusable pieces of content or functionality, and they can be combined to create pages.

Sightly/HTL Templating:
=====================
Sightly (HTML Template Language) is used for templating in AEM, allowing developers to create dynamic and responsive user interfaces.


OSGi Framework:
===============
AEM is built on the OSGi (Open Service Gateway Initiative) framework, enabling modular development, versioning, and runtime management of Java components.

Dispatcher:
===========
The Dispatcher is a caching and load balancing tool that sits in front of AEM Publish instances. It caches content, enhances performance, and acts as a security layer.

Workflows:
==========
AEM includes a robust workflow system for automating content approval processes. Workflows define a series of steps and actions that content must go through 
	before publication.

Assets and DAM:
===============
AEM has a Digital Asset Management (DAM) system for managing and organizing digital assets, such as images and videos.

Security and Access Controls:
=============================
AEM provides security features, including access controls and permissions, to safeguard content and control user access.

Integration Points:
===================
AEM offers various integration points, including APIs, servlets, and connectors, allowing seamless integration with external systems and services.

===============================================================================================================================================

Q: What is the purpose of the Dispatcher in AEM?
===============================================================================================================================================

A: The Dispatcher is a caching and load balancing tool that sits in front of AEM Publish instances, caching content, and 
	improving website performance by serving cached content to end-users.


Q: What is Sightly in AEM?

A: Sightly is a templating language used in AEM for building HTML-based user interfaces. It was later renamed to HTL (HTML Template Language).

===============================================================================================================================================

Q: template in AEM.

A: A template defines the structure and layout of a page and is used to create pages.
===============================================================================================================================================

Q: What is the purpose of the Design Dialog in an AEM component?

A: It allows authors to customize the appearance and behavior of a component when used on a page.
===============================================================================================================================================

Q: What is the purpose of workflows in AEM?

A: Workflows in AEM are used to automate and streamline content approval processes. They define a series of steps that content must go through before being published.
===============================================================================================================================================

Q: Explain the role of replication agents in AEM.
--

A: Replication agents in AEM are responsible for copying content from the Author instance to the Publish instance. 
   They ensure that approved content is made available to end-users.


Q: How does versioning work in AEM?
===============================================================================================================================================

A: AEM maintains versions of content to track changes over time. When a page is edited, a new version is created. Authors can revert to previous versions if needed.


===============================================================================================================================================
1.what is aem? why it is use.
--

-->content management solution within the Adobe Marketing Cloud. It enables organizations to create, manage, 
	and deliver digital content across multiple channels, including websites and mobile apps.

-->AEM features : include web content management, digital asset management, personalization, multichannel delivery, forms management, and 
	integration with other Adobe Marketing Cloud tools. It is used to streamline content workflows, enhance user experiences, 
	and support digital marketing efforts.



===============================================================================================================================================
2.what is component?

-->component is a modular and reusable building block for creating web pages. 
-->Components represent specific pieces of content or functionality, 
-->such as a text block, image slider, or form. 
-->They are designed to be easily added, edited, and arranged within AEM's content management system,
 	providing a flexible and efficient way to structure and customize web pages.
-->developed by using scripting language as a html or htl



===============================================================================================================================================
3.what is content fragment?

Content Fragments:

-->Purpose: Content Fragments are structured content pieces designed for easy reuse across different pages, channels, and projects.
-->Structure: They consist of structured content elements, such as text, images, and other components, organized in a modular and reusable manner.
-->Reuse: Content Fragments are primarily used for managing and reusing textual and media content across various parts of a website or different digital channels.
-->Flexibility: They provide flexibility by allowing content authors to create and maintain content in a structured way, ensuring consistency and ease of updates.

Uses:

*They focus on the creation and maintenance of individual content items, such as text, images, videos, etc.

*Content Fragment might contain a single product description, a news article, or a recipe.

*Content Fragments manage individual pieces of content in a modular and reusable manner.



===============================================================================================================================================
4.what is experince fragment?
 
Experience Fragments:

-->Purpose: Experience Fragments go a step further by bundling not only content but also layout and design components.
   Content + Layout + Design:
-> Experience Fragments include the actual content (text, images) along with the layout and design elements,
   providing a more comprehensive and reusable package.


Uses:

*combination of various content elements like text, images, videos, and components to create a complete experience.

*hero banner, a promotional section, or a complete campaign landing page with multiple components.

===============================================================================================================================================
5.what is cq dialog?

-->Edit Dialog: Defines the authoring interface for the component and independent for the content. 
		It includes fields for configuring the component's properties, 
		such as text, image sources, or other options.

	User Interface: They provide a user-friendly interface for content authors to interact with components and customize their behavior.

	Development: Developers create CQ Dialogs using Granite UI, an AEM-specific markup language, defining the fields, options, and constraints 
			that authors can modify when using the component.


-->Design Dialog: Allows authors to configure the component's appearance within a page template.


===============================================================================================================================================

6.what is mean by out of box components?

-->"Out-of-the-box components" refers to pre-built or pre-packaged components that come with a software or platform by default, 
    without the need for additional customization or development. These components are ready to use immediately after installing or setting up the software, 
    providing essential functionalities and features without requiring users to create them from scratch.


===============================================================================================================================================

7.sling:resourceType and sling:resourceSuperType?

-->sling:resourceType:
	sling:resourceType identifies the specific type of the content and determines its rendering logic.
	Points to the location of the component's rendering script or template in the repository.
	----------------------

-->sling:resourceSuperType:
	sling:resourceSuperType facilitates code reuse by allowing a component to inherit rendering logic from a parent component.


===============================================================================================================================================
8.what is Dispatcher and uses?(apache web server has a despactcher it will help to interact with server to aem)

*below mentioned featurs will apply both apache web server and dispatcher (dispacture is a part of apache web server)


-->Dispatcher is a caching and load-balancing tool 
-->use for optimizing the performance and security of AEM websites.

*Caching:
	One of the primary functions of the Dispatcher is to cache content served by AEM. Cached content is stored on the web server itself,
	 reducing the load on the AEM instance and improving response times.

*Load Balancing:
	The Dispatcher can be configured to distribute incoming requests across multiple AEM instances, providing load balancing. 

*Security:
	The Dispatcher acts as a security layer by blocking direct access to certain resources on the AEM instance. 
	It can be configured to only allow access to specific URL patterns

*Reduced Server Load: uses in aem


===============================================================================================================================================
9.what is overlay and override?

OVERLAY: When you overlay a node, you create a copy of the original node in a custom location within the repository. 
	The custom location is typically under the /apps directory. 
	AEM gives precedence to content in the /apps directory, so your custom content overrides the original content.

OVERRIDE: Overrides are commonly used when you want to replace or extend the behavior of existing AEM functionality without altering the original source code.

			
===============================================================================================================================================
10.what is editable templates and how to create it?

-->allow authors to define and modify the structure and layout of a page directly within the authoring environment. 

With editable templates, authors can create and design pages without the need for developers to intervene for every change.

all templates are present in config


===============================================================================================================================================
11.what is osgi services and osgi config and how to create?

creation:
1.create service class @component(service=interfacename.class)
	@designate(ocd and desgnate is for locating the osgi conf interface)

2.Create an OSGi Configuration  by using @objcladefini and @interface and @attridefenition
3.create interface and implemnting to class


SERVIECE in AEM:
---------------

What is it?
In AEM, a Service refers to an OSGi (Open Service Gateway Initiative) service, which is a modular and reusable component.


What does it do?
Services encapsulate functionalities or business logic that can be reused across different parts of the application buy using @Reference.

Key Functions:

Modularity: It promotes a modular approach, allowing functionalities to be divided into smaller, manageable units.
Reusability: Services can be reused in different parts of the application or shared among multiple components.
Integration: They facilitate integration with AEM, enabling interaction with the content repository, performing operations, or handling events.


===============================================================================================================================================
12.what is servlets and creation?

SERVLET in AEM:
-------------------
What is it?
A Servlet in AEM is a Java class that handles incoming HTTP requests and generates responses.

What does it do?
It processes requests made to the AEM server, performing tasks such as retrieving content, handling form submissions, or interacting with AEM resources.


Key Functions:

Request Handling: Receives requests (e.g., for web pages or data) from browsers or clients.
Response Generation: Generates and sends back responses (e.g., web page content, JSON data) based on the request.


Simplified Comparison:

Servlet is like a specific task performer that handles incoming requests (like a receptionist taking requests at the entrance of a building).
Service is like a multi-tool that provides specific functionalities or services that can be used by various parts of the application (like a toolbox with tools that can be used by different people for various tasks).

Summary:
Servlet: Handles incoming requests and generates responses in AEM.
Service: Provides reusable functionalities or business logic that can be utilized by different parts of the application.
In essence, Servlets handle HTTP requests and responses, whereas Services are modular components offering reusable functionalities within the AEM environment.



===============================================================================================================================================
13.what is schedulers and creation?

-->Schedulers automate task execution at specified intervals, managing the timing of recurring activities in software. 
	They enable automation of processes like data updates and maintenance routines, enhancing efficiency.


Creation:

1.Define a Job Interface:
	package com.example.scheduler;

	public interface MyScheduledJob {
   		 void run();
	}

2.Implement the Job:

	package com.example.scheduler;
	public class MyScheduledJobImpl implements Job {
    		@Override
    	public void run(JobContext jobContext) {
        
   	 }
	}

3.Configure the Scheduler:

	@Component(immediate = true)
	public class MyScheduledJobImpl implements Job {
  	  @Reference
  	  private Scheduler scheduler;

   	 // Other components can use this method to trigger the job manually if needed
    	public void triggerJob() {
    	    scheduler.fireJobAt(null, null);
    	}


===============================================================================================================================================
14.what is sling models and explain the all annotations uses?

-->Sling Models are a way to map the content of a resource in the repository to a Java object.

1.@Model:This is the primary annotation used to mark a Java class as a Sling Model. 


-->@Inject: directly extracting specific property values from the resource's 

-->when: It is used to directly inject specific properties from the resource into your Sling Model class fields.


--> @ValueMapValue : It is used to retrieve values from the ValueMap of the resource. The ValueMap is a map-like interface representing the properties of the resource.

-->when: when you want flexibility and might need to handle various properties, including inherited ones.(if current resource property not present it will take parent one)

@Default annotation will consider default value if no value authored.

@Required annotation make sure resource having property.

@Optional annotation is to tell model field is optional.

@Named(“property_name”) annotation in case field name didn’t get match with property name.


@Self:
Purpose: Injects the adaptable object itself into the model.
Usage: @Self

@Via annotation helps you specify the path or property to navigate through when adapting the resource.

it will go through that path or object which one we specify or where to find the data to fill in the fields or methods of your Java class.

Usage: @Via("path/to/property")

@ScriptVariable:
Purpose: Injects objects available in the scripting context (e.g., request, response).
Usage: @ScriptVariable

@DefaultInjectionStrategy:
Purpose: Sets the default injection strategy for fields.
Usage: @DefaultInjectionStrategy

@PostConstruct:
Purpose: Methods annotated with @PostConstruct are executed after object instantiation.
Usage: @PostConstruct

@RequestAttribute:
Purpose: Injects a request attribute.
Usage: @RequestAttribute

@RequestParameter:
Purpose: Injects a request parameter.
Usage: @RequestParameter

@RequestHeader:
Purpose: Injects a request header.
Usage: @RequestHeader

@RequestParameterMap:
Purpose: Injects the request parameter map.
Usage: @RequestParameterMap

@ResourcePath:
Purpose: Injects the resource path.
Usage: @ResourcePath

@ChildResource:
Purpose: Injects a child resource.
Usage: @ChildResource

@InjectDefault:
Purpose: Injects a default value when the original injection is null.
Usage: @InjectDefault(values = {"default1", "default2"})

@InjectorsSet:
Purpose: Combines multiple injectors for the same field.
Usage: @InjectorsSet


===============================================================================================================================================

15.what is a workflow and how to create, why it is use?

--> workflows are often used to its a step by step automate and streamline the approval, review, and publishing processes of content.

-->workflows in AEM streamline content management processes,providing an automated and 
   controlled way to manage the lifecycle of digital assets and content within the system.

-->workflows are stored in two places var(run time model) and config(model design)

Creation: 

-->tools -> workflow--> create models add participant or varsions edit the versions compo specify the page path then start work flow then can check in timeline 

--> create lauchers to trigger the workflow-->event type: modifeid(whene somthing chnahes or modified our luncher will excecute)
	nodetype: cq:page(if workflow is applying for page), select path of the page, select our newly createdworkflow ,
	 check the activate(our laucher will activte to our specific workflow)

1.model: cteating work flow models
2.instances: use for individual work flow excecution
3.launches : trigger the work flow mean which type(modification , creation, etc)
4.archive :check the history or details of the workflow .
5.failures : if failures will occur in our workflow we can go through it


===============================================================================================================================================
16.what is querry builder and uses? write querrys

-->Query Builder is a powerful querying mechanism used to retrieve content from the JCR (Java Content Repository).

-->Uses of Query Builder in AEM:

1.Content Retrieval:
Retrieve content based on specific criteria, such as node types, properties, or paths.

2.Search Functionality:
Implement search functionality on AEM websites, enabling users to find content based on keywords, tags, or criteria.

3.Custom Component Development:
Build custom components that dynamically display content based on specific conditions or filters.

4.Content Synchronization:
Synchronize content between AEM instances or environments by retrieving and replicating specific sets of content.

5.Asset Management:
In AEM DAM, search and retrieve digital assets based on metadata or properties associated with the assets.


===============================================================================================================================================
17.what are event handlers and event listeners?

EVENT LISTENERS:
-->Event listeners are often used to respond to lower-level JCR events, such as node creation, modification, or deletion.
-->They are suitable for scenarios where you need to capture changes at the content repository level.

--An event is listened by implementing EventListener interface which belongs to javax.jcr.observation package.

--onEvent(): This method is executed when an event is listened. The business logic is written inside this method.

EVENT HANDLERS:
--->Event Handler is responsible for Sling Level Events. It uses the OSGi Event Admin service to receive events.
-->Event handlers are commonly used for intercepting and processing events related to resource modification, replication, workflow, etc.
-->They can be configured to execute custom logic when events like content creation, modification, or deletion occur.

--How to listen to an Sling Level event?

An event is listened by implementing EventHandler interface which belongs to org.osgi.service.event package.


Handler Implementation will consist of one method i.e. handleEvent (Event event). handleEvent method gets called whenever event occurs.


===============================================================================================================================================
18.what is sightly and types?

Data-sly-use Directive:

-->It allows you to define and use Java objects directly in HTL.

1. HTML Block:
	The basic block in HTL is the HTML block, which allows you to write regular HTML markup.

Example:<div class="container">
    <h1>Hello World</h1>
</div>


2. Text Block:
	The text block is used to output plain text or variables.


Example: ${variable}


3. Expression Block:
	The expression block is used to evaluate expressions and output their results.

Example: ${expression}

*  data-sly-use:  is a directive used to include and instantiate a Sling model or a Java object within a Sightly script. 


4. Conditional Block (data-sly-test):
	Conditional blocks allow you to conditionally render content based on a specified condition. If the condition is true, the content within the block is rendered.

Example:

<sly data-sly-test="${condition}">
    <p>This will be displayed if the condition is true.</p>
</sly>


5. Loop Block (data-sly-list):
	Loop blocks allow you to iterate over a collection and generate content for each item in the collection.

Example:
<ul>
    <sly data-sly-list="${items}" var="item">
        <li>${item}</li>
    </sly>
</ul>


6. Repeat Block (data-sly-repeat):
	The repeat block allows you to repeat a block of content a specified number of times.

Example:


The main difference between data-sly-list and data-sly-repeat is that data-sly-list allows for specifying additional behavior for when the list is empty. It's typically used when you want to render different content or handle edge cases based on whether the list is empty or not.




<sly data-sly-repeat="${3}">
    <p>This will be repeated 3 times.</p>
</sly>


7. Switch Block (data-sly-switch and data-sly-case):
	The switch block allows you to specify different cases and execute different code based on the value.

Example:

<sly data-sly-switch="${variable}">
    <sly data-sly-case="value1">
        Content for value1
    </sly>
    <sly data-sly-case="value2">
        Content for value2
    </sly>
    <sly data-sly-default="">
        Default content
    </sly>
</sly>

These blocks provide flexibility in controlling the behavior and rendering of your templates in AEM using HTL.




8. data-sly-resource:

<!-- Access a component from within another component -->
<div data-sly-resource="${'aem-training' @ resourceType='path/to/other/component'}"></div>



11. data-sly-template:
<!-- Define a reusable template -->
<template data-sly-template.aem="path/to/template/file.html">
    <!-- Template content -->
</template>


9. data-sly-attribute:

<!-- Conditionally set or add attributes -->
<div class="${PageTitle}" data-sly-attribute.title="${title}"></div>



10. data-sly-call:
It allows you to call a template and pass parameters to it. This facilitates the reuse of the same template in different contexts.

<!-- Call a template defined with data-sly-template -->
<div data-sly-call="${aem @ template='path/to/template/file.html'}"></div>


11.dta-sly-unwrap:

it is use for removing the unwanted tags


===============================================================================================================================================
19.what are the global objects in sightly? and mention.
	

-->several global objects that are automatically available for use within Sightly scripts. 

1.properties: Provides access to the properties of the current resource. 

2.currentPage: Represents the current page being rendered. ex: <p>${currentPage.title}</p>

3.designer: Available when the script is executed in the AEM Sites editor. It provides access to design-related information, such as the design path.
		ex: <p>${designer.path}</p>

4.wcmMode: Provides access to the current request object, allowing you to retrieve request-specific information.
		Ex: <p>${request.requestURI}</p>

	
5.request: Represents the current WCM mode (Web Content Management mode). It is often used to conditionally render content based on the editing mode.
		Ex:<div data-sly-test="${wcmmode.edit}">Editable Content</div>

6.resource : Represents the current resource being processed. It allows access to properties and other information about the current resource.
		Ex: <p>${resource.path}</p>

7.log: Provides access to a logging object, allowing you to log messages from within your Sightly scripts.
	Ex:<!-- Log a message -->
		${log.info('This is an informational message')}

8.helper: helper global object in Sightly for various operations such as string manipulation, date formatting, URL encoding/decoding, math operations, and JSON parsing. 
	Ex 1: <!-- Format a date -->
	<p>${helper.formatDate('2023-01-01T12:30:00', 'dd/MM/yyyy')}</p>

	Ex 2: ${helper.toLowerCase('HELLO')}



===============================================================================================================================================
20.Adapters and Adaptabels?


Adaptables:
-->its a java object / interface and adaptTo() method is commonly used convert one type of object into another.

-->Adaptables provide a way to obtain different views or functionality from a single RESOURCE.

Adapters:
-->these are java classes and implememnted adaptable interface
-->Adapters are used to provide additional functionality to a existing class or resource or object without modifying its original code.

ex: if you want to fetch request based values, you will pass SlingHttpServletRequest.class to adaptables.

Use adaptables = Resource.class when:
--------------------------------------
You primarily need to work with content stored in the JCR repository.
You want to create Sling Models for components that represent content resources.


Use adaptables = SlingHttpServletRequest.class when:
----------------------------------------------
You need access to request-specific information.
You want to create Sling Models for components that require interaction with the current HTTP request.


===============================================================================================================================================

21.GraphQL?

Single Endpoint:
-->GraphQL typically exposes a single endpoint for all interactions, simplifying the API surface compared to REST.

-->GraphQL is particularly beneficial in scenarios where clients have diverse data requirements, need real-time updates,
 or want to avoid over-fetching or under-fetching of data. 

-->Batched Queries:

   Clients can send multiple queries in a single request, reducing the number of HTTP requests and improving performance.

===============================================================================================================================================

22.What are the key advantages of using AEM?

->Some advantages of AEM include its robust content management capabilities, 
->scalability, ability to deliver personalized experiences,
->integration with other Adobe products,and flexibility to create diverse digital experiences across channels means different platform.

Scalability:system to handle increased demands, workload, or growth without compromising performance or stabilit

means making a system that can do more work or handle more users without slowing down or breaking.




PROJECT SET UP: 

https://experienceleague.adobe.com/docs/experience-manager-learn/getting-started-wknd-tutorial-develop/project-archetype/project-setup.html?lang=en
---------------------------------------


HTL:HTML Template Language (HTL) is the preferred and recommended server-side template system for HTML in Adobe Experience Manager

HTL Layers

1.HTL Specification - HTL is an open-source, platform-agnostic specification, which anyone is free to implement.
2.Sling HTL Scripting Engine - The Sling project has created the reference implementation of HTL, which is used by AEM.
3.AEM Extensions - AEM builds on top of the Sling HTL Scripting Engine in order to offer developers convenient features specific to AEM.


Two different kinds of syntaxes:

Block Statements - To conditionally display the <h1> element, a data-sly-test HTML5 data attribute is used. HTL provides multiple such attributes,
		 which allow attaching behavior to any HTML element, and all are prefixed with data-sly.

Expression Language - HTL expressions are delimited by the ${ and } characters. At runtime, these expressions are evaluated and their value is injected into the outgoing HTML stream.


===========================================================================================================================
List of BLOCKS:
===========================================================================================================================

===========================================================================================================================
${properties.name1}<br>

${properties.date}<br>

${'yyyy-MM-dd' @format=properties.date}<br>

${'welcome{0}' @format=properties.name1}<br>

${'welcome ,{0}, {1}' @format=[properties.name1,properties.name2]}<br>

===========================================

*HTL OPERATORS

1.Logical Operators :AND, OR, NOT

Ex:
->.AND:<p data-sly-test="${properties.jcr:title && properties.jcr:description}">DISPLAY</p>
->.OR:<p data-sly-test="${properties.jcr:title || properties.jcr:description}">DISPLAY</p>
->.NOT:<p data-sly-test="${!currentPage.hasChild}">DISPLAY</p>

2.Conditional(ternary) Operators
3.Comparison Operators
4.Grouping parentheses 
5.Relational Operators

===========================================================================================================================

GLOBAL OBJECTS:
=============================

Variable Name				Description									Backed By
properties			List of properties of the current resource			org.apache.sling.api.resource.ValueMap
pageProperties			List of page properties of the current page			org.apache.sling.api.resource.ValueMap
inheritedPageProperties		List of inherited page properties of the current page		org.apache.sling.api.resource.ValueMap

===========================================================================================================================
CREATING TEMPLATE:

tools->general->config browser->create (folder)editable temp -> home page -> tool -> Templates -> select our newly created folder -> html 5 temp ->policy(give allowed comp and all) ->drag one experience fragment(select the pathn of availabl header and footer)(create here header and footer)

(templates is stored in config folder)(while craeteing the pages make the template enable and add the allowed template(path) in properties(give the path of the template


modes :
=====
layout mode --- we can give width of any component(adjust the size for diffrent component)
structure mode -- giving the policies and locking and unlocking components(if we lock here we cannt acces in intial comp mode and also in the pages wecant edit)
initial content ---in this mode if we have created any no. of pages with the template and may have some content and if we change the template some content in initial content mode it will be reflected to next creating page not pages which are already craeted usinfg the template


we can create our own header or footer in experieence fragments



@context --'html',script,text,........upto 7 or 8

========================================================

creating the content fragment:
=============================

tools->cofiguration browser(conf folder in crdex) ->create folder (select as Content Fragment Models)->tools->assets -->content fdragment model
->select your folder(if we create the content fragment model(it is like a skeleton) inside the project folder then we can see it in crxde
-> cfg folder inside it we will have the content fragment in the project folder ,otherwise content frag will be outside only)
-> create the model->drag the data types add the propertries inside it.
->then go back and go to normal navigationn page ->Select Assets ->Files ->create folder and select the folder and properties 
->cloud service ->in here select the path and then open the folder again and create content fragment->create variations there 
->go back and go t sites and create the page in your project thre add the content fragment component (here select path of the content fragment variation we have created)


=============================================================================================================================

Creating Languagecopy/livecopy:
==============================

ex: 1. from wknd page->create page as LanguageMaster->click on Languge Master and create page as english name:en(Languge Master is parent) 
    2.create few pages (english page is parent)->
    3.create Laguage copies(under english page)->select Default configuration it will take automayically Mcrosft.TT.license
    ->Target Language(s) selct few languages->click on create->select project as multi transaltor click create 
    4.create new blueprint root location as our lagugemaster(in crxde apps->msm->our bprint will be) for site creation.
    5.sites(tool) options->create->select rootlocation as lagugemaster->then we can create sites->
    6.select our wknd page it will show ->create sites for all coutry->select our newly created bprint->
      ->title=give countryname(ex:Arab), name=sitename(ex:ar),siteowner=admistrator,chck=livecopy,rollout=standardrolloutconfig
      ->then remove unwanted languages and put what we want
    7.

Advantages: if we create a any content or pages for the language copy it will apply to all the all live copies

ex: if i created content or page for english laguge copy when we call rollout it will apply to all sites english live copy


MSM:
----
after created the sites and langua copies we have to sent lagugaes

1.go to projects-> open our projects -> start refresh and complete to all pages

2.if we want to add laguage to each selected components to pages go to general-> transitionproject->content-> edit-> add component-> selectPath remove apps/ from path
   -> add property name field name which we want transalte in component ex: name of the feild--> if we want add extra laguage property to feild 
	you can add dynamically-->crxde->config-> global-> transition -> open rule find your property and add extra

3.go back to prject -> add-> translation job -> new one will get create ->select target -> laguage-> 3 dots-> add--> asset pages-> 
	select you loc of page should get translate which one has compo (we should add component before selection of loc of page)
============================================================================================================================


Servlets:
----------------		OSGI

				 |
	CLIENT  --->	 SERVLET CONTAINER(X,Y,Z)   --->   PACKAGES(X,Y,Z)
	         	
	  	
Servlet: it is used run the our java code on the server.
Servlet Container: it will have no of servlets(x,y,z) and each servlet has a differnet packages.
OSGI: it will manage the the no of Packages




	@OSGI Service

1. ResourceType based servlet

2. path based servlet

    -> we can extends in 2 ways

1. SlingSafeMethodServlet :-> Read operation/Get

2. SlingAllMethodServlet :->  Read and write (Get and Post) both we can work

https://developer.adobe.com/experience-manager/reference-materials/6-5/javadoc/org/apache/sling/api/servlets/ServletResolverConstants.html 
http://localhost:4502/system/console/bundles

====================================================================

Node API : 

1. Sling API
	->REsource Resolver - 1.System User and 2.SlingHttpServaletRequest		
	->Resource
	->Value Map
	->Modifable ValueMap


=======================================


video

<sly data-sly-use.template="core/wcm/components/commons/v1/templates.html">

<div data-sly-use.video="com.adobe.aem.guides.wknd.core.models.VideoComponent">

    <video controls autoplay loop muted >

        <source src="${video.desktopPath}" type="video/mp4" media="width: 100%)">

        <source src="${video.mobilePath}" type="video/mp4">

      <h3 style = "color:red" >  Your browser does not support the video tag. </h3>
    </video>


</div>

</sly>

<sly data-sly-call="${template.placeholder @ isEmpty=!headEmpty, classAppend='cmp-title'}"></sly>

===========================================================

COMPONENTS:

Definition: Components are reusable modules or building blocks within AEM used to structure and design web pages. 
	    They encapsulate specific functionality, content, or both. Examples include image carousels, text blocks, navigation menus, etc.

Characteristics:

Reusability: Components can be used multiple times across various pages within a site.

Customization: They allow for customization through parameters, enabling authors to configure component behavior or appearance.

Flexibility: Components are usually designed to be flexible, accommodating various content types and design requirements.

Development: Components are created using HTL (HTML Template Language) or JSP (JavaServer Pages), allowing developers to define the structure, behavior, and presentation of the component.

=================================================================
CQ Dialog:

Definition: CQ Dialogs (CQ stands for Communique, the former name of AEM) are authoring interfaces used to configure and set properties for AEM components.

Purpose:
->Property Configuration: CQ Dialogs allow authors to set parameters, define content, and configure component settings without directly manipulating code.

->User Interface: They provide a user-friendly interface for content authors to interact with components and customize their behavior.

->Development: Developers create CQ Dialogs using Granite UI, an AEM-specific markup language, defining the fields, options, and constraints 
		that authors can modify when using the component.

->Functionality: CQ Dialogs facilitate the separation of content and presentation by enabling authors to manage content 
		 independently of the underlying code of the component.


	In summary, Components are the building blocks used to create web page structures and functionalities,
 	while CQ Dialogs provide an interface for authors to configure and customize the behavior and properties of these components 
	without directly dealing with the underlying code. Together, they streamline the content authoring and management process in AEM.


===============================================================================================================================================

Repoinit language examples.
============================================

1. --------------Create System/service user and add permissions----------
create service user aemgeeks-service-user with path /home/users/system/geeks/aemgeeks-service-user

set ACL for aemgeeks-service-user
allow jcr:read,rep:write on /content/aemgeeks
allow jcr:read on /conf/aemgeeks
allow jcr:read on /apps
end

2. --------------Create user group and add permissions----------
create group geeks-users with path /home/groups/geeks-users
set ACL for geeks-users

allow jcr:read,rep:write on /content/aemgeeks
allow jcr:read,rep:write on /conf/aemgeeks
allow jcr:read,rep:write on /apps/aemgeeks
allow jcr:read,rep:write on /home
allow jcr:read on /
end

3. --------------Create user and add user to user group----------
create user geeks-admin with path /home/users/geeks/geeks-admin with password 12345

add geeks-admin to group geeks-users

4. --------------Create Page(any node) and add properties----------
create path /content/aemgeeks/ca(cq:Page)/jcr:content(cq:PageContent)
set properties on /content/aemgeeks/ca/jcr:content
set sling:ResourceType{String} to aemgeeks/components/structure/geeks-content
set cq:template{String} to /apps/aemgeeks/templates/geeks-content
set jcr:title{String} to Canada
end

Official documentation :  https://sling.apache.org/documentatio...


Javascript
=======================
let promise = fetch("http://localhost:4502/crx/de/index.jsp#/apps/eeeee/component/ajaxEx/ajax.txt");

promise
  .then((response) => {
    try {

      return response.text();
    } catch (error) {
      console.log(error);
    }
  })
  .then((data) => {


    document.getElementById('#ajax').innerHTML=data;
  })
  .catch((error) => {

    console.log(error);
  });
