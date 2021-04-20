# Bruce Tsai - *Software Architect*

![photo](https://github.com/nanashi07/cv/blob/master/bruce.jpg)

## Summary

Familiar to design and develop software system, analysis and performance tuning, improve development process efficiency and producing quality. Understand performance issue and maintainability of development, having ability to integrate with developing system and various solution, and be able to work independently or leading members to achieve goals.

Major use Java and C#, and use Python / node.js / go, etc. as assistance. Familiar to web based systems, experienced with frameworks like Angular, Vue, Polymer, jQuery and so on. Familiar to SQL Server, Oracle and substitute of MySQL database.

Beside programming, familiar to linux system and solutions such as nginx, ELK, SonarQube, docker, Kubernetes and experienced with cloud service of GCP and Azure.

Love learning technology, have a habit of reading technology articles every day, and survey in-depth for things I interested in. Doing my owned side project at leisure time, and push completed projects to Github.


## Work experience

### Principal @*OpenNet*

> Jul 2019 - NOW

- Fix issue of third-party library, add and modify library for system requirement
- Migrate RabbitMQ to RocketMQ and update related code base
- Configure and implement Redis R/W split, balanced production loading
- Implemented tax logic, include withholding tax and excise tax
- Kickoff Sporty-Fantasy
  - System planning and architecture design
  - Multi-countries, multi-users contest game
  - Communicate and integrate with third-party API
  - 80% of total code implementation
- Split payment module into user endpoint and third-party endpoint
- Optimize MTS process with multi-thread in parallel, keeps the flow in synchronized to asynchronized then back to synchronized
- Implement authentication of KYC, ensure the user experience of deposit/withdraw and prevent the fraud
- Implement new promotion (DoB Promotion)
- Implement finance flow, add new mechanism of deposit/withdraw in deep logic flow (PAC Account)
- Implement user transfer feature, allow authenticated user to transfer to each other (P2P transfer)
- Kickoff Sporty.com
  - System planning and architecture design, totally 7 modules
  - As a sports media app, include news, video, chat, share and social
  - Communicate and integrate with third-party API
  - 75% of total code implementation
- Solve performance issue and optimize huge amount of settlement messages at the same time
- Solve cache not exactly recycle in CMS GC, tuning JVM arguments and migrate to G1 GC
- Design log analysis system for app and web/wap
- SQL performance tuning for all modules
- Assistance of database migration, from cetus to AWS RDS, check and optimize required query
- Assistance of new country environment deploy, load test environment deploy
- Production issue tracking , find the issue in the first place and fix immediately before user affected
- Production outage handling
- Upgrade modules from Spring Boot 1.6 to 2.3
- Configure resource in Kubernetes, analysis issue and optimize
  - Optimize resource usage
  - Plan HPA and replicas scaling strategy
- Log system integration solution (cloudwatch, rsyslog, kafka)
- Introduce technologies, such as SonarQube、Webflux、gRPC、drone、KEDA

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
- Introduce docker container service for simplify development environment and deployment.
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

- Develop a sub module of vendor collaborative management system (VCMS). 
- Upgrade Vendor2G from .net 1.1 with crystal report.
- Refactoring usage of source control and create guideline for develop flow.
- Provide CI/Jenkins solution for build and archive binaries.

##### Tags

`VCMS` `Vendor2G` `SISO` | `.NET Web form` `SQL Server` `jQuery` `Jenkins` `SVN`

##### Links

* https://7-11vcms.pcsc.com.tw

------------------------------------------------------------------------

### Senior Technical Consultant @*HY-Tech*

> Dec 2014 - May 2017

- Construct architecture for new or exists project, integration with multiple system and data exchange.
- Performance tuning and optimize resource usage strategy.
- Simplify developing flow such as reduce repetitive code snippets and automate repetitive tasks.
- Improve and keep high quality such as provide develop guide, use static code analysis and code review.
- Research and provide solution for project and pre-sales.
- Develop and provide foundation component like aop or code generator.
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

- Develop AI(Ability International) order system based on web application and migrate old one from lotus notes
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

`SQL Server` `Oracle` `MySQL` `MariaDB` `PostgreSQL` `Mongodb` `PouchDB` `Couchbase` `Redis`

### Message Queue

`RabbitMQ` `Kafka`

### SCM 

`Git` `SVN` `Team Foundation Server`

### DevOps

`Jenkins` `TeamCity` `Gitlab-CI` `Consul` `Kubernetes` `Istio`

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
* Gitbook: https://www.gitbook.com/@nanashi07
* Github: https://github.com/prhythm
* Web components: https://www.webcomponents.org/author/Prhythm
* Chrome extensions: https://goo.gl/J62Khh
* App: https://play.google.com/store/apps/details?id=com.prhythm.billtracker
