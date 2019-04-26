# Youbike 畢業專題

:point_right: 探討Youbike空位數，結合各種可能影響Youbike空位數的因素，打造出for管理者的Youbike多維度戰情系統

### 動機：

目前台北市的**Youbike站點有400個**，**車輛數有一萬多輛**，站在管理者的角度來看，想要知道 **｢空位數｣的變化狀況**是一件不容易的事，以往需要管理者告訴IT人員想要知道的或是提出問題，IT人員在進行查詢後把結果告訴管理者，是沒有效率的。於是如何能夠**節省查詢時間**，又能夠讓管理者能自行**簡單且方便的操作**，是我們想要做的。

### 目的：

針對**YOUBIKE車輛的｢空位數｣**，以簡單的管理者可能**提出的問題**為例，結合**原始資料**和我們額外的**維度設計**，使用POWER BI以**圖表化方式呈現**，得到空位數的變化，輔助管理者做分析，提高作業效率。
>期許本研究能解決下列問題：
* 減少查詢時間：
	* 對於IT人員來說，每當**管理者提出一次問題**，IT人員就**必須下一次查詢**，而且萬一資料量過多，**花費的時間也會過多**，實在**不符合效益**。
* 以圖表化呈現，管理者可以簡單自行操作：
	* 對於管理者來說，每次都要等待IT人員查詢，而且得到的結果也不易觀看，管理者如果可以自己操作，自由度就大幅提升，時間方面也能減少，圖表化的形式也可以更人性化的觀看。

### 目標：

若能完成這套YOUBIKE多維度戰情系統，將其應用在公司上，將可以**有效節省管理者查詢時間**並能從**不同面向瞭解空位數的變化**，使公司在營運管理上有一套**方便有效率**、且符合管理者需求及公司需求的系統，**為管理者提供決策支援。**
>期許本研究能達到下列目標：
* 結合各種**可能影響空位數變化**的因素：
	* 一般只是看空位數的變化，如果結合各項因素來觀察，例如**天氣、道路、紫外線等情況**，可以發現到不同的空位數變化，對於管理者來說這有可能是他會想知道的。
* 管理者可以了解營運狀況：
	* 經由**多維度的方式**進行查詢，可以**從不同面向查詢空位數**，管理者可以從想知道的問題去下查詢，從根本直接查詢能更清楚的得到空位數。
* 提升公司營運績效：
	* 綜合以上因素，**YOUBIKE多維度戰情系統**可以提供給管理者很好的**決策支援**，支援管理者下決策，做出對公司**最好的決策方向。**

### 結論與未來展望：

* 整個專題從**資料抓取**、**建立維度模型**、**資料整理**到最後的**圖表呈現**，最耗時費工的便是**資料整理**，而最關鍵的便是**維度模型的建立**，有了維度模型我們才能運用抓取的資料，呈現出**視覺化的圖表**。

* 透過Power BI 圖表呈現，我們發現**雨量、鄰近學校、或捷運站**等屬性對**空位數影響較大**，**紫外線**等部分屬性**影響較小**，如果沒有前面那些資料的轉換，用**原始資料是看不出直觀的空位數變化的。**

* 在圖表當中我們會去猜想說會不會是什麼樣的原因造成，這**都是假設**，至於說確不確定、是不是？**決策者自己判斷**，決策者看到這個圖之後會自己去猜想，可能是這樣，可能是那樣？我們提供給他這些圖表、這些決策支援，**不提供的話決策者無法有這種猜想**，但是是不是我們猜想的原因？最後還是要**跑統計模型**才行，所以我們把本來是**密密麻麻的數字**變得很生動很有趣而且**一目了然的圖表**，讓別人一眼看就知道，這樣子就做到**很好的決策支援。**

* 我們發想的情境以及假設皆是建立在我們**現有的維度模型還有原始資料上**，透過不同維度的交叉比對以及完整的原始資料得到更豐富更細緻的圖表，而這次專題因為在**政府的Youbike open data**中**沒有詳細的借還數量**，所以我們能研究的情境被限制許多，得出的假設也比較模糊，所以管理者想要了解更全面、更深入的問題，便需要**更多維度屬性以及相應的原始資料**才能繪製出圖表。

* 透過圖表我們能直觀的看出空位數變化，並提出假設，給予決策支援，讓管理者以自身經驗以及圖表顯示的資訊做出適當的決策，但為了讓我們的決策支援更有力，未來我們也可以讓我們蒐集到的原始資料**透過統計工具**來看**資料的顯著情形來證實假設**，以輔助決策者做決策。

### 心得：

* 在專題當中花費最多時間的不是建置維度屬性表而是**事實表的整理**，從最一開始能夠**穩定蒐集原始資料、進行資料清理、針對龐大的資料庫做維護**等等，確實有許多當初沒有想到導致後來需要花大量時間修改補救很多地方，像是事實表中要新增維度表的FK、開放資料網站改版使得爬蟲失效、雨量原始資料有誤、甚至是道路速率抓錯資料來源，導致最後整個原始資料無法使用，**只要錯誤發現的越晚，就越難補救**，除了從爬蟲程式碼修改來抓正確的來源資料，先前所有儲存在資料庫的資料也要一併修改，也就是從頭到尾都要更動，這是非常曠日廢時的。

* 這些經驗都在告訴我們在**取用原始資料時要很小心翼翼，對方所發布的資料不見得是百分之百正確**，要透過程式或工具來**觀察它的資料特徵**、它的**內容、一致性、結構**，測試說是否符合我們的需求來**評估要不要取用**，如果要用的話會有多少問題是需要解決的，**在使用或是在資料清理的過程中也要格外細心。**
