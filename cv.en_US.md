# Bruce Tsai - *Software Architect*

![photo](https://github.com/nanashi07/cv/blob/master/bruce.jpg)

## Summary

Familiar to design and develop software system, analysis and performance tuning, improve development process efficiency and producing quality. Understand performance issue and maintainability of development, having ability to integrate with developing system and various solution, and be able to work independently or leading members to achieve goals.

Major use Java and C#, and use Python / node.js / go, etc. as assistance. Familiar to web based systems, experienced with frameworks like Angular, Vue, Polymer, jQuery and so on. Familiar to SQL Server, Oracle and substitute of MySQL database.

Beside programming, familiar to linux system and solutions such as nginx, ELK, SonarQube, docker, Kubernetes and experienced with cloud service of GCP and Azure.

Love learning technology, have a habit of reading technology articles every day, and survey in-depth for things I interested in. Doing my owned side project at leisure time, and push completed projects to Github.


## Work experience

### Principal engineer @*OpenNet*

> Jul 2019 - NOW

#### Games
- Migrate RabbitMQ to RocketMQ for Sporty Soccer
- Kickoff Sporty-Fantasy
  - System planning and architecture design
  - Multi-countries, multi-users contest game
  - Communicate and integrate with third-party API
  - 80% of total code implementation
#### Sporty.com
- Kickoff Sporty.com
  - System planning and architecture design, totally 7 modules
  - As a sports media app, include news, video, chat, share and social
  - Communicate and integrate with third-party API
  - 75% of total code implementation
#### SportyBet
- Feature implementation
  - Fixed issue of third-party library, hacked library for system requirement
  - Configured and implemented Redis R/W access, balanced loading in production. Migrated high loaded Redis to cluster mode
  - Implemented tax logic, included withholding tax and excise tax
  - Optimized MTS process with multi-thread, integrated with sync-async conversion in order flow
  - Implemented KYC, ensure user experience in deposit/withdraw and avoid fraud from users
  - Implemented DoB promotion, provided trusted info for KYC
  - Implemented finance flow, append new mechanism of deposit in core logic flow (PAC Account)
  - Implemented supporter feature, allowed verified user to transfer money to another user (P2P transfer)
  - Designed and implemented log analysis service for mobile devices
  - Design and integrated all modules to CMS
  - Fix bug and vulnerabilities from SonarQube
- Performance
  - Solved and optimized performance issue on huge amount of settlement messages at the same time
  - Optimized settlement flow, decreased load of database, decreased unnecessary/duplicated computing
  - SQL performance tuning for all modules, based on the monitor from DBA
  - Optimized message push service, decreased push delay and increased scalability of service
  - Optimized memory cache usage, created metrics for caches for performance tuning
  - Enhanced Jaeger APM, provided more info in tracing performance issue
  - Added various metrics, made system status and abnormal clearly. Fix issues before damage encountered
  - Solved cache issue caused full GC, tuning JVM arguments and migrate parallel GC to G1 GC
  - Measured and analysis performance of order, made the metrics more clear and do improvement depend on it
  - Analysis API performance of sms module, improved incorrect collection usage and solve parallel issue.
  - Analysis OOM, high CPU, network issue and improve
  - Improve test performance, include code performance and environment performance (mysql)
- Architecture
  - Help database migration, from cetus to AWS RDS, rewrite and optimized part of queries
  - Split payment module into user endpoint and third-party endpoint, prevent affected each other
  - Help new country environment deployment, troubleshooting relevant issues
  - Upgrade modules from Spring Boot 1.6 to 2.3
  - Optimized resource configuration in Kubernetes, analysis issues on running
  - Log system integration solution (cloudwatch, rsyslog, kafka, loki)
  - Rebuilt load test solution, with gatling and argo workflow
  - Continuously code refactor
  - Optimized maven dependency for all modules
  - Split order module, avoid traffic and transaction from different caused loading issue
  - Plan and participate TiDB, SQL Proxy, Sharding JDBC migration
#### SportyBet - International
- Design and implemented email based registration, multiple countries, multiple languages, multiple currency supported
- Design and implemented dynamic, flexible KYC
#### Other
- Production issue trace, find issue at the first place and fix immediately before user affected
- Production outage handling
- Introduced solutions, such as SonarQube, Webflux, gRPC, drone, KEDA, arog workflow, gatling
#### Management
- Principal engineer since 2021/01
- Backend team leader since 2021/05
- Lead Stability & Security team, ensure production robust and stable. Traffic at the end of 2021 increased to 4x from earlier of 2021
- Backend team management

##### Tags

`SportyBet` `Fantasy` `Sporty.com` | `Java`, `Spring Boot`, `MySQL`, `Cetus`, `RocketMQ`, `RabbitMQ`, `Reids`, `ElasticSearch`, `Kubernetes`, `AWS`, `drone`, `gRPC`, `Reactive`, `Jaeger(opentracing)`, `Prometheus`

------------------------------------------------------------------------

### Engineer @*Silkrode  Technologies Co., Ltd.*

> Oct 2018 - Jul 2019

- Be backend contact, coordinate with each team.
- Define API specifications.
- Build Gitlab and ensure availability.
- Build required foundation structure and develop core system using .net core.
- Evaluate and plan architecture of production on GPC, Azure cloud
- Build production with Kubernetes(GKE), helm and other related solutions
- Verification of technical solution, includes:
  * Performance of the logging library (Nlog / Serilog / Log4net)
  * Redis client / server solution (StackExchange / ServiceStack / CsRedis / Cluster / Sentinel / Codis)
  * Performance of JSON serialization  (Newtonsoft / Jil / Utf8Json)
  * Availability and performance of MySQL (MGR) and its alternatives (Galera/XtraDB) on cloud services.
  * Asynchronized process performance. (Queue / HangFire / Polly)
- Intranet environment planning and construction.
- Management of cloud environment.
- CI/CD planning and implementation
- Sharing and technical training

##### Tags

`Trade` `Profit` | `C#` `.Net Core` `Percona` `Docker` `Kubernetes` `Redis` `RabbitMQ` `CentOS` `Gitlab-CI` `SonarQube` `Graylog` `ELK` `MongoDB` `GCP` `Azure` `Architect` `Helm` `HAProxy`

------------------------------------------------------------------------

### Leader of Engineers @*Dingok*

> Feb 2018 - Oct 2018

- Plan and architect deployment on azure.
- Introduce CI/CD using gitlab, define and simplify develop flow.
- Introduce code analysis using SonarQube and ensure code quality.
- Introduce Protobuf for serialization between platforms
- Reconstruct monolithic system structure with 4-layer/3-tier design.
- Introduce .NET Core 2.0 for new feature development.
- Ask team members providing automatic unit/integration test, reduce test costs and improve system quality.
- Complete a POC of seat allocation service in one month, with high loading, capability, availability and scalability.
- Introduce docker container service to simplify development environment and deployment.
- Introduce ELK log analysis for monitor and behavior analytics.
- Replace outsourced allocate system with self-designed service, claim refund of paid fees.
- Introduce Kubernetes for container deployment and managements.
- Plan and manage for team jobs, technical trainings

##### Tags

`Dingok` | `C#` `.NET Framework` `.Net Core` `WPF` `SQL Server` `Azure` `Docker` `RabbitMQ` `Redis` `CentOS` `Ubuntu` `Gitlab` `git` `SonarQube` `ELK` `CI` `CD` `Protobuf` `System Architect Design` `k8s`

##### Links

* https://dingok.com

------------------------------------------------------------------------

### Engineer @*President Information Corporation*

> Jun 2017 - Dec 2017

- Develop a submodule of vendor collaborative management system (VCMS). 
- Upgrade Vendor2G from .net 1.1 with crystal report.
- Refactoring usage of source control and create guideline for develop flow.
- Provide CI/Jenkins solution to build and archive binaries.

##### Tags

`VCMS` `Vendor2G` `SISO` | `.NET Web form` `SQL Server` `jQuery` `Jenkins` `SVN`

##### Links

* https://7-11vcms.pcsc.com.tw

------------------------------------------------------------------------

### Senior Technical Consultant @*HY-Tech*

> Dec 2014 - May 2017

- Construct architecture for new or exists project, integration with multiple system and data exchange.
- Performance tuning and optimize resource usage strategy.
- Simplify developing flow, such as reduce repetitive code snippets and automate repetitive tasks.
- Improve and keep high quality such as provide develop guide, use static code analysis and code review.
- Research and provide solution for project and pre-sales.
- Develop and provide foundation component like AOP or code generator.
- Manage project schedule and task assignment, lead members to reach goal.
- Provide training of project related skills for newbie and team members.
- Communicate with customers and earn the trust and recognition.

##### Tags

`Fetnet eService` `Fetnet Code trace` `NEC Cosmed` `Arcoa NDRS` `Arcoa EIP` `Kingdu` | `Spring MVC` `Struts` `.NET MVC` `Hibernate` `MyBatis` `Entity Framework` `Dapper` `ADO` `Oracle` `SQL Server` `MySQL` `angular.js` `Vue` `jQuery` `weblogic` `IIS` `CentOS` `RHEL`

##### Links

* http://ecare.fetnet.net/eServiceV3/
* http://ndrs.arcoa.com.tw/NDRS

------------------------------------------------------------------------

### Senior Software Engineer @*Trend Micro*

> Nov 2012 - Oct 2014

- Customize Umbraco CMS, design function of supplier or distributors access control
- Develop, maintain and manage project systems based on Microsoft office sharepoint
- Supply technical support for other teams

##### Tags

`ishare` `ishare 2.0` `ishare 3.0` `Legal Contract Management system` `Calendar Synchronization` `BIF - Report information frontend` `APAC Sales Kick-off` `Quarterly IS Awards` `The circle` `Olympic 25th` | `Sharepoint` `C#` `jQuery` `Android`

------------------------------------------------------------------------

### MIS Deputy Supervisor @*GrandTech Systems Ltd*

> Feb 2012 - Oct 2012

- Develop AI (Ability International) order system based on web application and migrate old one from lotus notes
- Develop CRM, attendance, repair service, customer service for departments of AI
- Maintain EIP of GrandTech and AI
- Network and servers maintenance
- MIS supporting of GI (GrandTech Information) and  TI (TopTeam Information)
- Develop and maintain ETL and reports from SAP and EIP, performance tuning for execution.
- Routine jobs and maintenance of SAP
- Source control reconstruction
- Daily jobs of MIS department

------------------------------------------------------------------------

### Senior Engineer @*CHAUN-CHOUNG TECHNOLOGY CORP.*

> May 2010 - Feb 2012

- Develop MES for manufacture flow
- Develop workflow for departments using GP
- Support and maintain Tiptop
- Maintenance of web portal
- Develop functional feature for departments
- Support general application process of RD
- Support network and hardware maintenance

------------------------------------------------------------------------

### Engineer @*Chunghwa Telecom (MyEgov & GSP Operation Center)*

> Jul 2008 - May 2010

- Develop and maintain eGov portal
- Develop and maintain eGov modules and services
- Develop and maintain data exchange interface and function
- Customize Worksite MP as KMS

------------------------------------------------------------------------

### Engineer @*GENESIS INFORMATION INC.*

> Feb 2007 - Jun 2008

- Maintenance customer's system. Develop online shopping site and enterprise portal.
- Mainly use JSP/Servlet, and MySQL, SQL Server database

## Education

### Chinese Culture University

> 1998 - 2004

Both of Information Management and Japanese Language and Literature


## Skills

### Language

`Chinese`, `English`, `Japanese`

### Programming Language

`Java` `C#` `.Net Framework` `.Net Core` `Javascript` `Kotlin` `Python` `node.js` `Go`

### Front End

`jQuery` `Angular` `Vue` `Polymer`

### OS

`Windows` `CentOS` `Ubuntu` `MacOS`

### Database

`SQL Server` `Oracle` `MySQL` `MariaDB` `PostgreSQL` `Mongodb` `PouchDB` `Couchbase` `Redis` `Cetus`

### Message Queue

`RabbitMQ` `Kafka` `RocketMQ`

### SCM 

`Git` `SVN` `Team Foundation Server`

### DevOps

`Jenkins` `TeamCity` `Gitlab-CI` `Consul` `Kubernetes` `Istio` `Argo workflow`

### Virtualization

`Virtualbox` `Hyper-V` `Docker` `KVM`

### Mobile 

`Android (Native)`

### Design 

`Software architect` `System design document` `System analysis`

### Management

`Communication for customers and members` `Skill training for team members` `Project tasks management`

## Personal Links

* Blog: https://nanashi07.blogspot.tw/
* Github: https://github.com/prhythm, https://github.com/nanashi07
* Web components: https://www.webcomponents.org/author/Prhythm
* Chrome extensions: https://goo.gl/J62Khh
