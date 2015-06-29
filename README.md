# MedAlerts Pool II Prototype Application

Check out the [live demo](http://medalerts-dev.sparcedge.com/).

[SPARC](http://sparcedge.com) evaluated the [FDA's](http://www.fda.gov/) role, mission, and goals to build a prototype that empowers consumers to research medications for recalls, label changes and general medication updates.

## Understand What People Need

SPARC reviewed [OpenFDA’s](https://open.fda.gov/) business goals, technical feasibility, and prototype time constraints. Research revealed that adverse medication side effects impact the population with [106,000 yearly deaths at an estimated cost of $135 billion per year](http://www.fda.gov/Drugs/DevelopmentApprovalProcess/DevelopmentResources/DrugInteractionsLabeling/ucm110632.htm); therefore, we chose drug safety as the prototype focus.

## Address the Whole Experience from Start to Finish

SPARC implemented an agile approach, allowing us to iterate on the broad concept of drug safety and focus in on what would have the highest value for the user.

The user can:

* Access the experience from a desktop or mobile browser
* See medication recalls and the impact of drug changes
* Search for medication and create a personalized list of medications 
* ‘Follow’ their medications and automatically receive update feeds, much like other social media applications

## Make it Simple and Intuitive

Rapid prototyping and feedback helped us quickly test our assumptions and revealed that “following” a medication was the user’s preferred experience.  Allowing the user to receive medication updates via feeds reduced the prototype’s user-flow to a single screen. 

SPARC created features based on an agile process model: 

User & Technical Research

* Define business goals 
* Understand OpenFDA API
* Understand the User 
* Conduct brainstorming sessions to choose valued features based on business goals, technical feasibility, and usefulness to the User
* Refine concept

Iterative Prototyping 

* Create initial prototype infrastructure
* Consume one API endpoint and display data in JSON format
* Search within returned data
* Store a list of medications
* Search across all medications and display results 

## Build the Service Using Agile and Iterative Practices

SPARC’s Agile and Iterative practices included:

* One-day sprints 
* Daily stand-ups and retrospectives
* Dedicated 'war room' for team collaboration 
* GitHub for source code version control and sharing
* Setup [Shippable](https://app.shippable.com/) for continuous integration and deployment to our development environment

## Structure Budgets and Contracts to Support Delivery

SPARC executed with repeatable program management and performance-focused processes, using [Google Sheets](https://www.google.com/sheets/about/) for level of effort monitoring and daily milestone activities.

## Assign One Leader and Hold That Person Accountable

SPARC assigned one Product Owner for leadership and accountability. 

## Bring in Experienced Teams

SPARC assembled an experienced, multi-disciplinary team to develop the prototype. This team included a mix of four labor categories; see Attachment C.

## Chose a Modern Technology Stack

Every layer of the stack leverages Open Source Software solutions:

**Development Layer**

* [Play Framework](https://www.playframework.com/)
* [Scala](http://www.scala-lang.org/)
* [AngularJS](https://angularjs.org/)
* [lodash](https://lodash.com/)

**QA Layer**

* [Scala Test](http://scalatest.org/)
* [Jasmine](http://jasmine.github.io/)
* [Karma](http://karma-runner.github.io/0.12/index.html)

**DevOps Layer**

* [Docker](https://www.docker.com/)
* [GulpJS](http://gulpjs.com/)

SPARC provided installation instructions for [Yosemite](https://en.wikipedia.org/wiki/OS_X_Yosemite) and [Debian](https://www.debian.org/) based systems and have deployed to [Amazon Web Services](http://aws.amazon.com/), [Vagrant](https://www.vagrantup.com/), Yosemite, and [Ubuntu Vivid](http://releases.ubuntu.com/15.04/) images.

## Deploy in a Flexible Hosting Environment

SPARC deployed to Amazon Web Services (AWS) for a flexible infrastructure to ensure real-time resources provisioning via APIs.

This prototype uses Elastic Beanstalk in one region with subnets in multiple availability zones. [AWS CloudFront](http://aws.amazon.com/cloudfront/) is our content delivery network (CDN) serving static application resources from [S3](http://aws.amazon.com/s3/).

## Automate Testing and Deployments

Each day (sprint) ended with a production-ready deliverable. SPARC implemented functional unit and integration testing, as well as security, performance, usability, and accessibility testing. We conducted automated testing using Scala Test for Scala, Jasmine for javascript, and Karma for AngularJS.

We used GulpJS to create an automated, streaming build system. 

We used Docker to automate the maintenance of deployments.  

We used Shippable to automate the entire CI&D process and push to production, leveraging it’s integration with Docker.

## Manage Security and Privacy Through Reusable Processes

The prototype uses a deployment script and environment variables to ensure production environment configuration remains consistent and controllable.

SPARC [installation instructions](INSTALLATION.md) detail the steps to install and run this prototype on another machine and include scripts to automate the process.

The production application environment sits inside a Virtual Private Cloud within AWS. Security groups and network Access Control Lists provide security and accessibility at the instance level and subnet level.

## Use Data to Drive Decisions

SPARC used [New Relic](http://newrelic.com/) for application monitoring and operational decisions.  We leveraged data from real-time metrics such as resource utilization and application performance.  We created automated alerts, tracked concurrent users, and monitored user and application behaviors.

## Default to Open

There is an [email contact](mailto:18f@sparcedge.com) link so users can report bugs and issues.

SPARC created an API layer to interact with and aggregate openFDA results and demonstrate OAuth2 competency.

We open sourced all prototype code via GitHub under the [MIT License](LICENSE.md) and published our approach to development via this file.
