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

1. checkout svn latest 
1. open solution to build
  - fix Newtonsoft
    - ASRS.DAL
    - ASRS.Repository
    - ASRS.Business 這時報錯
  - fix log4net
    - WMS.DAL
    - WMS.Repository
    - WMS.Business 這時報錯
  - fix Fakes
    - ExternalService  build時不報錯
      - to del Fakes folder
    - WebWMS.Web debug 時出錯
      
    
    
    
1. change web.config for db and 權限平台 

