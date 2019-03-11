# proc

## PRO*C練習一

一.<br/>
  程式名稱:s01001b.pc<br/>
  參數:s01001b 批號 form 單位ID起 單位ID迄 設定日期(YYYYMMDD)<br/>
  作業:<br/>
    1.從U01T_UNITFILE(單位資料檔)中讀取作業日期(PROC_DATE)欄位範圍依所輸入的參數(單位ID起迄)<br/>
    2.若作業日期小於參數的設定日期。將作業日期Update成參數的設定日期<br/>


## PRO*C練習二

一.<br/>
  程式名稱:s01002r.pc<br/>
  參數:s01002r 批號 form 印表機 處理局別 單位ID起 單位ID迄<br/>
  作業:<br/>
    1.從U01T_UNITFILE(單位資料檔)中讀取欄位<br/>
單位代號(UNIT_ID)<br/>
單位名稱(UNIT_NAME)<br/>
連絡人姓名(WORK_NAME)<br/>
作業日期(PROC_DATE)<br/>
範圍依所輸入的參數(單位ID起迄)<br/>
    2.依格式印出報表<br/>
    3.請依照各局別分頁列印<br/>


## PRO*C練習三

一.<br/>
  程式名稱:s01003r.pc<br/>
  參數:s01003r 批號 form 印表機 局別 單位ID起 單位ID迄 被保險人ID<br/>
       被保險人ID可輸可不輸(亦即不輸時可以NHI_NULL代替)<br/>
作業:<br/>
    1.從U01T_UNITFILE(單位資料檔)中讀取欄位<br/>
單位代號(UNIT_ID)<br/>
單位名稱(UNIT_NAME)<br/>
範圍依所輸入的參數(單位ID起迄)<br/>
    2.再依據單位代號(UNIT_ID)找出該單位所有人員投保資料(U02T_INSCUR 目前投保資料檔)與其姓名(資料在U02T_ASBAS 保險對象基本資料檔)<br/>
      從U02T_INSCUR(目前投保資料檔)中讀取欄位如下<br/>
        保險對象ID(AS_NHI_ID)<br/>
        被保險人ID(INS_NHI_ID)<br/>
        投保日期(IN_DATE)<br/>
        投保金額(INS_AMT)<br/>
        投保狀態(STATUS)<br/>
      從U02T_ASBAS(保險對象基本資料檔)中讀取欄位如下<br/>
        姓名(NAME)<br/>
    3.依格式印出報表<br/>






列印時間:          計 nn 頁



