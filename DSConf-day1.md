# 2017/11/11 資料科學年會 Day 1

## Big Data Visualization
馬匡六 / University of California at Davis Professor

* 相同的統計屬性，經過視覺化可能有完全不同的樣貌
* 視覺化是很好的 UI，易於操作、搜尋、分享
* 根據視覺化目標的使用者的不同，有著不同的呈現內容
* 視覺化的結果可提供決策的參考


## 重新認識資料視覺化
王昱舜 / 交通大學資訊工程系副教授

* 視覺化很有趣，但不一定實用
* 簡化的圖可能比實際地圖更容易讓使用者閱讀
* 一般的視覺化可能有現有工具可使用，可以快速產出
* 專家的視覺化可能沒有過去經驗可以參考，需花費較大量的時間設計
* 先找到專家進行訪談，了解需求才作開發


## 製造資料？科學？！
李家岩 / 成功大學製造資訊與系統研究所工作者

* 製造與服務的差異在於庫存
* 看到資料應能對應到現場問題
* 使用零組件推估現場狀況
* 收集現場資料之外，還要加上製造資料
* 預測與決策時，需考慮損失風險
* Prescriptive Analysis 要能提供決策所用，而非只是預測分析


## The Journey To Become A Data Scientist－From School To Industry
周曼如 / Oath APAC Data Team Senior Data Engineer

### 學習 Data Science Flow
* 學習 Machine Learning, Data Mining, Statistic
* 觀察 Raw Log 以後透過 Feature Engineering 設計模型
* Feature Selection

### 了解不同的 Domain Knowledge
* 從不同 team 需求的處理不同的 data
* Domain Knowledge 是理解 data 最重要的部分
* 從專家處學習

### Data Quality 的重要性
* 把雜亂的資料經過 ETL 整理
* Data Flow Design: 模組化、Schema、修復過去資料、效能
* 資料可靠性
* 持續監控

### 設計 Data Product 的問題
* 問題不一定來自 Model，可能來自 UX

### 
* 如何問一個好的 Data Science 問題
* 系統 + Data 才有力量
* 足夠好的系統比完美的系統有用


## 資料科學在國泰
陳榮錡 / 國泰金控資料科學實驗室 資料科學家

* 資料來源: 帳戶、理財、保險、信貸
* 各家公司資料格式不一、各有特色，前處理、人工成本過高
* 資料格式系統化、被動執行
* 藉由統一化的資料，提升客服的用戶體驗
* 設計檢查資料源是否就緒的機制
* 總和成一種響應式、模組化、系統監控 -> 微服務、被動式、水平架構
* 流程獨立、模組化
* 主動呼叫傳遞改為被動式訂閱驅動
* Service 分成四個階段
    * Frontier: 檢查前端資料是否就緒
    * Batch-ETL: 轉換客戶歷程
    * DB-ETL: 將客戶歷程存放到 DB
    * Query: 提供後續數據使用
* 使用大量 OpenSource Library(Hadoop, Kafka, Spark...)
* 建立客群網路，使用者之間的關聯
* 客群尋找機制，過去一月內購買旅遊商品的人(機票、海外住宿、旅行支票)
    * 有無旅遊意願人數比 10071:67014
    * 有旅遊意圖人群中 43.2% 購買旅遊商品，反之只有 12%
* 大型集團有更多樣化的資料
* 資料科學不應該是偵探式的尋找資料，應建立更全面性的系統

## KKBOX 上的個人化推薦系統
陳怡安 / KKBOX Machine Learning Researcher

* 以推薦系統增加客戶黏著度
* 藝人本身的轉變可能帶來較差的推薦效果
* 曲風本身定位不明，且年代流行不同
* 使用者本身有不同情境
* 完全準確的推薦系統無法擴展使用者興趣，只是最低要求
* Collaborative Filtering 在 Cold Start 會有問題
* 採用 Reinforcement Learning
* LSH 減少 k-NN 的工作
* 用頻率域上透過 NN 辨識子曲風(Spotify Paper)
* 跟專家共同確認子曲風的定義
* 將歌詞分類意境