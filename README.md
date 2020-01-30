# ASP.NET Core - App Building Workshop

[![Build Status](https://dev.azure.com/dotnet/AspNetCoreWorkshop/_apis/build/status/ASP.NET%20Workshop-ASP.NET%20Core%203.x?branchName=master)](https://dev.azure.com/dotnet/AspNetCoreWorkshop/_build/latest?definitionId=71&branchName=master)

[BackEnd Web API](https://aspnetcorews-backend.azurewebsites.net) | [FrontEnd Web App](https://aspnetcorews-frontend.azurewebsites.net)

## Setup

You can perform the exercises using [Visual Studio 2019](https://visualstudio.microsoft.com/downloads/), or the [.NET Core CLI and SDK](https://dotnet.microsoft.com/download/dotnet-core/3.0) from the command line.

> | **NOTE:** |
> | - |
> | *If you are installing Visual Studio, you only need to select the `ASP.NET and web development` workload.* |

If you have issues downloading the installers, we may have USB sticks with offline installers for you to use.

## What you'll build

In this workshop, you'll learn by building a full-featured ASP.NET Core application from scratch. The application displays information about conference sessions and speakers. The application enables users to register, and create their own conference agend based on the sessions they would like to attend. Users with administrative rights can also edit the details of conference sessions.

In Session 1, you'll start with a back-end application that exposes a web API for accessing and maintaining conference data. You'll store the conference information in a database, and the backend will use an Entity Framework model to retrieve and manage the data.

In Session 2, you'll extend the entity model and create Data Transfer Obects (DTOs) that the application can use to send and receive data.

In Session 3, you'll create a front-end web application that enables users browse sessions and speakers. This application will use the DTOs created in session 2 to package data when communicating with the backend web API.

In Session 4, you'll add security by implementing authentication and authorization. You'll also implement an administrative policy, that enables specific users to modify the details of sessions.

In Session 5, you'll enable logged in users to select sessions and create their own personalized conference agenda.

In Session 6, you'll also learn how to deploy the backend and frontend applications to a production environment. The session presents several different deployment scenarios, including deployment to Azure, and deployment as Docker containers.

Session 7 presents additional challenges that you can tackle if you have time.

Session 8 shows how to create a Single Page Application (SPA) that acts as an alternative front-end.

### Application Architecture

The diagram below highlights the components you'll create in this workshop, and the technologies used.

![Architecture Diagram](/docs/images/ConferencePlannerArchitectureDiagram.svg)

### Database Schema

You'll store the data in a SQL Server database. The following diagram shows the tables that the application will create.

**NOTE TO SELF: MAY NEED TO REGENERATE THIS DIAGRAM IF IT IS NOT UP TO DATE**

![Database Schema Diagram](/docs/conference-planner-db-diagram.png)

## Sessions

The table below provides links to the exercises for each session.

| Session | Topics |
| ----- | ---- |
| [Session #1](/docs/1.%20Create%20BackEnd%20API%20project.md) | Build the back-end web API with a basic Entity Framework model |
| [Session #2](/docs/2.%20Build%20out%20BackEnd%20and%20Refactor.md) | Extend the Entity Framework model. Add DTOs to the back-end web API, and refactor the model classes into view models |
| [Session #3](/docs/3.%20Add%20front-end%2C%20render%20agenda%2C%20set%20up%20front-end%20models.md) | Create an ASP.NET front-end web application, display session and speaker information, andc create front-end models |
| [Session #4](/docs/4.%20Add%20auth%20features.md) | Add authentication to the front-end web application. Implement an administrator policy that enables specific users to edit sessions information. Define and use a custom auth tag helper |
| [Session #5](/docs/5.%20Add%20personal%20agenda.md) | Enable users to register for a conference and create their own personal agenda |
| [Session #6](docs/6.%20Production%20Readiness%20and%20Deployment.md) | Configure health diagnostics for the back-end web API and the front-end web application. Deploy the back-end and front-end components to a rpoduction environment. |
| [Session #7](/docs/7.%20Challenges.md) | Add support for external authentication (Google or Twitter). Add a third-party logger to the front-end web application. Provide support for image uploading, editing, and display. Implement caching in the front-end web application. Modify the back-end to store data in MySQL or PostgreSQL. Write unit and functional tests. Add further features to the front-end and back-end applications.
| [Session #8](/docs/8.%20SPA%20FrontEnd.md) | Create a SPA front-end web application. |
