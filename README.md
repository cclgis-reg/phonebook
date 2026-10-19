# 電話簿 APK 打包步驟

1. 到 https://github.com 登入(沒有帳號就免費註冊),按右上角「+」→「New repository」,名稱隨意(例如 phonebook),建立後進入該儲存庫。
2. 按「uploading an existing file」,把這個資料夾解壓縮後的「所有內容」(含隱藏資料夾 .github)拖進去,按 Commit。
   - 注意:.github/workflows/build.yml 必須保留,否則不會自動打包。
3. 點上方「Actions」分頁,等「Build APK」跑完(約 3~5 分鐘,出現綠色勾勾)。
   - 若沒自動執行:左側點「Build APK」→「Run workflow」。
4. 點進該次執行,最下方「Artifacts」下載 phonebook-apk,解壓縮後得到 app-debug.apk,傳到手機安裝(需允許「安裝未知來源應用程式」)。

之後要改畫面,只要替換 www/index.html 再 Commit,就會重新打包。
