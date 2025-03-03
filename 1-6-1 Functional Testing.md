# 什麼是功能測試？

功能測試是一種軟體測試方法，主要驗證軟體系統是否符合功能需求與規格。此測試關注應用程式的功能，而不考慮其內部程式碼結構。功能測試通常屬於 **黑箱測試**，測試範圍包括 **使用者介面（UI）、API、資料庫、安全性、客戶端/伺服器通訊** 等。

功能測試可透過 **手動測試** 或 **自動化測試** 進行，目的在於確保軟體的功能符合需求，並能夠正確處理不同情境的輸入與輸出。

---

## 功能測試的範圍

功能測試主要檢查以下方面：

- **核心功能**：確保應用程式的主要功能正常運作。
- **基本可用性**：測試系統是否能讓使用者流暢操作。
- **可存取性（Accessibility）**：驗證系統對不同使用者的可用性。
- **錯誤處理**：檢查系統是否能正確處理錯誤，並顯示適當的錯誤訊息。

---

## 功能測試的步驟

1. 理解功能需求
2. 識別測試輸入（測試數據）
3. 計算預期結果
4. 執行測試案例
5. 比較實際結果與預期結果

---

## 功能測試的類型

### 1. 單元測試（Unit Testing）
測試軟體的最小單元（函式、類別等），需確保測試覆蓋率，包括：
- **行覆蓋率（Line Coverage）**
- **程式碼路徑覆蓋率（Code Path Coverage）**
- **方法覆蓋率（Method Coverage）**

### 2. 煙霧測試（Smoke Testing）
進行基本功能測試，確保系統穩定性。

### 3. 健全性測試（Sanity Testing）
確認主要功能是否能夠運作正常。

### 4. 回歸測試（Regression Testing）
確保新功能或修復不會影響原有功能。

### 5. 整合測試（Integration Testing）
驗證不同模組或系統的整合是否正常運作。

### 6. 使用者驗收測試（User Acceptance Testing, UAT）
由最終使用者測試系統，以確保符合業務需求。

### 7. 白箱測試（White Box Testing）
測試系統的內部運作方式與邏輯。

### 8. 灰箱測試（Grey Box Testing）
結合黑箱與白箱測試，檢查內部邏輯與功能。

### 9. 探索性測試（Exploratory Testing）
測試人員透過探索性的方式發掘潛在問題。

### 10. 黑箱測試（Black Box Testing）
只關注輸入與輸出，而不考慮內部邏輯。

### 11. 元件測試（Component Testing）
測試單一元件的獨立功能。

### 12. 資料庫測試（Database Testing）
確保資料庫的操作（新增、讀取、更新、刪除）符合預期。

### 13. 恢復測試（Recovery Testing）
驗證系統在故障後能否正常恢復。

### 14. 靜態測試（Static Testing）
不執行程式碼，而是透過檢查設計、文件或程式碼來驗證功能。

---

## 功能測試與非功能測試的區別

| 比較項目  | 功能測試（Functional Testing） | 非功能測試（Non-Functional Testing） |
|-----------|--------------------------------|-------------------------------------|
| **目的** | 驗證軟體是否符合功能需求 | 測試系統效能、可靠性、可擴展性等 |
| **測試重點** | 測試系統的行為與功能 | 測試系統的性能與用戶體驗 |
| **測試技術** | 等價類測試、邊界值分析、決策表測試等 | 性能測試、負載測試、壓力測試等 |
| **測試範例** | 測試表單提交功能 | 測試不同網路條件下的載入速度 |
| **常用工具** | Selenium、Cypress、Appium 等 | JMeter、LoadRunner 等 |

---

## 功能測試的技術

### 1. 系統測試（End-User/System Tests）
測試整個系統，確保所有元件協同工作。

### 2. 等價類測試（Equivalence Tests）
將測試數據分成不同區間，測試每個區間的一個代表值。

### 3. 邊界值測試（Boundary Value Tests）
測試數據範圍的上下限，以確保系統正確處理邊界條件。

### 4. 決策表測試（Decision-Based Tests）
根據不同的輸入條件，測試系統的決策邏輯。

### 5. 隨機測試（Ad-hoc Tests）
無計畫的測試，以找出難以預測的錯誤。

---

## 功能測試的工具

### 自動化測試工具
- **Selenium**
- **Cypress**
- **Playwright**
- **Puppeteer**
- **Appium**

### 測試管理工具
- **BrowserStack**
- **TestRail**
- **JIRA**

---

## 功能測試的優勢

✅ 早期發現錯誤  
✅ 確保符合業務需求  
✅ 提高軟體品質與用戶體驗  
✅ 確保跨平台相容性  
✅ 符合法規與標準  

---

## 功能測試的案例

### 測試場景：
某人力資源管理系統（HRMS）登入頁面包含 **使用者名稱** 與 **密碼欄位**，以及 **「登入」** 與 **「取消」** 按鈕。

### 測試條件：
- **使用者名稱**
  - 長度需為 **6~10 個字元**
  - 允許 **字母、數字、部分特殊符號（_ . -）**
  - 不得為空
- **密碼**
  - 長度需為 **6~8 個字元**
  - 允許 **字母、數字、所有特殊符號**
  - 不得為空

### 測試案例：

1. **正確的使用者名稱與密碼** → 成功登入  
2. **錯誤的密碼** → 顯示錯誤訊息  
3. **空白使用者名稱或密碼** → 顯示錯誤訊息  
4. **按「取消」按鈕** → 回到登入頁面  
