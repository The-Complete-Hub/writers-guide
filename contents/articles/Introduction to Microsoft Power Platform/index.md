---
slug: introduction-to-power-platform
title: Introduction to Microsoft Power Platform
author: [favour adeshina]
tags: [Power Platform, LowCode, Power Pages, Power Apps, Power Automate, Power BI]
---

This article is targeted at young innovative minds, who are passionate about building amazing products with Low-Code tools. 

It will be a detailed break down of Microsoft Power Platform for someone who is just hearing about this for the first time, or someone who needs clarity around what Microsoft Power Platform is about. 

Lets talk!

Microsoft's Power Platform is a No-Code/Low-Code Platform for Building amazing solutions faster with very little or no code. Hence the reason it is classified as a **Low-Code** product.

Power Platform comprises of five key products, which are: **Power Apps, Power Automate, Power BI, Power Virtual Agents, and recently Power Pages (recently called Portals)**

Microsoft Power Platform products/tools allows you to automate processes, build mobile and web app solutions faster, analyze data, and create virtual chat agents, powered by Artificial Intelligience. 

Now let us learn more about these products: 

## Power Apps

![powerapps.jpeg](./Power%20AutomateD.png)

Power Apps provides a rapid low code development environment for building custom apps for business needs. 

Microsoft Power Apps is not used for building ordinary custom applications, but apps built using Power Apps provide rich business logic and workflow capabilities to transform your manual business operations into digital, automated processes.

It has services, connectors, scalable data services and app platform (Microsoft Dataverse) to allow simple integration and interaction with existing data, giving you the ability to connect with data from different sources using [Standard and Custom Connectors](https://docs.microsoft.com/en-us/power-apps/maker/canvas-apps/connections-list). 

With Power Apps, you build **Canvas apps or  Model-Driven apps**, by connecting your business data that is stored either in the underlying data platform (Microsoft Dataverse) or in various online and on-premises data sources (SharePoint, Excel, Office 365, Dynamics 365, SQL Server, Google Sheets and so on).

*Microsoft Dataverse lets you securely store and manage data that is used by business applications. Data within Dataverse is stored within a set of tables.*

Find out more in this documentation: [What is Microsoft Dataverse?](https://docs.microsoft.com/en-us/power-apps/maker/data-platform/data-platform-intro)


### Canvas Apps
A Canvas app just like the name implies is an app built by dragging and dropping elements onto a canvas, just as you would design a slide in PowerPoint.

Canvas apps give you the flexibility to arrange the user experience and interface the way you want it. Allow your creativity and business sense to guide how you want your apps to look and feel.

With Canvas apps you build apps that integrate business data from a wide variety of Microsoft and third-party sources. 

Check out this Codelab [Create a canvas app from a sample template in Power Apps](https://docs.microsoft.com/en-us/powerapps/maker/canvas-apps/open-and-run-a-sample-app), to find out more and build your first Canvas App. 

### Model-Driven Apps

Model-Driven Apps or Process Driven Apps design is an approach that focuses on adding components such as forms, views, and charts and dashboards to tables using an app designer tool. 

Model-driven apps starts with your data model – building up from the shape of your core business data and processes in the Dataverse to model forms, views, and other components.

Model-driven apps are highly responsive across several devices.

Additionally, relationships connect tables together in a way that permits navigation between them and ensures that data is not repeated unnecessarily.

While they're called model-driven apps, it is often easier to think of them as data model-driven apps. 

This is because, without a data model housed within [Microsoft Dataverse](https://docs.microsoft.com/en-us/powerapps/maker/model-driven-apps/model-driven-app-glossary#dataverse), you can't create a model-driven app.

Using the app designer with little or no code, you can build apps that are simple or very complex, connecting with a Microsoft Dataverse.

Check out this Codelab [Build your first model-driven app](https://docs.microsoft.com/en-us/powerapps/maker/model-driven-apps/build-first-model-driven-app)


## Power Automate
[Power Automate](./Power%20AutomateD%20(1).png)

Power Automate is an online workflow service that automates actions across the most common apps and services.

An automated process/task simply means streamlining a system by removing human inputs, which decreases errors, increases speed of delivery, boosts quality, minimizes costs, and simplifies the business process. 

You can use Power Automate to automate workflows between your favorite applications and services, sync files, get notifications, collect data, and much more.

A very good use of Power Automate will be to automate the task of sending a requisition to the Team lead or Head of your department in your office/organisation, which is to be carried out every Monday morning. 

With Power Automate, you simply create a flow to perform that task for you every morning, hence ensuring that task is performed always smoothly. 

Another good example will be to monitor what people are saying about your business by creating a flow that runs whenever someone sends a tweet with a certain hashtag. The flow can add details about each tweet to a Facebook post, a SQL Server database, a Microsoft Lists list, or even a Microsoft Excel file that's hosted on OneDrive for Business–-whichever service works for you.

*A flow communicates between your business applications so they can work with each other to eliminate the need for manual processes. A flow begins with a 'trigger', a pre-defined event that then triggers a response.*

To understand more about Power Automate and Power Automate flows, check out: [Overview of the different types of flows](https://docs.microsoft.com/en-us/power-automate/flow-types).

## Power BI
[Power BI](./Power%20BI.png)

Microsoft Power Business Intelligience (BI) is one of the most popular of the five Microsoft Power Platform Products. 

Power BI is a very great tool used for data analysis, collaboration and presentation. 

Power BI is a collection of software services, apps, and connectors that work together to turn your unrelated sources of data into coherent, visually immersive, and interactive insights. Your data may be an Excel spreadsheet, or a collection of cloud-based and on-premises hybrid data warehouses. 

Power BI lets you easily connect to your data sources, visualize and discover what's important, and share that with anyone or everyone you want.

The three (3) basic **Power BI** elements are: 
1. Power BI Desktop
2. Power BI Service
3. Power BI mobile apps. 

These three basic elements all work together with certain functionalities reserved for each of the elements. 

Power BI Desktop is a **Windows desktop application**. Power BI Service is an **online *Software as a Service*. Power BI mobile apps are basically apps for iOS and Android devices. 

More recently Power BI have evolved from just being a tool for viewing reports and dashboards, to a tool used to push data into datasets or embed dashboards and reports into your own custom applications. 

One common workflow in Power BI begins by connecting to data sources in Power BI Desktop and building a report. You then publish that report from Power BI Desktop to the Power BI service, and share it so business users in the Power BI service and on mobile devices can view and interact with the report.

To find out more on Power BI, check out [Power BI documentation](https://docs.microsoft.com/en-us/power-bi/). 

## Power Virtual Chat Agents
Power Virtual Agents is another amazing Power Platform Product which is used for building AI Powered ChatBots which can be used in custom websites, Applications, and some social media platforms (Facebook, Microsoft Teams, etc). 

Power Virtual Agents are adaptable Artificial Intelligence (AI) chatbots, at your service.

They can solve common customer and internal-facing issues automatically, freeing up staff to focus on complex requests and high-value interactions. 

You can easily create your own virtual agents, powerful chatbots, without the need for developers or data scientists, by using a guided, no-code graphical interface.

### Important Concepts of Power Virtual Agents###

When you create chatbots with Power Virtual Agents, you author and edit topics. 

Topics: Topics are discrete conversation paths that, when used together within a single chatbot, allow for users to have a conversation with a chatbot that feels natural and flows appropriately. 

In Power Virtual Agents, a topic defines how a chatbot conversation plays out. You can author topics by customizing provided templates, create new topics from scratch, or get suggestions from existing help sites.

Trigger phrases: These are phrases, keywords, or questions that a user is likely to type that is related to a specific issue—and conversation nodes—these are what you use to define how a chatbot should respond and what it should do.

The AI uses natural language understanding to parse what a customer actually types and find the most appropriate trigger phrase or node.

For example, a user might type "Open hours" into your chatbot, the AI will be able to match that to the Store hours topic and begin a conversation that asks which store the customer is interested in, and then display the hours the store is open.

Entities: An entity can be viewed as an information unit that represents a certain type of a real-world subject, like a phone number, zip code, city, or even a person's name.

Actions: An Action in Power Virtual Agents simply refers to the integration of a Microsoft Power Automate flow into a Chatbot to perform an action. 

Remember I stated it earlier that Microsoft Power Apps enables the creation of web and mobile applications that run on all devices, in this section of the article we will be looking at running a power app on a mobile device. 

To learn more about [Power Virtual Agents](https://docs.microsoft.com/en-us/learn/modules/introduction-power-virtual-agents/). 

## Power Pages
[Power Pages](./Power%20pages.png)

Power Pages, the latest member of the Power Platform family, was announced during Microsoft Build 2022. 

Microsoft Power Pages formerly known as Portals, is a new standalone product. 

As a new standalone Product, Power Pages is a secure, enterprise-grade, low-code software as a service (SaaS) platform, that empowers you to create, host, and administer modern external-facing business websites quickly and easily, that seamlessly work across web browsers and devices.

Extending beyond portals capabilities, Power Pages empowers anyone, regardless of their technical background, with an effective platform to create data-powered, modern, and secure websites.

With new and exciting features added to this new product, businesses can now have a modern and secure website, which is built on a low-code platform that is business-centric in nature.

### Features and capabilities available in Power Pages

1. The Design Studio: The Design Studio makes it easy to design, style, configure and publish modern business websites. Start from scratch or use one of the ready-to-use templates to design your site pages with text, video, images, business data forms and lists, and more.

2. The Templates Hub: The Templates Hub hosts full-featured websites with demo data, so you can jumpstart your journey to managing scheduling, registration, application submission, and more, with these amazing built templates.

3. Learn Hub: With the Learn Hub, you can explore guides, tutorials, and quick videos to learn how to build websites, model and visualize business data, work with code components, and of course, configure sites. This will help you get started if you are just about building your first website or not quite familiar with building websites using a low-code tool.

Another amazing reason to try out Power Pages is that Power Pages runs on Microsoft Azure and connects with Dataverse to provide critical security capabilities that include advanced encryption, rich role-based access controls (RBAC), and support for Microsoft Azure Front Door and other web application firewalls. Microsoft Azure DDoS Protection addresses top web security vulnerabilities.

Also, Visual Studio Code is integrated into Power Pages, using Visual Studio Code in Power Pages, professional developers can code advanced capabilities using JavaScript, Liquid templates, code components, and web APIs. With these tools, you build and can securely interact with underlying business data and implement custom business logic, all without leaving the surface of your favorite developer tools.

Microsoft Power Platform command line interface also helps developers easily download and upload their customized projects.

To find out more about Microsoft Power Pages, please visit the [Power Pages Preview documentation] (https://docs.microsoft.com/power-pages/) 

In conclusion, we understood that Microsoft Power Platform Products are a set of Low-Code/No-Code Products, we also talked about the various Power Platform products, looking at their feautres, capabilities and features. 

Feel free to try out building amazing products with these tools. 

Lastly always visit the official Power Platform documentation to find out more about these products: [Microsoft Power Platform documentation](https://docs.microsoft.com/en-us/power-platform/).
