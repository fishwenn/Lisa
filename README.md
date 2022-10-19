# Lisa
**計算機概論**

* linux 各個目錄存放的內容              
  * /：根目錄，所有檔案皆從根目錄開始 ，只有root使用者具該目錄的許可權。                           
  * /root ：該目錄為系統管理員，也稱作超級許可權者的使用者主目錄。                      
  * /bin：存放著經常使用的命令。                                  
  * /boot ：系統啟動時必須讀取的檔案，包括系統核心。                             
  * /home ：存放普通使用者的家目錄，每個使用者都有自己的家目錄。                   
  * /etc ：放置與系統設定、管理相關的檔案。                           
  * /usr：這是一個非常重要的目錄，使用者的應用程式和檔案都放在這個目錄下 ，似windows 下的program fil目錄。                      
  * /media：可用來做為光碟片、軟碟片、隨身碟與其他分割區的自動掛載點。                           
  * /tmp：供全部使用者暫時放置檔案的目錄。                                     
  * /var：經常變動的資料或暫存檔(log file)，都會放置在這個目錄。     
---  
**Linux指令**
 * cd：變換目錄  
 * pwd：顯示目前的目錄的所在位置
 * ls：顯示目錄下的所有檔案
 * touch：建立檔案
 * cp：複製
 * cat：查看檔案內容
 * vi：編輯檔案
 * mkdir：建立一個新目錄
 * mkdir -p：同時建立多個目錄
 * rmdir：刪除一個裡面是空的空目錄
 * rm：刪除檔案
 * rm -r：強制刪除
 * mv：移動，重新命名
---  
**Linux指令-壓縮檔案**
 * gzip
   * 壓縮：gzip FileName
   * 解壓縮：gunzip FileName.gz/gzip -d FileName.gz
 * xz
   * 壓縮：xz -z FileName
   * 解壓縮：xz -d FileName.xz
 * tar.gz
   * 壓縮：tar -zcvf FileName.tar.gz DirName
   * 解壓縮：tar -zxvf FileName.tar.gz
  ---  
**Linux指令-檔案搜尋**
 * find 
   * -size EX：找出大於500M的檔案→ -size +500M
   * -name EX：找出為照片的檔案→ -name "*.jpg"
   * -type EX：-type f→ 一般檔案;  -type d→ 一般目錄
   * -user EX：同時找兩個擁有者的檔案→-user user1 -o -user user2
 * find 
   * -a：系統會顯示所有被找到的命令執行檔之完整路徑
   * -n<文件名長度>指定文件名長度，指定的長度必須大於 或等於所有文件中最長的文件名。
   * -p<文件名長度>與-n参數相同，但此處的<文件名長度>包括了文件的路徑
   * -w：指定輸出欄位的寬度。
   * -V：顯示版本訊息。
