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