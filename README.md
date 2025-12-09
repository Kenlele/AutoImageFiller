# Excel to Image Auto Fill (UiPath RPA)

本專案為一套使用 **UiPath RPA** 製作的自動化流程，  
能夠自動完成以下工作流程：

1. 讀取 Excel 資料
2. 開啟指定圖片模板
3. 將 Excel 對應欄位資料填入圖片指定位置
4. 產出並另存為新的 PNG 圖檔

適用於：  
📌 表單影像填值  
📌 證書、文件、名牌、票證圖片自動產生  
📌 大量圖像資料自動化處理

---

## 🧩 系統架構流程

Excel 資料來源
        ↓
讀取資料列
        ↓
開啟圖片模板
        ↓
依欄位對應填入圖片指定位置
        ↓
另存新圖片 (PNG)


## 🧩 資料夾結構

├── AutoFillImage.xaml                 # 主流程
├── project.json             
├── .screenshots/            
├── .settings/
├── .storage.runtime/
└── .tmh/

⚙️ 變數說明（使用前必須設定）

請在 UiPath 專案中自行設定以下 3 個路徑變數：

變數名稱	說明
InputExcelPath	Excel 資料來源路徑
TemplateImagePath	圖片模板路徑
OutputImageFolder	輸出圖片的資料夾路徑

## 🖼 圖片填值說明

使用圖片模板作為底圖

依 Excel 欄位資料對應填入：

姓名

編號

日期

最終輸出為：

PNG 圖檔格式

檔名可依 Excel 資料動態命名