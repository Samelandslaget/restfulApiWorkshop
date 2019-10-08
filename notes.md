# RESTful APIs
Workshop at DevConf 2019
Teacher: Spencer Schneidenbach
Date: 2019-09-25

## Intro
This workshop will teach you Spener's opinions.


## Intro to ASP.NET Core
- Totally modular
- Seamless transition from on-premises to cloud
- Open Source with contributors
- Choose your Editors and Tools
- Cross-Platform
- Faster framework

### Hosting
Flexible

### Middleware
Layers of functionality
Example
- GET request
- Security layer
- Etc.

### Configuration
We're using JSON files.


## RESTful APIs built in ASP.NET Core
Well documented?
Query string parameter behavior well defined?
Uptime issues?

Simple != Easy
It's not necessarily easy for developers to make an API that's easy to use.

There is no spec on REST APIs. There are no rules, only opinions.

### Six constraints of REST
- Client-Server
- Cacheable
- Stateless
	- All info is in the request. Nothing on the server
- Layered
- Code on Demand (optional)
	- Example: JacaScript
- Uniform Interface
	- Self-descriptive

### Pragmatic REST
RESTful API != Good API

### API Design process
- Design
- Implement
- Document
- Maitain

### Rules
1. KISS
1. Be consistent


## CQRS
Command Query Responsibilty Segregation

### Scaffolding
Scaffolding is a lie! Avoid scaffolding!

### Controller should only
- Route the request
- Return data

### Move these elsewhere
- Separate entity from request
- Invoke the services required to validate and run the command
- Validate
- Run service for request

### Advantages
- Reusability
- Testability
- Separation of concerns
- Ease of development

### Misc.
- Separate request and entity

### FluentValidation
A NuGet package
Good shit. Understandable code

### MedaitR

### AutoMapper
Super handy tool.


## Understanding verbs

### GET Requests
- Idempotent
- Empty request body

### Resource identification
Nouns vs. verbs: use plural nouns

### Page
When working with large data sets, consider paging.
Remember to validate page parameters (pageNumber, pageSize, etc.)


## Testing your API

### Testing methods
- Microsoft.AspNetCore.TestHost library
- Mocks (not covered in this workshop)

### TestHost


## POST, PUT, PATCH Overview

### Error reporting
Erros will happen. How will you handle them?

Again: Use a validator as you see fit.


## Versioning

### Change Management
Change management is hard.

### Deprecation


## Security

### Authentication / Authorization
A lot of documentation exists online


## Swagger
Really cool, but not perfect.


## Sub-resources


## General notes
Spencer has a talk


## Questions
Q: Route request?
A: It basically means: What controller method does this request map to?