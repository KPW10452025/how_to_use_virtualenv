# **virtualenv**
虛擬環境可以在任何資料夾下建立，並且同一個資料夾可以建立多個虛擬環境。
* 建立虛擬環境
<br>把 terminal 位置 cd 到想建立虛擬環境的專案資料夾。
<br>在 terminal 輸入 virtualenv 虛擬環境名稱。
<br>舉例：virtualenv testvenv
<br>這樣會建立一個名為 testvenv 的虛擬環境。
<br>專案資料夾會出現一個 testvenv 的資料夾。
* 啟動虛擬環境
<br>在 terminal 輸入 source 虛擬環境名稱/bin/activate
<br>舉例：source testvenv/bin/activate
<br>這樣會啟動方才建立的 testvenv 虛擬環境。
* 關閉虛擬環境
<br>在 terminal 輸入 deactivate
* 刪除虛擬環境
<br>在專案資料夾裡找到和虛擬環境依樣名稱的資料夾，刪除這個資料夾就能刪除此虛擬環境。
<br>本篇的說明例子就是刪除名為 testvenv 的資料夾即可。
* 導出安裝模組 model
<br>在 terminal 輸入 pip list 可以看目前的環境已安裝的模組
<br>在 terminal 輸入 pip freeze > 檔案名稱.txt 可以把目前的環境已安裝的模組導出至此 txt 檔案
<br>舉例：pip freeze > requirements.txt
<br>在 terminal 輸入 cat 導出檔案名稱.txt 可以觀看此 txt 黨的內容
* 導入安裝模組
<br>啟動虛擬環境
<br>在 terminal 輸入 pip install -r 檔案名稱.txt
<br>舉例：pip install -r requirements.txt