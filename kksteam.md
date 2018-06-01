
### Public opinion Monitoring Workflow
Data collection -> Data Process(NLP) -> Data analysis(怎樣去看數據)

Data Collection : ppt collect forum posr

Data Process : Design ad NER algorithm to detect title names for TV series

NER (wiki)=> information extraction that seeks to locate and classify named entities in text into pre-defined categories such as the names of persons, organizations, locations, expressions of times, quantities, monetary values, percentages, etc.

NER for Drama Title

Google Natural Language API?????
在冷門的領域可能做的不是很好

Many we need to build our NER

String Matching????
王牌大律師 v.s 勝者即是正義 v.s 律政狂人 v.s Legal High
月薪嬌妻 v.s 逃避雖可恥但有用
逃恥 v.s 月薪
逃避可恥但有用 v.s 逃避雖然可恥但有用

Typos??
經常請吃飯的漂亮姊姊 
經常請吃飯的漂亮姐姐 漂亮姊姊經常請吃飯
經常請你吃飯的漂亮姊姊 經常請我吃飯的漂亮姊姊
經常吃飯的漂亮姊姊 請我吃飯的漂亮姊姊
每天請吃飯的漂亮姊姊 請漂亮姊姊吃飯

How to design our NER algorithm?
先靠工人智慧 解決人工智慧的問題
書名號 語言特徵 將整句話的特點HighLignt
image1

Others?
Leverage the useful feature => 嘗試找一些comment 跟title是有相關性的
逃避可恥中的土屋百合 -> google(search) ->(資訊放大) 標題跟小標 -> 用這些將feature找出來 做count 

Something wrong?
Unperfected Example 
but 月薪 will match 工資（wiki）

Wiki is not a perfect entity refetece in out care T_T

Use other resources
利用影評網 dorama  or 豆瓣

Details make things perfect(儘量去除掉垃圾字)

NER Evaluation
Human label ground truth from PPT KoreaDrama board
Total 296 posts in April 2019
Accuracy: 76% (225/296)

 Data analysis
 Trend List
 Time series Analysis
 https://imgur.com/a/0JSCXM2
 (橘色那塊可能時好時壞->討論區的傳統 跟波的討論)

# Summary
 
 Developed a public opinion monitoring sysyem to collection social information

 外部跟內部資料比對 完食率
 Combined them with end-user behavior in KKTV to facilitate decision making for contene team and marketing team

# Refer
1.https://www.bnext.com.tw/article/41346/taiwan-ott
2.https://en.wikipedia.org/wiki/Named-entity_recognition
3.ccClub(Learning python) 行為科學中心