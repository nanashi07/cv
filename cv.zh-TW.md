# Bruce Tsai - _軟體架構師_

## 摘要

以目標導向管理與 2 倍 AI 創意生產力為核心。精通系統設計、軟體開發、系統分析與效能調校，擁有提升開發效率與確保軟體品質的豐富經驗。專注於效能最佳化與開發維護性。擅長整合多種解決方案的系統整合，習慣迎接挑戰並推動業務成長。在獨立貢獻、指導、團隊合作與領導方面均有卓越表現。

主要使用 Java 與 C# 進行開發；同時熟悉 Python、Node.js、Go、Rust 等語言。熟悉基於網頁的系統與框架，例如 Angular、Vue、Polymer、jQuery。具備使用 MySQL 與 SQL Server 的經驗；亦熟悉 Redis 等 NoSQL／快取解決方案。了解使用 RocketMQ 與 RabbitMQ 等訊息佇列的非同步流程，並熟悉整合 AWS、Azure 等雲端服務。

除了開發外，亦具備 Kubernetes、Linux、Nginx、ELK、SonarQube、Docker 等基礎設施技術經驗。精通 AWS 與 Azure 雲端服務。

為一熱愛自學者，緊貼軟體產業的變化，定期關注業界動態。閒暇時間喜歡開發有趣的個人專案。

---

## 工作經驗

### 首席工程師 @ _OpenNet_

> 2019 年 7 月 – 至今

#### 開發、效能與穩定性

- **功能實作與交付**

  - 開發稅務邏輯，包括預扣稅與消費稅。
  - 透過多執行緒與同步轉非同步優化訂單流程的 MTS 處理。
  - 實作 KYC 功能，提升存提款用戶體驗並降低詐欺風險。
  - 推出 DoB 推廣活動，提供可信資料以支援 KYC。
  - 建立財務流程並整合新存款機制（PAC 帳戶）至核心邏輯中。
  - 為驗證用戶打造 P2P 轉帳功能。
  - 設計並實作行動裝置日誌分析服務。
  - 將所有模組整合至 CMS。
  - 修復 SonarQube 掃描出的錯誤與漏洞。
  - 支援新國家環境部署並解決相關問題。
  - 開發支援多國、多語系與多幣別的電子郵件註冊功能。
  - 設計動態且具彈性的 KYC 系統。

  - **遊戲相關**

    - 將 Sporty Soccer 從 RabbitMQ 遷移至 RocketMQ。
    - 推出 Sporty-Fantasy：

      - 主導系統規劃與架構設計。
      - 開發支援多國、多用戶的競賽型遊戲。
      - 整合第三方 API。

  - **Sporty.com**

    - 設計與開發七個體育媒體應用模組（新聞、影片、聊天室、分享、社交功能等）。
    - 整合第三方 API。

- **效能**

  - 修復第三方函式庫問題並強化追蹤能力。
  - 配置 Redis 讀寫分離以達成負載平衡；將 Redis 遷移至叢集模式。
  - 優化結算流程，減少不必要計算與資料庫負載。
  - 使用 DBA 指標調整多模組的 SQL 效能。
  - 透過中介佇列層改善訊息推送服務的延遲與擴展性。
  - 強化記憶體快取效能，並導入效能指標。
  - 改進 Jaeger APM 標示方式以提升追蹤分析。
  - 增加指標以釐清系統狀態並主動偵測異常。
  - 解決快取因 Full GC 而導致的問題；優化 JVM 設定（從 Parallel GC 遷移至 G1 GC）。
  - 使用指標測量與提升訂單服務效能。
  - 優化 SMS 模組 API 的集合使用與平行處理。
  - 診斷並解決 OOM、高 CPU 與網路瓶頸等問題。
  - 測試（代碼與 MySQL）效能提升約 50%。

- **穩定性**

  - 主動追蹤生產問題，防止用戶受影響。
  - 處理生產事故並維持 99.99% SLA。
  - 提供跨區域架構支援。

#### 架構與創新

- **架構**

  - 主導資料庫從 Cetus 遷移至 AWS RDS，並優化查詢。
  - 拆分付款服務以隔離使用場景，避免交叉影響。
  - 將 Spring Boot 從 1.6 升級至 2.3，統一模組代碼。
  - 根據生產分析調整 Kubernetes 資源分配。
  - 實作整合式日誌系統（CloudWatch、rsyslog、Kafka、Loki）。
  - 標準化與簡化所有服務的 Maven 相依性。
  - 拆分訂單模組以分離交易與查詢負載，提升可擴展性。
  - 將 leader node 機制改為 Raft 以提升擴展性。
  - 協助 TiDB／SQL Proxy POC 規劃與執行。
  - 提議並推動 Redis 遷移以解決風控團隊的 big key 問題。
  - 獨立完成 Elasticsearch 遷移，表現無瑕。
  - 重構結算流程以優先處理補結算並提升效能。
  - 設計並實作 Multi-Redis 架構，突破 AWS 限制並降低叢集影響。
  - 重構系統核心以支援共用基礎架構上的多重部署，降低成本並提升彈性。

- **創新**

  - 導入 SonarQube、Webflux、gRPC、Drone、KEDA、Argo Workflow、Gatling 等工具。
  - 使用 Gatling + Argo Workflow 建立壓力測試框架。
  - 主導多模組 Sharding JDBC 遷移以排除資料庫瓶頸。
  - 提案並實作跨區域統一的 booking code 系統，降低 70% 成本。
  - 提出「any-bet」概念，探索更廣泛的市場機會。

#### 管理

- 晉升歷程：

  - 首席工程師（2021 年 1 月）
  - 後端團隊主管（2021 年 5 月）
  - 技術總監（2023 年 1 月）
  - 高級技術總監（2025 年 1 月）

- 領導穩定性與安全性團隊，確保生產環境穩定性；流量自 2021 至 2024 年增長 20 倍。
- 管理超過 150 位來自亞洲、印度、歐洲與美洲的工程師。
- 專注於以目標導向的團隊文化與策略推動。

##### Tags

`SportyBet`, `Fantasy`, `Sporty.com`, `SportyBet-International` | `Java 8`, `Spring Boot`, `MySQL`, `Cetus`, `RocketMQ`, `RabbitMQ`, `Redis`, `ElasticSearch`, `Kubernetes`, `AWS`, `drone`, `gRPC`, `Reactive`, `Jaeger`, `Prometheus`

##### Links

- https://sportybet.com
- https://sporty.com

---

### 工程師 @_思華科技_

> 十月 2018 - 七月 2019

- 擔任 backend 窗口，與各 team 溝通協調
- 制定 API 規格文件
- 建置 Gitlab 環境並保證其可用性
- 以 .net core 建置專案基礎功能與開發核心系統功能
- 評估並規劃 GCP、Azure 上的生產環境架構
- 以 Kubernetes (GKE) 與 helm 等相關方案建置生產環境
- 驗證技術方案與執行效能，如：
  - 驗證日誌套件的效能 (Nlog / Serilog / Log4net)
  - 驗證 redis client / server 方案 (StackExchange / ServiceStack / CsRedis / Cluster / Sentinel / Codis)
  - JSON 序列化效能 (Newtonsoft / Jil / Utf8Json)
  - 驗證 MySQL(MGR) 及其替代方案(Galera/XtraDB)在雲端服務上的可用性與效能
  - 非同步流程方案效能 (Queue / HangFire / Polly)
- 地端環境規劃建置
- 雲端環境管理規劃
- CI/CD 規劃建置
- 經驗分享與技術教學

##### Tags

`Trade`, `Profit` | `C#`, `.Net Core`, `Percona`, `Docker`, `Kubernetes`, `Redis`, `RabbitMQ`, `CentOS`, `Gitlab-CI`, `SonarQube`, `Graylog`, `ELK`, `MongoDB`, `GCP`, `Azure`, `Architect`, `Helm`, `HAProxy`

---

### 工程部組長 @_一訂科技_

> 二月 2018 - 十月 2018

- 到職一個月內確保系統流程完整並進行上線
- 規劃 Azure 部署架構，在符合現況的條件下提供足夠的擴充彈性
- 導入 CI／CD (Gitlab)，簡化開發流程
- 導入 SonarQube 程式碼分析，提升程式碼品質
- 導入 Protobuf 處理異質系統的序列化問題
- 修正系統架構(原 monolithic)，以 4-layer/3-tier 規劃開發架構，並以 REST API 提供對外接口重整各系統的功能架構
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

- https://dingok.com (deprecated)

---

### 軟體工程師 @_統一資訊_

> 六月 2017 - 十二月 2017

- 開發 VCMS 的超商存貨模組 (.net web form / sql server)。
- 提供升級方案並升級 Vendor2G 系統(.Net Framework 1.1 / Crystal Report 10.0)。
- 建立並提供原始碼管控流程(SVN)與相關文件，協助團隊成員符合流程規範。
- 提供以 Jenkins 處理自動建置與封存的 CI 方案。

##### Tags

`VCMS`, `Vendor2G`, `SISO` | `.NET Web form`, `SQL Server`, `jQuery`, `Jenkins`, `SVN`

##### Links

- https://7-11vcms.pcsc.com.tw

---

### 資深技術顧問 @_鴻揚科技股份有限公司_

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

- http://ecare.fetnet.net/eServiceV3/
- http://ndrs.arcoa.com.tw/NDRS

---

### 資深軟體工程師 @_趨勢科技_

> 十一月 2012 - 十月 2014

- 客製化 Umbraco CMS 供應商等存取權限管控功能
- 開發並維護 Microsoft office sharepoint 內容網站的功能
- 提供其它團隊技術支援

##### Tags

`ishare`, `ishare 2.0`, `ishare 3.0`, `Legal Contract Management system`, `Calendar Synchronization`, `BIF - Report information frontend`, `APAC Sales Kick-off`, `Quarterly IS Awards`, `The circle`, `Olympic 25th` | `Sharepoint`, `C#`, `jQuery`, `Android`

---

### 資訊部副主任 @_上奇科技股份有限公司_

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

---

### 高級工程師 @_超眾科技_

> 五月 2010 - 二月 2012

- 建置生產流程使用的 MES 系統
- 開發鼎新 GP 的工作流程
- 維護 Tiptop 相關的程式
- 維護公司官方網站
- 支援 RD 研發時與 MIS 相關的作業流程
- 支援硬體與網路相關的故障維護

---

### 軟體工程師 @_中華電信政網處_

> 七月 2008 - 五月 2010

- 護電子化政府 - 我的 e 政府相關的服務與模組
- 開發電子化政府與外部系統相關的介接程式
- 以 Worksite MP 開發 KMS 系統

---

### 軟體工程師 @_創世紀資訊_

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

- Github: https://github.com/prhythm, https://github.com/nanashi07
- Web components: https://www.webcomponents.org/author/Prhythm
- Chrome extensions: https://goo.gl/J62Khh
