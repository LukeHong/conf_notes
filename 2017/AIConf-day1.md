# 2017/11/09 人工智慧年會 Day 1


## Taiwan's Opportunities in the AI-First World
簡立峰 / Google Taiwan 董事總經理

**空話**

## Optimizing for User Experience with Data Science and Machine Learning
紀懷新 / Google Research Scientist

**Measure, Optimize, Impact**

產品面貌源自於系統設計

### Recommendation
* 早晚會有不同的興趣
* 用 RNN 作 sequential recommendation
* WSDM 2018 發 paper
* Attention Mechanism
* 相同的 Loss function 在不同情境會有不同量級的差異
* Focus Learning(A Model for all users and all items)
* model 要有 regularization 或 dropout
* focus alpha and unfocus alpha for transfer learning
* Understanding and Measuring what you are optimizing for.
    * Optimization in the real world is hard.
* Intuition 未必正確，可能導至錯誤的 Measurement


## Recent advances of deep learning in Google
邱中鎮 / Google Brain Software Engineer

* NIPS 2017 報名大爆炸
* ResNet 給的啟發
* 由 Network 自行設計 Network，於 Imagenet 結果完勝人類
* Sequence-to-sequence with attention
* Transformer: autoregressive attention without RNN
* Non-ML Solution in production

## Representation Learning on Big and Small Data
張智威 (Edward Y. Chang) / HTC Research & Healthcare President

* No accuracy for search ranking and ad matching
* Different result in different level of data
* Deep CNN model fail for lack of data in past 
    * AlexNet: 300k+ parameters
* Big data is required


## 不視而見的智慧
陳煥宗 / 清華大學副教授

* Detecting Nonexostent Pedestrians
* Auto-encoder, WGAN
* 那邊最可能出現行人


## 從雛形到千台連網相機的挑戰
吳亭範 / Umbo Computer Vision 科學家

* 訓練資料與監視器實際環境相差過多
* Labeling 是問題
* domain adaptation


## Deep Learning for Computational Photography
莊永裕 / 台灣大學資訊工程系教授

* 堅守傳統研究方式 vs 不知廉恥的擁抱深度學習
* 是否用計算攝影學修正照片場景的不完美
* sRGB space: 8 bits, RAW: 12 bits
* 使用深度學習設計不同的感光元件排列
* 使用一個 Network 取代 12 道 Image signal processing 程序


## 影音大數據商機挖掘
陳彥呈 / Viscovery VP of R&D

* 雷聲大雨點小
* 好的內容不限於原生內容，好的聚合與推薦同樣有價值
* 好的內容推薦能大幅提升用戶
* 從簡單的推薦開始
* 高維度帶來的詛咒
