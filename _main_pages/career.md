---
layout: default
emoji: 💼
title: Career
description: TODO
nav_order: 3
---

🚧 Under Construction

{%- comment -%}

# Wonderschool

**Senior Software Engineer** (April 2024 – Present)

## Core Entities (September 2024 – Present)

This work was attached to the Unified Parent Experience (UPE) project. The purpose was to unify two different applications (one built with Elixir/LiveView/Phoenix and the other with React/Firebase) that used two different data sources (Postgres DB and Firestore DB respectively).

### Technologies

- TypeScript
- NestJS
- Postgres
- Firestore/Firebase
- Elixir
- Phoenix
- LiveVIew

### Contributions

- Heavily involved in early planning meetings
- Led discussions for foundational architecture design
- Designed a phased migration approach:
  - Introduced an API layer between the front-end and Firestore to forward reads and writes
  - Implemented schema validation for API writes while updating client code to respect schemas
  - Created corresponding Postgres schemas for each resource
  - Implemented dual-writing to both databases while continuing to read from Firestore
  - Conducted backfills for completed resources
  - Switched reads to Postgres once resources were fully migrated
- Executed the plan with a team of 5 other engineers
- Led discussions and investigations for migrating Firestore data to Postgres

### Challenges

- Worked with a predetermined deadline based on business operational requirements
- Had to adapt the migration approach when the original plan proved less successful than anticipated
- Navigated the complexities of dual database systems while maintaining system functionality

### Results

- Migrating Firestore data to Postgres improved data quality which in turn enabled the engineering team to understand the data schema better and that enabled us to design, plan, and implement features faster
- Waiting to find out

## Kong API Gateway (August 2024\)

Set up Kong API Gateway in our Kubernetes cluster. Learned basic Lua to implement custom plugins for JWT verification.

### Technologies

- Kubernetes (External DNS,
- Kong
- Lua

### Contributions

### Challenges

### Results

## Network Admin (May 2024 – July 2024\)

This was a project for the Florida Department of Education to create a software solution for managing school listings. The system supported multiple user roles (network owner, network admin, school staff) with varying permissions and access levels.

### Technologies

- TypeScript
- Postgres
- NestJS
- Elixir
- Phoenix
- LiveView

### Contributions

- Designed, developed, and delegated tasks to build the back-end API to power the Network Admin
- Implemented CRUD endpoints for users and their roles with appropriate authorization guards
- Created endpoints to invite network users with automatic email notifications
- Developed endpoints to manage a given network user's module access (users, listings, analytics)
- Implemented functionality to manage user's listing access
- Consolidated divergent code into a shared SSO SDK that could be used in any React app
- Led discussions for data modeling and integration between teams working in different tech stacks

### Challenges

- Managed tight timeline pressure when deadline was moved up by a month due to governor's request
- Successfully integrated application UI and routing (developed in Elixir/Phoenix/LiveView) with API developed in TypeScript/NestJS as mandated by management

### Results

- Successfully secured a $1M+ contract with the Florida Department of Education
- Created a system that manages 24,000 schools through 18,000 users
- Developed features that positioned the company for similar contracts with other government entities
- Delivered the project successfully despite a compressed timeline

# Divvy Homes

**Senior Software Engineer** (April 2019 – September 2023\)

## Flexible Savings

Flexible Savings was a major initiative to increase the total addressable market for Divvy’s top of funnel. The original product was limited to a few options (2% down, build to 10% equity and 1% down, build to 5% equity). The Flexible Savings project allowed customers to adjust their equity savings target on a monthly basis. A customer would start with 2% down and then have two options: 1\) choose an equity savings target (e.g., 7%) and the app would calculate their monthly contribution or 2\) choose what monthly contribution they wanted and the app would calculate their total equity savings at the end of the lease.

### Technologies

- JavaScript/TypeScript
- React
- Postgres

### Contributions

- Led the design, planning, and implementation across 3 teams (underwriting, operations, and capital) for the project
- Contributed to increasing the total addressable market by making the product more flexible
- Transformed the original model (where monthly payments contributed to 10% home equity for down payment) into a more customizable solution

### Challenges

- Large surface area and I had to dive into code and areas of the business that I hadn’t previously

### Results

- Resulted in a 30% increase in approved applicants by making the product more accessible
- Doubled the total addressable market from 5.2M to 10.3M

## Automated Underwriting

An extension of the FastTrack project to fully automate as many underwriting applications as possible. It was the natural evolution of the FastTrack project and we used data from FastTrack to come up with heuristics for which applications could be automatically underwritten.

Worked with 1 other engineer and 1 PM.

### Technologies

- TypeScript
- PostgreSQL
- RabbitMQ
- Async Webhooks

### Contributions

- Designed, planned, and implemented integrations with The Work Number for instant income verification, EmpInfo for asynchronous income verification, Experian for nearly instant credit verification, and Arcgate for asynchronous transcription for documents like photo ID, bank statements, and tax documents
- Maintained the underwriting system while collaborating with stakeholders (underwriters and project managers)

### Challenges

- Had to make it work with unstructured and schema-less data in JSONB columns
- High pressure to deliver automation by a deadline determined upcoming real estate season

### Results

- Improved underwriting speed by automating credit, income, and identity verification processes
- Enabled instant underwriting in \~20% of applications
- Automated \~60% of applications which effectively doubled in inbound funnel

## First Republic and Spruce Integration

Integrated Divvy systems with First Republic bank to automate wire transfers based on settlement statements provided by an integration with Spruce, a closing/title company that operates in markets across the nation.

Started with 1 other engineer, 1 PM, 1 designer. After layoffs I was the single engineer. EM jumped in to help.

### Technologies

- SFTP–S3 bucket synchronization
- JavaScript
- PostgreSQL
- Async Webhooks from Spruce
- Arcane SFTP–S3–XML-based integration with First Republic

### Contributions

- Designed, planned, and implemented the integrations with each of the third parties
- Collaborated directly with the product manager and closing partners to understand and align on the problems we were solving, establish a solution, and agree on a roadmap for implementation

### Challenges

- Layoffs mid-project had to take on most of the project myself and then onboard my manager to help deliver on time

### Results

- Automated \~70% of home closing wire transfers which improved home closing rates and reduced time to close which helped secure deals

## FastTrack

Developed an internal underwriting tool with the goal of enabling 1-click approvals. Prior to this tool underwriters used an older tool that enabled their existing manual workflow which included verifying their credit score and credit report line items, verifying income by inspecting income documents, and verifying their identity by inspecting the uploaded identity documents. FastTrack automated each of those workflows and provided underwriters a high-level view of each application and the option to 1-click approve or dive deeper with the manual workflow underwriting tool.

Worked with 2 other engineers, 1 PM, and 1 designer.

### Technologies

- JavaScript
- Heroku
- PostgreSQL
- RabbitMQ
- Async Webhooks

### Contributions

- Collaborated directly with the product manager and underwriting partners to understand and align on the problems we were solving, establish a solution, and agree on a roadmap for implementation
- Worked with the lead engineer of the project on the technical design
- Provided feedback and iterated with the PM and underwriting stakeholders on UI and UX elements to ensure a consistent and enjoyable experience

### Challenges

We didn’t have a dedicated designer so eng and product had to iterate extensively with underwriting stakeholders and settle disagreements. It inflated the project timeline and although we eventually arrived at a consensus it took a lot of iteration.

The lead engineer adopted an unconventional programming paradigm that used JavaScript higher-order functions to do dependency inversion/it led to confusing code that wasn’t idiomatic to JavaScript

### Results

- Increased application throughput by \~30% which resulted in a \~50% increase in conversion; faster approvals kept users engaged meaning even if the throughput stayed the same we would have seen an increase in conversion
- Underwriters were happy to have a more streamlined tool and less stressed with their jobs because of the decreased load and easier workflow

{%- endcomment -%}
