# Social Media & NBA sales analysis
## 結果分析:
### 實作一-Reddit數據預測觀眾人數
![image](https://github.com/Nicetiesniceties/NBA_Sales_Analysis/blob/master/social_media/EDA/%E5%90%84%E9%9A%8A%E8%AE%9A%E6%95%B8%E3%80%81%E5%9B%9E%E6%96%87%E6%95%B8%E8%88%87%E4%B8%8A%E5%BA%A7%E7%8E%87%E9%97%9C%E4%BF%82%E5%9C%96(2018-2019%E7%90%83%E5%AD%A3).png)
#### 1.從這張圖可以看出score(讚數)、comment_num(回文數)與上座率都呈現正相關
#### 2.推論score、comment_num會影響門票銷售，導致上座率變動
![image](https://github.com/Nicetiesniceties/NBA_Sales_Analysis/blob/master/social_media/EDA/polynomial%20regression(2018-2019%E7%90%83%E5%AD%A3).png)
#### 1.實際跑各種Regression模型後發現預測結果不如預期，準確率只有6%左右
#### 2.可斷定score、comment_num並不足以影響上座率，實際上可能還有很多其他因子會影響上座率
### 實作二-文章情緒分析
![image](https://github.com/Nicetiesniceties/NBA_Sales_Analysis/blob/master/social_media/EDA/%E5%90%84%E9%9A%8A%E6%83%85%E7%B7%92%E5%88%86%E6%95%B8%E5%88%86%E5%B8%83%E5%9C%96(2018-2019%E7%90%83%E5%AD%A3).png)
#### 1.從這張情緒分數分布圖可以看出一整年各隊情緒分數分布大致相同，沒有辦法看出特徵
#### 2.因此我想詳細分析單一球隊(以勇士隊為例)，觀察其一整年情緒分布結果
![image](https://github.com/Nicetiesniceties/NBA_Sales_Analysis/blob/master/social_media/EDA/%E5%8B%87%E5%A3%AB%E9%9A%8A%E6%83%85%E7%B7%92%E5%88%86%E6%95%B8%E6%8A%98%E7%B7%9A%E5%9C%96(2018-2019%E7%90%83%E5%AD%A3).png)
#### 1.可以看出在季賽期間(2018/10~2019/04)情緒分數大致相同，但季後賽期間(2019/05~2019/06)情緒起伏就明顯增大
#### 2.符合認知，在季後賽期間因為賽況緊張，網友情緒起伏大是合理的
![image](https://github.com/Nicetiesniceties/NBA_Sales_Analysis/blob/master/social_media/EDA/%E5%8B%87%E5%A3%AB%E9%9A%8A%E6%83%85%E7%B7%92%E5%88%86%E6%95%B8%E6%8A%98%E7%B7%9A%E5%9C%96(2018-2019%E7%90%83%E5%AD%A3)%E6%A9%98%E8%89%B2%E9%BB%9E%E7%82%BA%E7%90%83%E9%9A%8A%E8%BC%B8%E7%90%83%E6%99%82%E9%96%93%E9%BB%9E.png)
#### 1.橘色點是球隊輸球的時間點，與情緒低點大致吻合
#### 2.可以推斷影響球迷情緒的主要原因是比賽輸贏
### 實作三-球迷習慣分析
![image](https://github.com/Nicetiesniceties/NBA_Sales_Analysis/blob/master/social_media/EDA/%E5%90%84%E5%80%8B%E6%99%82%E9%96%93%E9%BB%9E%E7%95%99%E8%A8%80%E4%BA%BA%E6%95%B8(%E5%8B%87%E5%A3%AB%E9%9A%8A).png)
![image](https://github.com/Nicetiesniceties/NBA_Sales_Analysis/blob/master/social_media/EDA/%E4%B8%80%E5%B9%B4%E9%96%93%E7%95%99%E8%A8%80%E4%BA%BA%E6%95%B8(%E5%8B%87%E5%A3%AB%E9%9A%8A).png)
#### 1.從結果可發現球迷留言的活躍時間約在一天中的21~22點
#### 2.若以一整年的尺度來看，可以發現留言的活躍期約界在2019/05~2019/06(季後賽期間)
#### 3.應用:可以利用球迷留言活躍期進行較多廣告投放或商品推銷
