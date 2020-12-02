---
layout: default
---
# 討論與決策

## 開發工具
- 是否有計畫升級開發工具?
  - 台北直接使用VS2019,SZ仍使用VS2012。

## 版本控制
- 持續使用 svn 或是改用 git?
- 服務器所在位置或租用服務?


## WMS頁面應用
- 是否有計畫升級WMS頁面應用開發的底層框架?
- 已知規格和限制
  - 使用 WebForm, 參考[微軟官網](https://docs.microsoft.com/zh-tw/aspnet/web-forms/what-is-web-forms)。
  - 是否升級改用的考慮, 參考[微軟官網](https://docs.microsoft.com/zh-tw/dotnet/architecture/blazor-for-web-forms-developers/migration)。


## 數據庫開發
- (台北目前無此顧慮)
- 已知規格和限制
- 是否升級現有 EF6 為 EF Core 的考慮,參考[微軟官網]([https://docs.microsoft.com/zh-tw/ef/efcore-and-ef6/)。


## 權限平台
- 是否有計畫升級權限平台的機制和功能?

## WebPDA
- 是否有計畫升級目前的安卓應用的技術框架?
- 已知規格和限制
  - 使用 WebView, 參考[微軟官網](https://developer.android.com/reference/android/webkit/WebView)。
  - 可以快速使用現有WEBPDA部署的網站,好像是安卓手機或PDA的應用。
    - PDA可以硬件操作啟用掃碼功能。
    - 手機無法啟用掃碼功能。必需在類似原生代碼的方式加入啟用照相功能才能掃碼。
