# 新增需求
## 1. PDA



## 2. 庫存調整

### Requirement

1. 針對儲位中放錯料號的情境: 將錯誤料號歸0並新增正確料號
1. 針對T01現場人員有可能手動操作地上盤入庫的情境: 是否能直接新增料號與數量到指定儲位?

### TODO

1. 在現有基礎上, 允許數量調為0
2. 允許新加物料到指定儲位.


### Steps

#### 1. checkout svn latest 
#### 2. open solution to build
  - ASRS.DAL
  - ASRS.Repository
  - ASRS.Business 這時報錯     fix Newtonsoft
  - WMS.DAL
  - WMS.Repository
  - WMS.Business 這時報錯      fix log4net
  - ExternalService  build時不報錯 to del Fakes folder  
#### 3. change web.config for db and 權限平台 
#### 4. debug to run on vs2019
#### 5. 庫存調整時, 可以設為0, 但在[確認]時彈出錯誤信息
  - 儲位[01-0102105]不能沒有庫存
  - FrmSTOCK_ADJUSTList.aspx
  - btnConfirm_Click
  - listQuery.CanStockDoAction(id, "1");
  - SELECT dbo.Fun_IsAllowAction('{0}','{1}')", id, flag
  - [Fun_IsAllowAction](./Fun_IsAllowAction)

