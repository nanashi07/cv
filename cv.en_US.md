# Bruce Tsai - _Software Architect_

## Summary

Goal-driven management and 2× AI creative productivity. Proficient in system design, software development, system analysis, and performance tuning. Experienced in enhancing development efficiency and ensuring software quality. Focused on performance optimization and development maintainability. Highly skilled in system integration with diverse solutions. Accustomed to overcoming challenges and driving business growth. Performs excellently as an independent contributor, mentor, team player, and leader.

Primarily uses Java and C# for development; additionally proficient with Python, Node.js, Go, Rust, and more. Familiar with web-based systems and frameworks such as Angular, Vue, Polymer, and jQuery. Experienced with persistence layers like MySQL and SQL Server; also familiar with NoSQL/caching solutions like Redis. Knowledgeable in asynchronous process flows using message queues like RocketMQ and RabbitMQ, and in integrating cloud services such as AWS and Azure.

Beyond development, experienced with infrastructure technologies including Kubernetes, Linux, Nginx, ELK, SonarQube, Docker, and more. Well-versed in cloud services including AWS and Azure.

A passionate self-learner, attuned to changes in the software industry, and regularly follows industry news. Enjoys building interesting side projects during personal time.

---

## Work Experience

### Principal Engineer @ _OpenNet_

> Jul 2019 – Present

#### Development, Performance, and Stability

- **Feature Implementation and Delivery**

  - Developed tax logic including withholding and excise tax.
  - Optimized MTS process using multithreading and sync-to-async conversion within the order flow.
  - Implemented KYC, enhancing user experience in deposit/withdrawal and mitigating fraud.
  - Delivered DoB promotion to provide trusted data for KYC.
  - Built finance flows and integrated a new deposit mechanism (PAC Account) into the core logic.
  - Created P2P transfer feature for verified users.
  - Designed and implemented a mobile device log analysis service.
  - Integrated all modules into the CMS.
  - Fixed bugs and vulnerabilities flagged by SonarQube.
  - Supported deployments for new country environments and resolved related issues.
  - Developed email-based registration supporting multiple countries, languages, and currencies.
  - Designed dynamic, flexible KYC system.

  - **Games**

    - Migrated Sporty Soccer from RabbitMQ to RocketMQ.
    - Launched Sporty-Fantasy:

      - Led system planning and architecture design.
      - Developed multi-country, multi-user contest game.
      - Integrated with third-party APIs.

  - **Sporty.com**

    - Designed and developed seven modules for a sports media app (news, video, chat, sharing, social features).
    - Integrated with third-party APIs.

- **Performance**

  - Resolved issues in third-party libraries and enhanced tracing capability.
  - Configured Redis read/write access for load balancing; migrated Redis to cluster mode.
  - Optimized settlement flow and reduced unnecessary computation and DB load.
  - Conducted SQL performance tuning across modules using DBA metrics.
  - Improved message push service latency and scalability by a middle queue layer.
  - Enhanced memory cache performance and introduced performance metrics.
  - Improved Jaeger APM instrumentation for better trace analysis.
  - Added metrics to clarify system status and detect abnormalities proactively.
  - Resolved cache issues from full GC; optimized JVM settings (migrated from Parallel GC to G1 GC).
  - Measured and improved order service performance using metrics.
  - Tuned SMS module APIs for collection usage and parallelism.
  - Diagnosed and resolved OOM, high CPU, and network bottlenecks.
  - Enhanced testing performance (code and MySQL) by ~50%.

- **Stability**

  - Proactively traced production issues to prevent user impact.
  - Handled production incidents while maintaining 99.99% SLA.
  - Provided architectural assistance across regions.

#### Architecture & Innovation

- **Architecture**

  - Led database migration from Cetus to AWS RDS with optimized queries.
  - Split payment services to isolate use cases and prevent cross-impact.
  - Upgraded Spring Boot from 1.6 to 2.3 and aligned codebase across modules.
  - Tuned Kubernetes resource allocation based on production analysis.
  - Implemented integrated log system (CloudWatch, rsyslog, Kafka, Loki).
  - Standardized and simplified Maven dependencies across services.
  - Split order modules to isolate transaction vs. query load for scalable performance.
  - Contributed to TiDB/SQL Proxy POC planning and execution.
  - Led Sharding JDBC migration for multiple modules to eliminate DB bottlenecks.
  - Proposed and executed Redis migration for the risk team to resolve big key issues.
  - Migrated Elasticsearch independently and flawlessly.
  - Replaced leader node mechanism with Raft for better scalability.
  - Refactored settlement flow to prioritize resettlement and enhance performance.
  - Designed and implemented Multi-Redis architecture to bypass AWS constraints and reduce cluster impact.
  - Refactored system kernel to support multiple deployments on shared infrastructure, reducing cost and improving flexibility.

- **Innovation**

  - Introduced tools like SonarQube, Webflux, gRPC, Drone, KEDA, Argo Workflow, Gatling.
  - Built load testing framework using Gatling + Argo Workflow.
  - Proposed and implemented a unified booking code system across regions, reducing costs by 70%.
  - Pitched "any-bet" concept, exploring broader market opportunities.

#### Management

- Promoted to:

  - Principal Engineer (Jan 2021)
  - Backend Team Lead (May 2021)
  - Technical Director (Jan 2023)
  - Senior Technical Director (Jan 2025)

- Led the Stability & Security team to ensure maximum production robustness; traffic grew 20× from 2021 to 2024.
- Managed over 150 engineers across Taiwan, India, Europe, and Brazil.
- Focused on goal-driven team culture and strategy.

#### Other

**Tags**: `SportyBet`, `Fantasy`, `Sporty.com` | `Java`, `Spring Boot`, `MySQL`, `Cetus`, `RocketMQ`, `RabbitMQ`, `Redis`, `Elasticsearch`, `Kubernetes`, `AWS`, `Drone`, `gRPC`, `Reactive`, `Jaeger`, `Prometheus`

**Links**:

- [sportybet.com](https://sportybet.com)
- [sporty.com](https://sporty.com)

---

### Engineer @_Silkrode Technologies Co., Ltd._

> Oct 2018 - Jul 2019

- Be the backend contact and coordinate with each team.
- Defined API specifications.
- Built Gitlab and ensured its availability.
- Built the required foundation structure and developed the core system using .NET Core.
- Evaluated and planned architecture of production on GCP and Azure cloud
- Built production with Kubernetes(GKE), Helm and other related solutions
- Verification of the technical solutions includes:
  - Performance of the logging library (Nlog / Serilog / Log4net)
  - Redis client / server solution (StackExchange / ServiceStack / CsRedis / Cluster / Sentinel / Codis)
  - Performance of JSON serialization (Newtonsoft / Jil / Utf8Json)
  - Availability and performance of MySQL (MGR) and its alternatives (Galera/XtraDB) on cloud services.
  - Asynchronized process performance. (Queue / HangFire / Polly)
- Intranet environment planning and construction.
- Management of the cloud environment.
- CI/CD planning and implementation
- Sharing and technical training

##### Tags

`Trade`, `Profit` | `C#`, `.Net Core`, `Percona`, `Docker`, `Kubernetes`, `Redis`, `RabbitMQ`, `CentOS`, `Gitlab-CI`, `SonarQube`, `Graylog`, `ELK`, `MongoDB`, `GCP`, `Azure`, `Architect`, `Helm`, `HAProxy`

---

### Leader of Engineers @_Dingok_

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

- https://dingok.com (deprecated)

---

### Engineer @_President Information Corporation_

> Jun 2017 - Dec 2017

- Developed a submodule of the vendor collaborative management system (VCMS).
- Upgraded Vendor2G from .NET 1.1 by crystal report.
- Refactored the usage of source control and created guidelines for development flow.
- Provided CI/Jenkins solutions to build and archive binaries.

##### Tags

`VCMS`, `Vendor2G`, `SISO` | `.NET Web form`, `SQL Server`, `jQuery`, `Jenkins`, `SVN`

##### Links

- https://7-11vcms.pcsc.com.tw

---

### Senior Technical Consultant @_HY-Tech_

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

- http://ecare.fetnet.net/eServiceV3/
- http://ndrs.arcoa.com.tw/NDRS

---

### Senior Software Engineer @_Trend Micro_

> Nov 2012 - Oct 2014

- Customize Umbraco CMS and design the function of supplier or distributor access control
- Develop, maintain and manage project systems based on Microsoft Office SharePoint.
- Supply technical support for other teams

##### Tags

`ishare`, `ishare 2.0`, `ishare 3.0`, `Legal Contract Management system`, `Calendar Synchronization`, `BIF - Report information frontend`, `APAC Sales Kick-off`, `Quarterly IS Awards`, `The circle`, `Olympic 25th` | `Sharepoint`, `C#`, `jQuery`, `Android`

---

### MIS Deputy Supervisor @_GrandTech Systems Ltd_

> Feb 2012 - Oct 2012

- Develop AI (Ability International) order system based on a web application and migrate the old one from Lotus Notes.
- Develop CRM, attendance, repair service, and customer service for departments of AI
- Maintain the EIP of GrandTech and AI
- Network and server maintenance
- MIS supports GI (GrandTech Information) and TI (TopTeam Information)
- Develop and maintain ETL and reports from SAP and EIP, and perform performance tuning for execution.
- Routine jobs and maintenance of SAP
- Source control reconstruction
- Daily jobs of the MIS department

---

### Senior Engineer @_CHAUN-CHOUNG TECHNOLOGY CORP._

> May 2010 - Feb 2012

- Develop MES for manufacturing flow.
- Develop workflows for departments using GP
- Support and maintain Tiptop
- Maintenance of the web portal
- Develop functional features for departments
- Support the general application process for RD.
- Support network and hardware maintenance

---

### Engineer @_Chunghwa Telecom (MyEgov & GSP Operation Center)_

> Jul 2008 - May 2010

- Develop and maintain the eGov portal
- Develop and maintain eGov modules and services
- Develop and maintain a data exchange interface and function
- Customize Worksite MP as KMS

---

### Engineer @_GENESIS INFORMATION INC._

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

- Github: https://github.com/prhythm, https://github.com/nanashi07
- Web components: https://www.webcomponents.org/author/Prhythm
- Chrome extensions: https://goo.gl/J62Khh
