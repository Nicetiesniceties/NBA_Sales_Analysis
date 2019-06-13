# NBA_Sales_Analysis
> 目前大概完成了7成到8成的工作量，我們的目標是NBA team 的售票revenue預測與分析。

[PRESENTATION SLIDES](https://drive.google.com/file/d/1EFu6v5GMxRxfOM4N2mKGKZ8rAs9a4qyV/view?usp=sharing)

我們資料分析的大致可以分為：

- Player Performance 的分析 (./player performance/Predicting NBA Player Salary using Player Statistics.ipynb)
- Player Salary的分析 
- Player Social Power的分析 (./social media/)
- NBA ticket Price的分析 (./league tickets price/final_nba 拷貝.ipynb)

大部分的分析與預測結果都有附在上述的`ipynb`檔案裡面，以下會簡述我們的實作過程。

## Player Performance

（完整與其他結果請直接到 `./player performance/Predicting NBA Player Salary using Player Statistics.ipynb` 查看）

首先有對各類的球員data去visualize co-relation。

![Unknown-5](https://github.com/Nicetiesniceties/NBA_Sales_Analysis/blob/master/README%20imgs/Unknown-5.png?raw=true)

並且對幾個特定資料也有做比對與視覺化。

![Unknown-4](https://github.com/Nicetiesniceties/NBA_Sales_Analysis/blob/master/README%20imgs/Unknown-4.png?raw=true)

![Unknown-2](https://github.com/Nicetiesniceties/NBA_Sales_Analysis/blob/master/README%20imgs/Unknown-2.png?raw=true)

最後是採用Elastic net 與 regression的方式去預測球員的薪資與表現。

![Unknown-3](https://github.com/Nicetiesniceties/NBA_Sales_Analysis/blob/master/README%20imgs/Unknown-3.png?raw=true)

## Social Power

Social Power 的部分主要是利用Reddit上的資料來促進銷售最佳化

並會將其中發現的結論以及數據納入進一步模型的考量。

## NBA ticket Price

（同上，細部的作法與其他的結果與視覺化都在`./league tickets price/final_nba 拷貝.ipynb`裡面）

![Unknown-2 copy](https://github.com/Nicetiesniceties/NBA_Sales_Analysis/blob/master/README%20imgs/Unknown-2%20copy.png?raw=true) 

這部分主要是透過各種不同的變量去探討影響票價的因素。

並且用不同的模型去以過往票價預測未來票價，並進行比較，主要評估方式用RMSE：

![Unknown-2 copy 2](https://github.com/Nicetiesniceties/NBA_Sales_Analysis/blob/master/README%20imgs/Unknown-2%20copy%202.png?raw=true)



# 統整上述的結果並預測銷售

（這部分的細節在`./sales/Prediction.ipynb`）

最終我們透過過往票價、上座率、球隊表現與球隊相關的類別資訊做one-hot encoding試著製作了一個NN的模型來預測未來的售票情形，目前的誤差cross validation出來的RMSE誤差在8000多左右，換言之，我們的模型準確率高於90%。

![Unknown](https://github.com/Nicetiesniceties/NBA_Sales_Analysis/blob/master/README%20imgs/Unknown.png?raw=true)

但我們認為這不是最理想的結果，因為NN的實際收斂過程有點太快，目前下一週的目標就是多用不同的模型與手段來預測銷售結果，以越可驗證和越準確為目標。並且將球星的表現部分也納入模型之中。

