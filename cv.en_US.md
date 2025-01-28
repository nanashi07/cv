# Bruce Tsai - *Software Architect*

![photo](https://github.com/nanashi07/cv/blob/master/bruce.jpg)

## Summary

Familiar with system design, software development, system analysis and performance tuning. Experienced in improving the efficiency of the development process and producing quality. Focus on performance issues and the maintainability of development. Highly skilled in integration between multiple systems with various solutions. Had used to face difficulties and overcome them to help business growth. Excellent performance as an independent contributor, mentor, team player and leader.

The majority use Java and C# for development, and others use Python, Node.js, Go, Rust, etc. for assistance. Familiar with web-based systems and experienced with frameworks like Angular, Vue, Polymer, jQuery and so on. Familiar with persistence layers such as MySQL and SQL Server; familiar with NO-SQL/cache such as Redis; familiar with asyncrhonized process flow using queue systems such as RocketMQ and RabbitMQ; familiar with integration with cloud services such as AWS and Azure.

Beside development, be familiar with infrastructure such as Kubernetes, Linux, Nginx, ELK, SonarQube, docker, etc. Experienced with the cloud services such as AWS and Azure.

Love self-learning technology skills, sensitive to the changes in the software industry, used to learn from the daily news. Love to develop interesting side-project on my personal time.


## Work experience

### Principal engineer @*OpenNet*

> Jul 2019 - NOW

#### SportyBet
- Feature implementation
  - Fixed issue of third-party library, hacked library for system requirement
  - Configured and implemented Redis R/W access, balanced loading in production. Migrated high-loaded Redis to cluster mode
  - Implemented tax logic, including withholding tax and excise tax
  - Optimized MTS process with multi-thread, integrated with sync-to-async conversion in order flow
  - Implemented KYC, ensure user experience in deposit/withdraw and avoid fraud from users
  - Implemented DoB promotion, provided trusted info for KYC
  - Implemented finance flow, added new mechanism of deposit in core logic flow (PAC Account)
  - Implemented a supporter feature, allowed verified users to transfer money to another user (P2P transfer)
  - Designed and implemented a log analysis service for mobile devices
  - Designed and integrated all modules into the CMS
  - Fix bugs and vulnerabilities scanned by SonarQube.
- Performance
  - Solved and optimized performance issues on a huge number of settlement messages at the same time
  - Optimized settlement flow, decreased load on the database, decreased unnecessary or duplicate computing
  - SQL performance tuning for all modules, based on the monitor from DBA or metrics
  - Optimized message push service, decreased push delay and increased scalability of service
  - Optimized memory cache usage, created metrics for caches for performance tuning
  - Enhanced Jaeger APM, provided more information on tracing performance issues.
  - Added various metrics, made system status and abnormalities clear. Fix issues before damage is encountered.
  - Solved the cache issue caused by full GC, tuned JVM arguments and migrated parallel GC to G1 GC
  - Measured and analyzed the performance of order service, made the metrics more clear, and made improvement depend on them.
  - Analyzed the API performance of the SMS module, improved incorrect collection usage, and solved parallel issues.
  - Analyzed OOM, high CPU and network issues
  - Improved test performance, including code performance and environment performance (MySql)
- Architecture
  - Assist database migration, from Cetus to AWS RDS by rewriting and optimizing parts of queries
  - Split the payment service into user oriental and third-party oriental services, prevent them from affecting each other
  - Helped with new country environment deployment and troubleshooting relevant issues
  - Upgrade services from Spring Boot 1.6 to 2.3
  - Optimized resource configuration in Kubernetes, analysis issues on production
  - Log system integration solution implementation (cloudwatch, rsyslog, kafka, loki)
  - Continuous code refactoring
  - Optimized maven dependency for all modules
  - Split the order module to avoid traffic and transactions interrupted by query performance issues.
  - Planned and participated in TiDB, SQL Proxy POC
  - Provided a Redis migrate solution for the risk team. Completed the Elasticsearch migration independently.
  - Refactored and integrated settlement flow, made related flow controllable, and improved performance.
  - Design and implement Multi-Redis architecture to resolve the resolve the infrastructure limitation to single Redis cluster.
  - Refactor the system kernal, allow multiple systems deploy on single infrastructure
- Innovation
  - Built load test solution with Gatling and Argo workflow
  - Designed and implemented Sharding JDBC migration on multiple modules
  - Proposed optimized booking code solution, allows unified code across regions and provides more business value
  - Proposed the concept of any-bet, exploring more market opportunities
#### Management
- Principal engineer since Jan 2021
- Backend team leader since May 2021
- Technical director since Jan 2023
- Senior technical director since Jan 2025
- Lead the Stability & Security team, ensured production environment is as robust and stable as possible. Traffic at the end of 2024 increased by 20 times from earlier in 2021.
- Backend team and technical teams management
- Team culture and strategy management
#### SportyBet - International
- Designed and implemented email-based registration, multiple countries, multiple languages, and multiple currencies supported
- Designed and implemented dynamic, flexible KYC
#### Games
- Migrate RabbitMQ to RocketMQ for Sporty Soccer
- Kickoff Sporty-Fantasy
  - System planning and architecture design
  - Multi-country, multi-user contest game
  - Communicated and integrated with third-party APIs
  - 80% of total code implementation
#### Sporty.com
- Kickoff Sporty.com
  - System planning and architecture design, totaling 7 modules
  - As a sports media app, include news, video, chat, sharing, and social features
  - Communicated and integrated with third-party APIs
  - 75% of total code implementation
#### Other
- Production issue trace: find the issue in the first place and fix it immediately before users are affected
- Production incidents handling
- Introduced solutions, such as SonarQube, Webflux, gRPC, drone, KEDA, Argo workflow, Gatling
- Assist architecture design cross teams in other regions

##### Tags

`SportyBet`, `Fantasy`, `Sporty.com` | `Java`, `Spring Boot`, `MySQL`, `Cetus`, `RocketMQ`, `RabbitMQ`, `Reids`, `ElasticSearch`, `Kubernetes`, `AWS`, `drone`, `gRPC`, `Reactive`, `Jaeger(opentracing)`, `Prometheus`

##### Links

* https://sportybet.com
* https://sporty.com

------------------------------------------------------------------------

### Engineer @*Silkrode  Technologies Co., Ltd.*

> Oct 2018 - Jul 2019

- Be the backend contact and coordinate with each team.
- Defined API specifications.
- Built Gitlab and ensured its availability.
- Built the required foundation structure and developed the core system using .NET Core.
- Evaluated and planned architecture of production on GCP and Azure cloud
- Built production with Kubernetes(GKE), Helm and other related solutions
- Verification of the technical solutions includes:
  * Performance of the logging library (Nlog / Serilog / Log4net)
  * Redis client / server solution (StackExchange / ServiceStack / CsRedis / Cluster / Sentinel / Codis)
  * Performance of JSON serialization  (Newtonsoft / Jil / Utf8Json)
  * Availability and performance of MySQL (MGR) and its alternatives (Galera/XtraDB) on cloud services.
  * Asynchronized process performance. (Queue / HangFire / Polly)
- Intranet environment planning and construction.
- Management of the cloud environment.
- CI/CD planning and implementation
- Sharing and technical training

##### Tags

`Trade`, `Profit` | `C#`, `.Net Core`, `Percona`, `Docker`, `Kubernetes`, `Redis`, `RabbitMQ`, `CentOS`, `Gitlab-CI`, `SonarQube`, `Graylog`, `ELK`, `MongoDB`, `GCP`, `Azure`, `Architect`, `Helm`, `HAProxy`

------------------------------------------------------------------------

### Leader of Engineers @*Dingok*

> Feb 2018 - Oct 2018

- Planned and architected deployment on Azure.
- Introduced CI/CD using Gitlab, defined and simplified the development flow.
- Introduced code analysis using SonarQube and ensured code quality.
- Introduced Protobuf for serialization between platforms
- Reconstructed monolithic system structure by 4-layer/3-tier design
- Introduced .NET Core 2.0 for new feature development.
- Asked team members to provide automatic unit and integration tests, reduced test costs and improve system quality.
- Completed a POC of seat allocation service in one month with high loading, capability, availability and scalability.
- Introduced docker container service to simplify the development environment and deployment.
- Introduced ELK log analysis for monitoring and behavior analytics.
- Replaced the outsourced allocation system with a self-designed service and claimed a refund of paid fees.
- Introduced Kubernetes for container deployment and management.
- Planned and managed for team jobs and technical trainings

##### Tags

`Dingok` | `C#`, `.NET Framework`, `.Net Core`, `WPF`, `SQL Server`, `Azure` `Docker`, `RabbitMQ`, `Redis`, `CentOS`, `Ubuntu`, `Gitlab`, `git`, `SonarQube`, `ELK`, `CI`, `CD`, `Protobuf`, `System Architect Design`, `k8s`

##### Links

* https://dingok.com (deprecated)

------------------------------------------------------------------------

### Engineer @*President Information Corporation*

> Jun 2017 - Dec 2017

- Developed a submodule of the vendor collaborative management system (VCMS). 
- Upgraded Vendor2G from .NET 1.1 by crystal report.
- Refactored the usage of source control and created guidelines for development flow.
- Provided CI/Jenkins solutions to build and archive binaries.

##### Tags

`VCMS`, `Vendor2G`, `SISO` | `.NET Web form`, `SQL Server`, `jQuery`, `Jenkins`, `SVN`

##### Links

* https://7-11vcms.pcsc.com.tw

------------------------------------------------------------------------

### Senior Technical Consultant @*HY-Tech*

> Dec 2014 - May 2017

- Construct architecture for new or existing projects, integration with multiple systems, and data exchange.
- Performance tuning and optimizing resource usage strategies
- Simplify the development flow, such as by reducing repetitive code snippets and automating repetitive tasks.
- Improve and keep high quality, such as by providing a development guide, using static code analysis and code review.
- Research and provide solutions for projects and pre-sales.
- Develop and provide foundation components like AOP or code generator.
- Manage the project schedule and task assignment, and lead members to achieve the goal.
- Provide training in project-related skills for newbies and team members.
- Communicate with customers and earn their trust and recognition.

##### Tags

`Fetnet eService`, `Fetnet Code trace`, `NEC Cosmed`, `Arcoa NDRS`, `Arcoa EIP`, `Kingdu` | `Spring MVC`, `Struts`, `.NET MVC`, `Hibernate`, `MyBatis`, `Entity Framework`, `Dapper`, `ADO`, `Oracle`, `SQL Server`, `MySQL`, `angular.js`, `Vue` `jQuery`, `weblogic`, `IIS`, `CentOS`, `RHEL`

##### Links

* http://ecare.fetnet.net/eServiceV3/
* http://ndrs.arcoa.com.tw/NDRS

------------------------------------------------------------------------

### Senior Software Engineer @*Trend Micro*

> Nov 2012 - Oct 2014

- Customize Umbraco CMS and design the function of supplier or distributor access control
- Develop, maintain and manage project systems based on Microsoft Office SharePoint.
- Supply technical support for other teams

##### Tags

`ishare`, `ishare 2.0`, `ishare 3.0`, `Legal Contract Management system`, `Calendar Synchronization`, `BIF - Report information frontend`, `APAC Sales Kick-off`, `Quarterly IS Awards`, `The circle`, `Olympic 25th` | `Sharepoint`, `C#`, `jQuery`, `Android`

------------------------------------------------------------------------

### MIS Deputy Supervisor @*GrandTech Systems Ltd*

> Feb 2012 - Oct 2012

- Develop AI (Ability International) order system based on a web application and migrate the old one from Lotus Notes.
- Develop CRM, attendance, repair service, and customer service for departments of AI
- Maintain the EIP of GrandTech and AI
- Network and server maintenance
- MIS supports GI (GrandTech Information) and  TI (TopTeam Information)
- Develop and maintain ETL and reports from SAP and EIP, and perform performance tuning for execution.
- Routine jobs and maintenance of SAP
- Source control reconstruction
- Daily jobs of the MIS department

------------------------------------------------------------------------

### Senior Engineer @*CHAUN-CHOUNG TECHNOLOGY CORP.*

> May 2010 - Feb 2012

- Develop MES for manufacturing flow.
- Develop workflows for departments using GP
- Support and maintain Tiptop
- Maintenance of the web portal
- Develop functional features for departments
- Support the general application process for RD.
- Support network and hardware maintenance

------------------------------------------------------------------------

### Engineer @*Chunghwa Telecom (MyEgov & GSP Operation Center)*

> Jul 2008 - May 2010

- Develop and maintain the eGov portal
- Develop and maintain eGov modules and services
- Develop and maintain a data exchange interface and function
- Customize Worksite MP as KMS

------------------------------------------------------------------------

### Engineer @*GENESIS INFORMATION INC.*

> Feb 2007 - Jun 2008

- Maintenance of the customer's system. Develop an online shopping site and enterprise portal.
- Mainly use JSP/Servlet, MySQL and SQL Server

## Education

### Chinese Culture University

> 1998 - 2004

Both information management and Japanese language and literature


## Skills

### Language

`Chinese`, `English`, `Japanese`

### Programming Language

`Java`, `C#`, `.Net Framework`, `.Net Core`, `Javascript`, `Kotlin`, `Python`, `node.js`, `Go`, `Rust`

### Front End

`jQuery`, `Angular`, `Vue`, `Polymer`, `LitElement`

### OS

`Windows`, `CentOS`, `Ubuntu`, `MacOS`

### Database

`MySQL`, `SQL Server`, `Oracle`, `MariaDB`, `PostgreSQL`, `Mongodb`, `PouchDB`, `Couchbase`, `Redis`, `Cetus`

### Message Queue

`RabbitMQ`, `Kafka`, `RocketMQ`

### SCM 

`Git`, `SVN`, `Team Foundation Server`

### DevOps

`Kubernetes`, `Jenkins`, `TeamCity`, `Gitlab-CI`, `Consul`, `Istio`, `Argo workflow`

### Virtualization

`Virtualbox`, `Hyper-V`, `Docker`, `KVM`, `Promox`

### Mobile 

`Android (Native)`

### Design 

`System architect`, `System integration`, `Documentation`, `System analysis`

### Management

`Team leading`, `Culture establish`, `Communication`, `Training and mentoring`, `Project management`

## Personal Links

* Blog: https://nanashi07.blogspot.tw/
* Github: https://github.com/prhythm, https://github.com/nanashi07
* Web components: https://www.webcomponents.org/author/Prhythm
* Chrome extensions: https://goo.gl/J62Khh
