# 加入一筆庫存調整明細

## 第一階段
  - 在現有的 庫存管理->庫存調整單,尚未[確認] 或尚未[審核]
    - 以模擬操作後定案
  - 已有任何物料,包括已經調整為0的
    - 這是為了要取虛擬棧板
  - 直接以外掛方式插入一筆明細
    - 保持現有的[確認][審核]流程
    
## Steps
  - 單頭列表 FrmSTOCK_ADJUSTList.aspx
    - STOCK_CURRENT_ADJUST
  - 單身明細 FrmSTOCK_ADJUSTEdit.aspx
    - STOCK_CURRENT_ADJUST_D
  - 使用現成的單身明細做為模板, 按給定信息加入一筆
    - 可以[確認]
    - [審核]時報錯: 库存调整单明细表中的储位跟库存表中的不一致！2-1

  - 這是因為現有系統有去比對庫存信息
    - STOCK_CURRENT
    - STOCK_CURRENT_SN
    
  - 也就是說要針對加入的物料，也需要去維護上述的兩張表單。
-----
## 基本外掛的功能已實現

<video src="assets/good1.mp4" controls="controls" width="100%" height="auto"/>
