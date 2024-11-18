
### 灌完虛擬機通常要做的事 for Virtual Box ver 6.1.38 

## 步驟 1 VBoxWindowsAdditions.exe
> 在裝置 >插入Guest additions CD 映像... 

插入完會出現 CD光碟機 VirtualBox Guest additions

在VirtualBox Guest additions 中 

會看到三個VBoxWindowsAdditions.exe 三個猜一個

通常選檔案最小的那個安裝(若知道自己電腦什麼位元數可以自己選裝哪個)

這步驟類似安裝驅動 要裝了才有很多功能 ( 裝完必須重啟虛擬機 )

 > 裝完可退出 Guest additions CD 映像...

 > 安裝完在 檢視 > 自動調整客體大小 (打勾) 默認應該是勾的 (會自己幫你隨視窗大小調整虛擬機螢幕大小)

## 步驟 2 基礎設定
> 在裝置 > 共用剪貼簿 > 雙向 > 拖放 > 雙向 (方便在虛擬機和外部之間操作)

## 步驟 3 共用資料夾製作 (可做可不做，用的是絕對路徑，若在別台電腦上的絕對路徑不同則無法使用)

 > 在管理虛擬機頁面 > 右鍵欲修改的虛擬機 > 在檔案總管中顯示 > 

 > 建立一個資料夾(名稱和位置可自訂) > 再來回到管理虛擬機頁面選中該虛擬機 > 設定

 > 共用資料夾 > 加入共用資料夾 (有個加號的小圖示) > 貼上資料夾路徑 (絕對路徑)

 > 唯讀不勾(不然不能寫東西進去) > 自動掛載 (打勾) > 按確定完虛擬機裡就會出現設定的資料夾(能和本機共用)

## 步驟 4 基本設定 (非絕對但需要留意) (虛擬機關機時才能改)

 > 在管理虛擬機頁面 > 選中欲修改的虛擬機 > 設定 > 系統 > 主機板 > 基本記憶體 通常會拉到 4GB (4096MB) (視電腦效能或是需求)

 > 處理器 > 處理器通常會給到 2 ~ 4 若需要更多效能可以拉更多給它 (匯出時通常拉到2 怕換電腦效能不夠 匯入跑不動)

 > 顯示 > 視訊記憶體 拉滿 (不要省 就是拉滿) > 圖形控制器(三選一) 看作業系統改 Windows通常VboxSVGA

 > 3D加速 6.1.38 版的虛擬機通常 不開 (畫面會變透明)

## 步驟 5 其他事項

# 如何在虛擬機插入 USB ?

 > 管理虛擬機頁面 > 選中欲修改的虛擬機 > 設定 > USB > 啟用USB控制器 1.1 幾.幾 跟傳輸速度有關 視需要安裝外掛

 > 開啟虛擬機 > 執行介面右下角 (預設) 通常會有USB小圖示 > 右鍵小圖示 > 選中欲讀取的USB > 在虛擬機中出現 


# .vdi檔?

> 在管理虛擬機頁面 > 選中欲修改的虛擬機 > 右鍵在檔案總管中顯示 > 可以看到.vdi檔
  vdi檔相當於電腦的硬碟，也就是虛擬機的硬碟，妥善保存。


# 拖放和共用檔案時注意事項?

> 拖放必須精準且小心，否則容易當機。
當機時 : 縮放視窗大小，不行的話重開機。
共用檔案時請注意不要虛擬機開檔案，本機又開檔案，易出問題。
