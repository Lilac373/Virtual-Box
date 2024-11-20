## For QGIS ver (QGIS-OSGeo4W-3.34.12-1) Install guide

用的虛擬機環境檔名 Win10_64_CHT_START_v20241022a.ova

QGIS安裝好 (打開非custom的那個)

打開可能會出現SSL憑證問題 > 按忽略

關閉 > 按丟棄 > 重開QGIS (若在添加WMTS時跑出SSL交握失敗可執行丟棄重開)

左邊列表選到 XYZ Tiles > 添加OpenStreetMap圖層(添加完要打勾才會顯示) > 找到台灣放大 (記得放大的時候要慢 否則畫面會變白色的)

WMS / WMTS 右鍵 New connection ... > 開啟網頁搜索 wmts 到這個網頁(https://www.nlsc.gov.tw/NLSC_Content.aspx?n=11987&s=183225)

然後複製(http://maps.nlsc.gov.tw/S_Maps/wmts) (或是直接複製這個網址(http://maps.nlsc.gov.tw/S_Maps/wmts)

填上

name : nlsc 

url :http://maps.nlsc.gov.tw/S_Maps/wmts

按確定 (解析度問題可能看不到確定，可以直接按ENTER)

點開nlsc > 添加正射影像(通用)圖層並打勾 (同時OpenStreetMap圖層 打勾)

記得先放大完OpenStreetMap再開正射影像圖(通用) 且 圖層順序 正射影像圖(通用)在OpenStreetMap上面

正常顯示影像 > 完成!

這軟體超破，有問題一律儲存重開 或是 丟棄重開 (丟棄重開=重新上面的步驟)
