# PyCon TW 2018

## from ai.backend import python

Joe / Umbo CV

* CV Worker = Web service + ML model
* Refactor Stream Manager with async/await
* Refactor CV Worker
  * Lua to Python, Torch to PyTorch
  * aiohttp server
* GPU resources are the bottleneck
* Debug: pyflame, tracemaclloc
* ML is not so easy to learn
* Data collection -> Labeling Platform -> Dataset DB -> Training/Test
* Uber Michelangelo
  * [ML Platform] (https://eng.uber.com/michelangelo/)
  * [ML Pipeline] (https://eng.uber.com/tag/michelangelo/)
* Labeling Platform
  * Flask + plugins
  * NumPy
  * Celery/Redis/Pymongo
  * uWSGI
* Visualization Platform
  * Visualize ground truth data and evaluation result
  * Flask + plugin
  * NumPy
  * SQLAlchemy
* a faster pipeline means a shorter turnaround time
* Collaboration with researcher
* Every young engineer knows machine learning
* 2-factor model deploy

## 輿論分析量測電視劇觀看喜好的風向

Kevin / KKStream

* 理論上聲量大的劇收視覺好
  * 上映前默默無名，開播大紅的黑馬
  * 上映前名聲大，開播後大雷
* Data Collection -> Data Process -> Data Analysis
* 從 PTT 韓日台陸劇板收集資料
* Named-entity Recognition
  * 大量別名、使用者 typo
  * 語言特性可以節省很多（書名號）
* leverege useful feature
  * information retrieval 找出重要 content
  * 善用 Google 搜尋、Wikipedia
  * 容易對應到錯誤的資訊，更換 knowledge base
* python-ptt-crawler
* time series analysis
  * 每日單劇總留言佔比
  * 延續話題的能力
* 外部資訊跟平台內部資訊不一定相符

## 自製高擴充性機器學習系統

KK, Richard / Mobagel

* Pandas + Sci-kit Learn
* RapidMiner
* 分析監控 Celery

## 建立知識圖譜

* Ontology
* w2v
* Harmonic Mean (W2V + TF)
* Seq2Seq for TextSum

## Deep Learning for NLP (PyTorch vs Tensorflow)

* no universal definition for emotions
* text-based emotion detection system
* PyTorch vs Tensorflow
  * Dynamic graph vs Static graph
  * Debug: runtime vs special tool
  * Visualization: None vs Tensorboard
  * Deploy: manual vs fast
  * Distrubuted: None vs Yes
  * Data parallelism: easy and hard
* GitHub: NLP-Dataset
* bag of words can't represent sequence
* GloVe, Word2Vec, Tweet-based Word2Vec (CBOW)
* PyTorch is mor native(step-by-step approach)
* Tensorflow just build architect and learn
* 3 LSTM layer

## 運用 Keras 打造遊戲精彩剪輯

* 手機遊戲直播
* 只有 9% 的影片長度會被重播
* 自動剪輯提升兩倍使用者觸及、節省行銷人員時間
* Label
  * 遊戲場景（選角色、載入、死亡）softmax
  * 事件（擊殺、勝負）sigmoid
* SqueezeNet pre-train model
  * 人為判斷結果後迭代
* 將影片分割成每秒一張的圖片
* 優先選擇擊殺畫面（前四秒到後一秒）
* 改進事件偵測（角色、競技賽、畫面英雄密度）
  * 根據玩家選擇的角色技能華麗程度
  * 競技賽較一般比賽精彩
  * 避免出現擊殺訊息但玩家正在發呆，採用畫面英雄密度夠高
* 螢幕錄影導致在遊戲外容易誤判，改為當判斷擊殺訊息持續三秒
* 移植 model 到新遊戲
  * 用原有 model，使用低 learning rate 再次訓練進行「修正」
* 「傳說 MVP 特輯」將每週剪輯經由行銷人員處理後放出，提升一倍觀看
* weakly supervised crowd counting
* 環境包在 docker 內
* 根據自動剪輯與直播的熱絡程度是相符的