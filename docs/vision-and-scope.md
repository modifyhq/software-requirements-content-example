---
id: vision-and-scope
title: Vision and scope
description: Business requirements grouped into a single deliverable; used as basis for subsequent development work.
---

<InfoMessage header="Alternative names" content="Marketing requirements document (MRD)">

This adapts a template by Karl Wiegers. You can find a preview at: https://www.processimpact.com/process_assets/vs_preview.pdf. 

## Background

- We started Modify to solve our problems creating and managing documentation for an ISO 27001-compliant security programme.
- We had requirements for version control (both docs and tabular data), reviews, traceability from requirements to controls, and rendering to multiple formats (html, pdf, docx, xlsx), to name a few.
- Many of our prefered tools and workflows e.g. markdown/MDX for writing, Git for version control, static site generators for html, happened to be a good fit. 
- If we could wrap these up into a web app, that could also support team collaboration, we thought we might be onto something. And so Modify was born...

## Problem/Solution

- Most publishing workflows do not support the tools software teams know and love, namely plain text markup (e.g. markdown and MDX), Git, and popular build tools (e.g. NexktJS, Gatsby) and hosting services (e.g. Netlify, AWS S3). 
- Modify aims to solve this by providing a tool that does (see [website](https://modifyhq.com/#/)). 

## Opportunity 

- There are an estimated 23m developers globally, many of whom work in teams that produce, or want to produce, content
- There are many incumbent tools, but few that target the needs of software teams per se, and practically none that properly supports popular technologies like markdown/MDX, Git, static site generators and React-based frameworks. 

## Objectives

*Product-market fit (PMF)*:

- 40% of users surveyed answering "Very Disappointed" to the question "How would you feel if you could no longer use Modify?". 
- See [full survey](https://coda.io/@rahulvohra/superhuman-product-market-fit-engine/set-up-your-survey-31) for details.

*Beyond PMF*:

- Net promoter score (NPS) of XX (XX months after beta launch)
- Week-on-week user growth of XX% once in GA

## Vision statement

- **For** software development teams
- **Who** need to document their work for internal and external audiences
- **The** Modify service
- **Is** a web app
- **That** helps teams collaborate with plain text (markdown, MDX and yaml) and Git (GitHub and Bitbucket), configure graphical and text views that work for them, and run render and publish jobs using Docker containers
- **Unlike** other apps for creating and managing docs
- **Our product** targets the needs of software teams using their preferred technologies and workflows, and gives them control of key parts of the workflow.

## Features

See [features-register]

## High-level use cases

- User docs
- Blogs
- Architecture 
- Software requirements
- Security 
- Medical device compliance 
- Policies and procedures

## Users 

Members of software teams including:

- CTOs
- Architects
- Tech leads
- Software developers 
- Business analysts 
- Product owners
- Quality assurance engineers
- Technical writers
- Compliance managers
- Security engineers 

Check out our [personas] for more detail. 

## Releases

- **Prototype** - Text editor, markdown docs, GitHub connector, relationships, workspace branching, reviews. 
- **MVP** - All listed features.
- **Further iterations** - Improvements and new features, as determined by user feedback. 

## Deployment

Modify services will be deployed as Docker containers on AWS's EKS managed kubernetes (k8s) service. 

AWS cloud infrastructure will be provisioned using [Palumi](https://www.pulumi.com/) scripts, k8s infrastructure using [Helm](https://helm.sh/) charts.
