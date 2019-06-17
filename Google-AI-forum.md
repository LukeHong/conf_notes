# 2018-03-21 Google 人工智慧論壇

## AlphaGo 與 AI 的黃金時代 / Aja Huang

* 熱情是驅動向前的動力
* 深度學習帶來巨幅的進步
* 團隊包含各個領域的專家合作（圍棋、分散式系統、ML）
* 硬體資源很重要（AlphaGo Zero 使用 500台機器*4顆 TPU）
* 建議
  * 數學不可怕，基礎數學能力越紮實對於調整模型更有用
  * 實驗、實驗、實驗，很多東西不是靠理論就能得到好結果，時常要實驗後回推原因
  * 閱讀新論文跟新理論
* 星海爭霸 AI
  * 對 AI 來說變化太複雜
  * 需要只依靠畫面或 feature 來做決策
* AlphaGo 對李世石第二局第 37 手是超越人類圍棋知識的一手

## 紀懷心

* Nothing tends so much to the advancement of knowledge as the application of a new instrument
* 棋局是 closed system，而推薦系統是 opened system
* Measure, Optimize, Impact
* 語言是減少 Isolation 的關鍵
* Twitter 葡萄牙文佔 9.6%，源自於巴西人對 SNS 的熱愛
* G+ 翻譯最大來源語言是日文與英文
* Recommandation Problem
  * f(User, Context) = Item
  * Shifting User Preferences, Sparse Feedback
  * Dynamic and Changing Contexts
  * Noisy & Sparse Labels, Large Changing item set
  * Low latency with a huge corpus of users and items
* impression -> consume -> like -> query -> impression (Recommendation)
  * recommendation -> like -> query -> consume -> comment -> dislike
* RNN Model with Time [Beutel et al., WSDM 2018]
  * add time spend and time delta
  * Latent Cross as Attention Mechanism
* Long-Term Impact
* User-Item matrix erase context
* Recommender quality inconsistent across genre
* A model that predicts well for all users and all items
  * Focus Selection: Bussiness dicition
  * Focus Learning: Choose model based on focused group(Validation set)
* "Globally optimal" is not best for everybody.
* Understand and Measure what you are optimizing for
* Optimization in real world is complex

## Speech and Language Processing /

* sentence similarity
  * accroding to response
* use conversation data to train embedding (reddit)
* improve 30% recall @80% percision
* smart reply
  * 3 suggestion buttons
* Measure 'suggest conversion', % of times shown suggestions are clicked
* Latency is important: use dot product, approxim search
* No ML model is perfect, small UX change can be big (3% impove)
* one of the most exciting areas in AI
* Used to build and improve many products affecting user daily life
