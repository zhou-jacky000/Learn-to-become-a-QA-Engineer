# 壓力測試 (Stress Testing) 重點整理

## 1. 什麼是壓力測試？
壓力測試是一種用來驗證軟體應用程式的穩定性與可靠性的測試方式。  
**目標**：測試軟體在極端高負載下的強韌性與錯誤處理能力，確保軟體在壓力情境下不會崩潰。  
透過測試超越正常運行條件，評估系統在極端情況下的表現。

## 2. 壓力測試的重要性
**實際應用案例**：
- 電商網站在節日促銷期間流量激增。
- 新聞網站因熱門事件流量突然暴增。
- 教育考試成績查詢網站在成績公布時使用者大量湧入。

**壓力測試的價值**：
- 確保系統在異常條件下仍能運行。
- 檢查系統是否能顯示適當的錯誤訊息。
- 避免因系統崩潰造成收入與聲譽損失。
- 提前準備好應對突發流量，提升系統可用性。

## 3. 壓力測試的目標
- 觀察系統在失敗後的行為，確保能夠適當恢復（Recoverability）。
- 確保在壓力狀況下，系統能夠提供適當的錯誤訊息。
- 在測試過程中，可能會使用大量數據，因此數據安全也是重要考量。

## 4. 負載測試 vs. 壓力測試

| **負載測試 (Load Testing)** | **壓力測試 (Stress Testing)** |
| ------------------------- | -------------------------- |
| 測試系統在正常負載下的行為。 | 測試系統在極端負載下的表現，直到系統崩潰。 |
| 目的在於評估系統的效能。 | 目的是找出系統的崩潰點與錯誤處理能力。 |
| 不會導致系統崩潰。 | 可能導致系統崩潰，觀察極限情況。 |

## 5. 壓力測試的類型

### 分散式壓力測試（Distributed Stress Testing）
- 在分散式客戶端-伺服器系統中執行，伺服器會將壓力測試指令發送給所有客戶端並監控執行情況。
- 若伺服器未收到來自某些客戶端的回應，可能需要進一步調查。

### 應用程式壓力測試（Application Stress Testing）
- 專注於發現與資料鎖定、網路問題與效能瓶頸相關的缺陷。

### 交易壓力測試（Transactional Stress Testing）
- 測試兩個或多個應用程式之間的交易，確保系統能夠進行細微調整與最佳化。

### 系統性壓力測試（Systemic Stress Testing）
- 跨多個系統進行壓力測試，找出某個應用程式的資料是否影響其他應用程式。

### 探索性壓力測試（Exploratory Stress Testing）
- 測試系統在非預期情境下的行為，例如：
  - 大量用戶同時登入。
  - 病毒掃描在所有機器上同時執行。
  - 資料庫突然離線時系統的應對方式。
  - 大規模數據同時寫入資料庫的影響。

## 6. 壓力測試流程
1. **規劃測試**  
   收集系統數據，分析系統，定義壓力測試目標。
   
2. **建立自動化測試腳本**  
   開發測試腳本，準備測試數據，設計壓力測試場景。

3. **執行測試腳本**  
   進行壓力測試，並記錄測試結果。

4. **分析測試結果**  
   找出效能瓶頸，分析系統行為。

5. **調整與最佳化**  
   進行系統調整（優化程式碼、調整設定等），再重新測試。  
   通常需要 3～4 次測試迭代，才能達到最佳效能標準。

## 7. 壓力測試的指標

### 系統擴展性與效能
- **每秒請求數（Pages per Second）**：測量每秒處理的頁面數。
- **吞吐量（Throughput）**：單位時間內的資料處理量。
- **測試輪次（Rounds）**：測試場景執行的次數。

### 應用程式回應時間
- **點擊時間（Hit Time）**：加載圖片或頁面的平均時間。
- **首字節時間（Time to First Byte）**：伺服器傳送第一個字節的時間。
- **頁面載入時間（Page Time）**：加載整個頁面的時間。

### 錯誤與失敗
- **失敗連線數（Failed Connections）**：伺服器拒絕的連線次數。
- **失敗測試輪次（Failed Rounds）**：執行測試時的失敗次數。
- **失敗請求數（Failed Hits）**：未成功載入的請求數（如壞鏈接、丟失的圖片等）。

## 8. 壓力測試實例
- **電商網站的促銷活動**  
  測試場景：電商網站在促銷期間可能會面臨數百萬用戶同時訪問，需測試伺服器的承載能力。
  
- **新聞網站在重大事件時**  
  測試場景：當重大新聞發生時，新聞網站的流量可能突然暴增，需測試系統是否能正常運作。

- **考試成績查詢網站**  
  測試場景：當大量學生同時查詢成績時，網站是否能夠應對突發流量。

- **社群網站、部落格、應用程式**  
  測試場景：當一個部落格被大型媒體報導後，網站可能會突然湧入大量訪客，需測試伺服器的反應能力。

## 結論
壓力測試的主要目標：
- 檢測系統在極端條件下的穩定性。
- 監控系統資源（記憶體、CPU、網路等）。
- 測試系統在崩潰後是否能夠恢復（Recoverability）。
- 檢查系統是否能適當地顯示錯誤訊息。
