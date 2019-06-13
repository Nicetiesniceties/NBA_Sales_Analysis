# Social Media & NBA sales analysis
## 結果分析:
### 實作一-Reddit數據預測觀眾人數
![image](https://github.com/Nicetiesniceties/NBA_Sales_Analysis/blob/master/social_media/EDA/polynomial%20regression(2018-2019%E7%90%83%E5%AD%A3).png)
#### 1.從這張圖可以看出score(讚數)、comment_num(回文數)與上座率都呈現正相關
#### 2.推論score、comment_num會影響門票銷售，導致上座率變動
![image](picture or gif url)
#### 1.實際跑各種Regression模型後發現預測結果不如預期，準確率只有6%左右
#### 2.可斷定score、comment_num並不足以影響上座率，實際上可能還有很多其他因子會影響上座率
### 實作二-文章情緒分析
![image](picture or gif url)
#### 1.從這張情緒分數分布圖可以看出一整年各隊情緒分數分布大致相同，沒有辦法看出特徵
#### 2.因此我想詳細分析單一球隊(以勇士隊為例)，觀察其一整年情緒分布結果
![image](picture or gif url)
#### 1.可以看出在季賽期間(2018/10~2019/04)情緒分數大致相同，但季後賽期間(2019/05~2019/06)情緒起伏就明顯增大
#### 2.符合認知，在季後賽期間因為賽況緊張，網友情緒起伏大是合理的
![image](picture or gif url)
#### 1.橘色點是球隊輸球的時間點，與情緒低點大致吻合
#### 2.可以推斷影響球迷情緒的主要原因是比賽輸贏
### 實作三-球迷習慣分析
![image](picture or gif url)
![image](picture or gif url)
#### 1.從結果可發現球迷留言的活躍時間約在一天中的21~22點
#### 2.若以一整年的尺度來看，可以發現留言的活躍期約界在2019/05~2019/06(季後賽期間)
#### 3.應用:可以利用球迷留言活躍期進行較多廣告投放或商品推銷
