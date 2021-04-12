## 部署基本
1. IIS的目錄指向這個Publish
2. 要維護 appsettings.json 裡的 connection string
3. 要有DHDB 第一版數據庫(另外發佈)
4. 要有SQL Script做基本初值設置


## 開發測試階段 
- 早上Build : 每天 11 AM  --- 部署人員應即部署測試
- 下午Build : 每天  4 PM  --- 部署人員應即部署測試
- 晚間Build : 如有加班    --- 部署人員於隔日早上開工時,部署測試


