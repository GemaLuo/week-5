# week-5
* **要求三**
  * 1.使⽤ INSERT 指令新增⼀筆資料到 member 資料表中，這筆資料的 username 和 password 欄位必須是 test。接著繼續新增⾄少 4 筆隨意的資料。
  ![IMAGE](https://github.com/GemaLuo/week-5/blob/main/%E8%A6%81%E6%B1%82%E4%B8%89-1.png)
  * 2.使⽤ SELECT 指令取得所有在 member 資料表中的會員資料。
  ![IMAGE](https://github.com/GemaLuo/week-5/blob/main/%E8%A6%81%E6%B1%82%E4%B8%89-2.png)
  * 3.使⽤ SELECT 指令取得所有在 member 資料表中的會員資料，並按照 time 欄位，由近到遠排序。
  ![IMAGE](https://github.com/GemaLuo/week-5/blob/main/%E8%A6%81%E6%B1%82%E4%B8%89-3.png)
  * 4.使⽤ SELECT 指令取得 member 資料表中第 2 ~ 4 共三筆資料，並按照 time 欄位，由近到遠排序。**( 並非編號 2、3、4 的資料，⽽是排序後的第 2 ~ 4 筆資料 )**
  ![IMAGE](https://github.com/GemaLuo/week-5/blob/main/%E8%A6%81%E6%B1%82%E4%B8%89-4.png)
  * 5.使⽤ SELECT 指令取得欄位 username 是 test 的會員資料。
  ![IMAGE](https://github.com/GemaLuo/week-5/blob/main/%E8%A6%81%E6%B1%82%E4%B8%89-5.png)
  * 6.使⽤ SELECT 指令取得欄位 username 是 test、且欄位 password 也是 test 的資料。
  ![IMAGE](https://github.com/GemaLuo/week-5/blob/main/%E8%A6%81%E6%B1%82%E4%B8%89-6.png)
  * 7.使⽤ UPDATE 指令更新欄位 username 是 test 的會員資料，將資料中的 name 欄位改成 test2。
  ![IMAGE](https://github.com/GemaLuo/week-5/blob/main/%E8%A6%81%E6%B1%82%E4%B8%89-7.png)
 
--------
  \***新增follower_count\***
  ![IMAGE](https://github.com/GemaLuo/week-5/blob/main/%E8%A6%81%E6%B1%82%E5%9B%9B-%E6%96%B0%E5%A2%9E%E8%BF%BD%E8%B9%A4%E6%95%B8.png)
***
* **要求四**
  * 1.取得 member 資料表中，總共有幾筆資料 ( 幾位會員 )。
  ![IMAGE](https://github.com/GemaLuo/week-5/blob/main/%E8%A6%81%E6%B1%82%E5%9B%9B-1.png)
  * 2.取得 member 資料表中，所有會員 follower_count 欄位的總和。
  ![IMAGE](https://github.com/GemaLuo/week-5/blob/main/%E8%A6%81%E6%B1%82%E5%9B%9B-2.png)
  * 3.取得 member 資料表中，所有會員 follower_count 欄位的平均數。
  ![IMAGE](https://github.com/GemaLuo/week-5/blob/main/%E8%A6%81%E6%B1%82%E5%9B%9B-3.png)
  
***
* **要求五**
  * 1.使⽤ SELECT 搭配 JOIN 語法，取得所有留⾔，結果須包含留⾔者會員的姓名。
  ![IMAGE](https://github.com/GemaLuo/week-5/blob/main/%E8%A6%81%E6%B1%82%E4%BA%94-1.png)
 
  * 2.使⽤ SELECT 搭配 JOIN 語法，取得 member 資料表中欄位 username 是 test 的所有留⾔，資料中須包含留⾔者會員的姓名。
  ![IMAGE](https://github.com/GemaLuo/week-5/blob/main/%E8%A6%81%E6%B1%82%E4%BA%94-2.png)
  
  * 3.使⽤ SELECT、SQL Aggregate Functions 搭配 JOIN 語法，取得 member 資料表中欄位 username 是 test 的所有留⾔平均按讚數。
  ![IMAGE](https://github.com/GemaLuo/week-5/blob/main/%E8%A6%81%E6%B1%82%E4%BA%94-3.png)
  
***
* **延伸作業**
   > 1.新增message
   <img src="https://github.com/GemaLuo/week-5/blob/main/%E5%BB%B6%E4%BC%B8%E4%BD%9C%E6%A5%AD/%E6%96%B0%E5%A2%9Emessage.png" />
* 註:like_record的member_id=member表的id，like_record的msg_liked=message表的id
   > 2.建立按讚紀錄表格
   >> 若僅將member_id設為主鍵，在msg_liked設定UNIQUE(數據不重複插入)會使留言無法被其他人按讚且會員只能按一個留言的讚
   >>> 使用[複合主鍵](https://www.796t.com/content/1544850548.html)，保持紀錄的唯一性，則每位會員都能按不同留言的讚各一次(不能重複按讚)
   <img src="https://github.com/GemaLuo/week-5/blob/main/%E5%BB%B6%E4%BC%B8%E4%BD%9C%E6%A5%AD/1_%E5%BB%BA%E7%AB%8B%E6%8C%89%E8%AE%9A%E7%B4%80%E9%8C%84%E8%A1%A8%E6%A0%BC.png" />
  
   > 3.插入按讚會員與被按讚留言的id
   <img src="https://github.com/GemaLuo/week-5/blob/main/%E5%BB%B6%E4%BC%B8%E4%BD%9C%E6%A5%AD/2_%E6%8F%92%E5%85%A5%E6%8C%89%E8%AE%9A%E6%9C%83%E5%93%A1%E8%88%87%E8%A2%AB%E6%8C%89%E8%AE%9A%E7%95%99%E8%A8%80%E7%9A%84%E8%B3%87%E8%A8%8A.png" />
   
   > 4.取得按留言讚的會員名稱及被按讚的留言內容
   <img src="https://github.com/GemaLuo/week-5/blob/main/%E5%BB%B6%E4%BC%B8%E4%BD%9C%E6%A5%AD/3_%E5%8F%96%E5%BE%97%E6%8C%89%E7%95%99%E8%A8%80%E8%AE%9A%E7%9A%84%E6%9C%83%E5%93%A1%E8%88%87%E8%A2%AB%E6%8C%89%E8%AE%9A%E7%9A%84%E7%95%99%E8%A8%80.png" />
   
   > 5.使用留言msg_liked的編號(亦即member表格的id)取得按讚會員的name
   >> 使用[巢狀搜尋](https://www.gushiciku.cn/pl/gzwb/zh-tw>IN)，用like_record表格(子查詢)中的留言msg_liked編號取得member_id(等於member表格的id)(先執行子查詢=最內層)
   >>> 再利用member的id取得按讚的會員
   <img src="https://github.com/GemaLuo/week-5/blob/main/%E5%BB%B6%E4%BC%B8%E4%BD%9C%E6%A5%AD/4_%E7%94%A8msg_liked%E5%8F%96%E5%BE%97%E6%8C%89%E8%AE%9A%E6%9C%83%E5%93%A1%E5%90%8D%E7%A8%B1.png" />
