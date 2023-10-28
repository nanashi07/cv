# Bruce Tsai - *軟體架構師*

![photo](https://github.com/nanashi07/cv/blob/master/bruce.jpg)

## 概要

擅長系統規劃與開發，分析並提升系統效能，在簡化開發流程，提升效率與產出品質方面有豐富的經驗。專注開發程式的效能與可維護性，精通多個系統與各種解決方案之間的整合，並且能夠獨立作業或帶領成員完成目標。習慣於面對困難並克服它們來促進業務發展。作為獨立貢獻者、導師、團隊合作者和領導者都有出色的表現。

主要使用語言為 Java 及 C# 進行開發，並以 Python / node.js / go / rust 等為輔助開發工具。熟悉但不限定於 Web 相關的系統，了解前端框架 Angular，Vue，Polymer，jQuery 等。熟悉 MySQL, SQL Server 等持久層。熟悉 Redis 等 NO-SQL/快取。熟悉使用 RocketMQ 和 RabbitMQ 等佇列系統的非同步流程。熟悉與 AWS 和 Azure 等雲端服務的整合。

除了開發之外，還熟悉 Kubernetes、Linux、Nginx、ELK、SonarQube、docker 等基礎架構。熟悉 AWS、Azure 等雲端服務。

熱愛自學技術技能，對軟體產業的變化敏感，習慣從日常新聞中學習。喜歡利用個人時間開發有趣的業餘項目。


## 經歷

### 技術總監 @*OpenNet*

> 七月 2019 - NOW

#### SportyBet
- 功能實作
  - 修正第三方函式庫臭蟲。覆寫第三方函式庫功能。
  - 實作 Redis 讀寫分離機制，平衡生產環境的負載。遷移高負載的 Redis 為叢集模式
  - 實作稅務處理，包含預扣稅與消費稅
  - 優化 MTS 處理流程，以多執行緒並行提高效能，並整合進同步轉非同步訂單流程
  - 實作 KYC 驗證流程，在保證儲值與提款的流暢體驗下防止詐騙與盗號
  - 實作 DoB 驗證與 promotion，以提供後續客戶 KYC 驗證資訊
  - 實作帳務流程，控制儲值/提款的底層邏輯 (PAC Account)
  - 實作用戶轉帳功能，允許通過驗證的用戶互相轉帳 (P2P transfer)
  - 設計日誌收集分析系統（analytics），供行動裝置回報分析
  - 設計並建構後端各模組與 CMS 系統整合
  - 修正 SonarQube 分析的 bug 與漏洞
- 效能優化
  - 解決並優化系統處理大量結算時的負載問題（settlement)
  - 優化比賽結算，分流不同優先級的資料，降低資料庫面的負擔，並減少不必要的冗餘運算
  - 各模組 SQL 效能調校，優化 DBA 監控提供的效能問題
  - 優化賽事資訊推送功能，減少延遲並提升推送服務的可擴展性
  - 優化各模組的 cache 使用，建立對應的指標以觀察 cache 的效能
  - 強化 Jaeger APM 的追蹤內容，改善效能追蹤時可提供的資訊
  - 設計多項監控指標，用以了解系統狀態，並快速反應異常
  - 解決程式造成的 GC 問題，調校 JVM 並改用 G1 GC 替代原本的 Parallel GC
  - 量測並分析 order 效能，細化指標後依據指標優化 order
  - 分析 SMS 模組 API 效能，優化改進，(Collection contains, parallel issue)
  - 分析 OOM、高 cpu、網路問題原因，並針對問題改善
  - 提升測試效能，包含啟動速度，環境執行速度（MySQL）
- 系統架構
  - 資料庫遷移，由 cetus 遷移至 AWS RDS，調整遷移時前後的查詢問題
  - 分離金流模組入口，拆分為用戶端入口與第三方入口，避免相互影響
  - 協助建立新國家部署，排除建置問題
  - 升級各模組 Spring Boot 1.6 至 2.3
  - 優化 Kubernetes 各類配置，並分析 kubernetes 的問題
  - Log system 整合方案 (cloudwatch, rsyslog, kafka, loki)
  - 重建壓測方案，使用 gatling 與 arg workflow
  - 持續重構各模組程式碼
  - 優化各模組的 maven dependency
  - 分離訂單模組，避免因流量或 bug 造成訂單問題。
  - 規劃並參與 TiDB、SQLProxy
  - 完成 Sharding JDBC 遷移計畫
#### Management
- 自 2021 年 1 月升為 principal engineer
- 自 2021 年 5 月擔任 backend team leader 
- 領導 Stability & Security 團隊，確保線上環境穩定，並自 2021 年初流量成長 4 倍
- 管理後端開發人員，引導同仁職涯發展，協助解決同仁開發困難
#### SportyBet - International
- 開發以 email 為基礎的註冊流程，支援多國家，多語言，多幣別會員
- 設計彈性動態的 KYC 功能
#### Games
- 遷移 Sporty Soccer  RabbitMQ 至 RocketMQ
- 啟動 Sporty Fantasy 專案
  - 系統整體規劃與設計
  - 多國、多人競合遊戲
  - 第三方 API 溝通與串接
  - 80% 的後端程式碼實作
#### Sporty.com
- 啟動 Sporty.com 專案
  - 系統整體規劃與設計，共 7 個模組
  - 定位為運動類型多媒體，包含新聞、影片、聊天、分享、社交等功能
  - 第三方 API 溝通與串接
  - 75% 的後端程式碼實作
#### Other
- 系統異常追蹤，主動發現問題並在造成影響前修復或降低影響
- 線上環境緊急災難應變
- 引入多項技術，包含 SonarQube、Webflux、gRPC、drone、KEDA, argo workflow, gatling
- 協助其它區域團隊改善系統架構

##### Tags

`SportyBet`, `Fantasy`, `Sporty.com`, `SportyBet-International` | `Java 8`, `Spring Boot`, `MySQL`, `Cetus`, `RocketMQ`, `RabbitMQ`, `Redis`, `ElasticSearch`, `Kubernetes`, `AWS`, `drone`, `gRPC`, `Reactive`, `Jaeger`, `Prometheus`

##### Links

* https://sportybet.com
* https://sporty.com

------------------------------------------------------------------------

### 工程師 @*思華科技*

> 十月 2018 - 七月 2019

- 擔任 backend 窗口，與各 team 溝通協調
- 制定 API 規格文件
- 建置 Gitlab 環境並保證其可用性
- 以 .net core 建置專案基礎功能與開發核心系統功能
- 評估並規劃 GCP、Azure 上的生產環境架構
- 以 Kubernetes (GKE) 與 helm 等相關方案建置生產環境
- 驗證技術方案與執行效能，如：
  * 驗證日誌套件的效能 (Nlog / Serilog / Log4net)
  * 驗證 redis client / server 方案 (StackExchange / ServiceStack / CsRedis / Cluster / Sentinel / Codis)
  * JSON 序列化效能 (Newtonsoft / Jil / Utf8Json)
  * 驗證 MySQL(MGR) 及其替代方案(Galera/XtraDB)在雲端服務上的可用性與效能
  * 非同步流程方案效能 (Queue / HangFire / Polly)
- 地端環境規劃建置
- 雲端環境管理規劃
- CI/CD 規劃建置
- 經驗分享與技術教學

##### Tags

`Trade`, `Profit` | `C#`, `.Net Core`, `Percona`, `Docker`, `Kubernetes`, `Redis`, `RabbitMQ`, `CentOS`, `Gitlab-CI`, `SonarQube`, `Graylog`, `ELK`, `MongoDB`, `GCP`, `Azure`, `Architect`, `Helm`, `HAProxy`

------------------------------------------------------------------------

### 工程部組長 @*一訂科技*

> 二月 2018 - 十月 2018

- 到職一個月內確保系統流程完整並進行上線
- 規劃 Azure 部署架構，在符合現況的條件下提供足夠的擴充彈性
- 導入 CI／CD (Gitlab)，簡化開發流程
- 導入 SonarQube 程式碼分析，提升程式碼品質
- 導入 Protobuf 處理異質系統的序列化問題
- 修正系統架構(原monolithic)，以 4-layer/3-tier 規劃開發架構，並以 REST API 提供對外接口重整各系統的功能架構
- 導入 .NET Core 2.0，並設計交易處理模式
- 要求單元／整合測試自動化，降低測試成本與提高系統品質
- 於一個月內完成配位系統（鎖位系統）POC，具有高承載能力，高可擴展性，能在瞬間大量使用者進入時仍保持運作正常 
- 導入容器服務用於處理分散式叢集服務
- 導入 ELK 日誌分析，處理系統監控與使用行為統計等
- 以自行設計的配位系統替換外包商的鎖位服務，並要求外包商退還數百萬設計費用
- 運用 Kubernetes (AKS) 管理容器的部署與運作
- 規劃並管理團隊任務，技術相關教育訓練

##### Tags

`Dingok` | `C#`, `.NET Framework`, `.Net Core`, `WPF`, `SQL Server`, `Azure`, `Docker`, `RabbitMQ`, `Redis`, `CentOS`, `Ubuntu`, `Gitlab`, `git`, `SonarQube`, `ELK`, `CI`, `CD`, `Protobuf`, `System Architect Design`, `Kubernetes`

##### Links

* https://dingok.com

------------------------------------------------------------------------

### 軟體工程師 @*統一資訊*

> 六月 2017 - 十二月 2017

- 開發 VCMS 的超商存貨模組 (.net web form / sql server)。
- 提供升級方案並升級 Vendor2G 系統(.Net Framework 1.1 / Crystal Report 10.0)。
- 建立並提供原始碼管控流程(SVN)與相關文件，協助團隊成員符合流程規範。
- 提供以 Jenkins 處理自動建置與封存的 CI 方案。

##### Tags

`VCMS`, `Vendor2G`, `SISO` | `.NET Web form`, `SQL Server`, `jQuery`, `Jenkins`, `SVN`

##### Links

* https://7-11vcms.pcsc.com.tw

------------------------------------------------------------------------

### 資深技術顧問 @*鴻揚科技股份有限公司*

> 十二月 2014 - 五月 2017

- 依客戶需求建置合適的軟體系統，整合複數的外部系統與各類介接服務。
- 優化系統執行時的效能，調整不同系統執行的資源策略。
- 簡化開發時的作業流程，減少重覆性的程式碼片段，以自動化處理重覆性作業
- 提高程式碼產出的品質，包含建立開發規範，引進程式碼分析，Code review 等
- 研究並提供專案與 pre-sale 合適的解決方案
- 提供開發上所需的基礎元件如 AOP 及 code generator 等
- 管理專案事務包含時程與需求，帶領專案人員完成目標
- 提供教育訓練資源並指導新進人員專業技術能力
- 維繫客戶關係並取得客戶信任

##### Tags

`Fetnet eService`, `Fetnet Code trace`, `NEC Cosmed`, `Arcoa NDRS`, `Arcoa EIP`, `Kingdu` | `Spring MVC`, `Struts`, `.NET MVC`, `Hibernate`, `MyBatis`, `Entity Framework`, `Dapper`, `ADO`, `Oracle`, `SQL Server`, `MySQL`, `angular.js`, `Vue`, `jQuery`, `weblogic`, `IIS`, `CentOS`, `RHEL`

##### Links

* http://ecare.fetnet.net/eServiceV3/
* http://ndrs.arcoa.com.tw/NDRS

------------------------------------------------------------------------

### 資深軟體工程師 @*趨勢科技*

> 十一月 2012 - 十月 2014

- 客製化 Umbraco CMS 供應商等存取權限管控功能
- 開發並維護 Microsoft office sharepoint 內容網站的功能
- 提供其它團隊技術支援

##### Tags

`ishare`, `ishare 2.0`, `ishare 3.0`, `Legal Contract Management system`, `Calendar Synchronization`, `BIF - Report information frontend`, `APAC Sales Kick-off`, `Quarterly IS Awards`, `The circle`, `Olympic 25th` | `Sharepoint`, `C#`, `jQuery`, `Android`

------------------------------------------------------------------------

### 資訊部副主任 @*上奇科技股份有限公司*

> 二月 2012 - 十月 2012

- 建置佳能國際(Ability International)簽呈系統並取代既有的 lotus notes 功能
- 維護佳能國際 CRM, 差假, 維修, 客服等內部系統
- 維護佳能國際與上奇科技的 EIP 系統
- 網路與硬體環境的規劃維護
- 支援上奇資訊與佳魁資料的 MIS 業務
- 維護 SAP 與 EIP 相關的報表 ETL，改善系統執行的效能
- SAP 日常事務處理
- 原始碼整理控管
- 其它 MIS 日常事務處理

------------------------------------------------------------------------

### 高級工程師 @*超眾科技*

> 五月 2010 - 二月 2012

- 建置生產流程使用的 MES 系統
- 開發鼎新 GP 的工作流程
- 維護 Tiptop 相關的程式
- 維護公司官方網站
- 支援 RD 研發時與 MIS 相關的作業流程
- 支援硬體與網路相關的故障維護

------------------------------------------------------------------------

### 軟體工程師 @*中華電信政網處*

> 七月 2008 - 五月 2010

- 護電子化政府 - 我的 e 政府相關的服務與模組
- 開發電子化政府與外部系統相關的介接程式
- 以 Worksite MP 開發 KMS 系統

------------------------------------------------------------------------

### 軟體工程師 @*創世紀資訊*

> 二月 2007 - 六月 2008

- 既有系統及專案維護, 小型購物網站, 企業形象網站建置與開發,。
- 主要應用技術為 JSP/Servlet, 資料庫應用為 MySQL 與 SQLServer

## 學歷

### 中國文化大學

> 1998 - 2004

資訊管理學系／日文系雙學位。

## 技能

### 語言能力

`Chinese`, `English`, `Japanese`

### 程式語言

`Java`, `C#`, `.Net Framework`, `.Net Core`, `Javascript`, `Kotlin`, `Python`, `node.js`, `Go`, `Rust`

### 前端框架

`jQuery`, `Angular`, `Vue`, `Polymer`, `LitElement`

### 作業系統

`Windows`, `CentOS`, `Ubuntu`, `MacOS`

### 資料庫

`MySQL`, `SQL Server`, `Oracle`, `MariaDB`, `PostgreSQL`, `Mongodb`, `PouchDB`, `Couchbase`, `Redis`, `Cetus`

### 佇列

`RabbitMQ`, `Kafka`, `RocketMQ`

### 版本控制

`Git`, `SVN`, `Team Foundation Server`

### DevOps

`Kubernetes`, `Jenkins`, `TeamCity`, `Gitlab-CI`, `Consul`, `Istio`, `Argo workflow`

### 虛擬化

`Virtualbox`, `Hyper-V`, `Docker`, `KVM`, `Promox`

### 行動裝置

`Android (Native)`

### 設計

`系統架構`, `系統整合`, `文件化`, `系統分析`

### 管理

`團隊領導`, `文化建立`, `溝通`, `教育訓練與指導`, `專案管理`

## 個人活動

* Blog: https://nanashi07.blogspot.tw/
* Github: https://github.com/prhythm, https://github.com/nanashi07
* Web components: https://www.webcomponents.org/author/Prhythm
* Chrome extensions: https://goo.gl/J62Khh
