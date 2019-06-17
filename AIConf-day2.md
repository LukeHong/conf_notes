# 2017/11/10 人工智慧年會 Day 2


## AlphaGo－深度學習與強化學習的勝利
黃士傑 / Google DeepMind Research Scientist

**人因夢想而偉大**

### 起源
* 重要里程碑
    * 對奕李世乭贏得第一盤
    * 操作 Master 下完 60 盤棋
    * 烏鎮對奕柯潔
    * AlphaGo Zero
* Erica 以單機版擊敗其他叢集版
* 不做 Erica+，極限在業餘三段
* Policy Network 對原始版本 100% 勝率
* Value Network 解決 Overfitting 後對前一代 AlphaGo 95% 勝率(強化學習)
* 科學研究要推動領域的發展

### AlphaGo Lee
* 對奕前發表 Nature 論文
* Google TPU 大量提升 AlphaGo 勝率
* 對奕李世乭的第四盤有嚴重失誤，為全面改善 AlphaGo 的動機

### AlphaGo Master
* AlphaGo Master 由 13 layers 改為 20 layers
* Policy Network, Value Network 結合為 Dual Network
* 改進 Training Pipeline, MCTS
* 單機板 4 TPU 每步思考 4-8 秒
* 上網下棋，每日 10 盤不眠不休
* 野狐第一日職業棋士不願意接受挑戰，第二天主動邀請
* 約第 50 手勝率激增 (柯潔堅持到 60, 70 手)
* 烏鎮對奕氣氛良好，共同探索圍棋機會

### AlphaGo Zero
* 移除所有人類知識
* 訓練三天走過人類千年來為期研究的歷程
* 極大化運算效能（降低功耗）

### 結論
* 深度學習與強化學習的勝利
* 團隊合作力量大
* 硬體資源與 TPU 提供強大協助
* AlphaGo Zero 展現強化學習的巨大潛力
* AI 在未來會成為人類的助力

### 問答
* AlphaGo Zero 目標在於驗證沒有人類知識可到達的極限
* AlphaGo Zero 訓練使用 500 台機器 * 4 TPU = 2000 TPU
* 脫離 **圍棋知識**，保留 **規則知識**
* AlphaGo Lee 的 Bug 在於神經網路的盲點
* 讓同等級的 Zero 不斷自我對奕，同時增強


## CGI and CGI
吳毅成 / 交通大學資訊工程系教授

* 西洋棋不是 AI 的果蠅，圍棋才是
* 象棋難以找到專家協助
* 蒙地卡羅樹大量減少搜尋量
* CNN 無法用於 2048


## The Interplay of Big Data, Machine Learning, and Artificial Intelligence
林軒田 / Appier Chief Data Scientist

### Contract Bridge Bidding by Learning
* 沒有其他人作橋牌
* 從零開始學習

* Big Data(Source), Machine Learning(Technique), Artificial Intelligence(Outcome)
* ML 的服務系統更重要
* 學界研究時常先射箭再畫靶
* 技術不是重點，而是成果
* Big data to ML: domain knowledge
* ML to AI: resource
* Big data to AI: Data Analysis


## 使用少量標記資料訓練聊天機器人的語意模型
朱柏憲 / 優拓資訊 Data Scientist Lead

* 任務導向 Task Oriented Chatbot
* bag-of-words 成果很糟
* word2vev 成果較佳
* Self-Taught Learning，Seq2Seq + DNN 成果驚人（能辨識火星文）
* OpenAI: Unsupervised Sentiment Neuron
* 善用資料潛在的監督式訊息
* character-based 斷詞不會比較差
* Semi-supervised sequence tagging with bidirectional language models(ACL 2017)
* 斷詞需考慮專有名詞


## 大數據情緒分析的經驗分享
陳宜欣 / 清華大學資工系副教授

* 正統: 了解詞性 -> 了解意義 -> 了解字詞關聯、規則
* Twitter 可以很簡單的取得大量資料
* 利用 hashtag 取得使用者的情緒
* 分析中心字、社區字


## 認知神經科學 x人工智慧
黃從仁 / 臺灣大學心理學系助理教授

* 從群眾隱藏的情緒作訓練(Twitter hashtag, Facebook emotion)