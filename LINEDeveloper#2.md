# 20180309 Line developer meetup

## 談 LINE 福岡 DataLabs 的資料工程：一個新人的觀點/ Liangchi Hsieh

* Azkaban scheduling tool
* Running Kafka/DBs/ES and Hadoop cluster
* Line stick automatical tagging
* Learning Japanese is part of job

## 機器學習在LINE福岡的各種應用/ Wenchun Kao

* Data Labs - Machine Learning Engineer
* 提供分析技術、API 等
* 由 Data Team 串連各個服務，提供跨服務的分析
* Data Labs 由 Planner, Data Scientist, Engineer 組成 (福岡無 Planner)
* Spam Filter (ML, Keyword, Rules)
* Monitoring Platform (for developer, mod)
* Customer Service Automation
  * Japanese text classification task
  * 維護日文詞庫
* ML System
  * Data Management
    * Data Versioning(ETL, New Data, etc.)
    * Feature Versioning/Sharing
  * Experiment Management
    * Model Performance Comparison
    * Computation Resource Allocation
  * API/Model Management
    * Monitoring
    * Developing
* Open Source ML Deployment Tool
  * K8s, GRPC, Python
  * 管理、切換 Model

## Building a company-wide data pipeline on Apache Kafka - engineering for 150 billion messages per day/ Yuto Kawamura

* 200M+ MAU
* 25B messages a day, 80B API calls a day
* 40 PB accumulated data(for analysis)
* client -> LEGY server(JP, DE, SG...) -> talk-server
* LINE Event Delivery Gateway (LEGY)
  * API Gateway/Reverse Proxy
  * Write in Erlang
  * Zero latency code hot swapping w/o closing client connection
* talk-server
  * Java based web application
* Hybrid datastore
  * Redis (home-brew cluster)
  * HBase
  * Cascading faulure handling
    * Async write from background
    * Data correction batch per day
* Kafka 150B messages per day (3M per sec)
* Usages sensitive for delivery latency
* Broker's latency impact throughput
  * kafka is a queue
* contribute it back (kafka)
* Kafka Summit SF 2017

## 在 LINE NOW docker 化系統架構中的測試/ Johnny Wu

* 將環境盡可能 container 化
* 使用 Rancher 管理 cluster