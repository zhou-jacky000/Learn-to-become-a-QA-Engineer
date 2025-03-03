# 非功能測試（Non-Functional Testing）

非功能測試主要關注系統的**效能（Performance）、擴展性（Scalability）、安全性（Security）、可用性（Usability）**及**可靠性（Reliability）**，而非具體功能。此類測試確保系統能應對**真實世界的需求**，提供**流暢且高品質的使用者體驗**。

## 非功能測試的類型
- **效能測試（Performance Testing）**
- **擴展性測試（Scalability Testing）**
- **可用性測試（Usability Testing）**
- **安全測試（Security Testing）**
- **本地化測試（Localization Testing）**
- **可靠性測試（Reliability Testing）**

---

## 為什麼非功能測試很重要？
### 非功能測試的核心優勢：
✅ **確保系統穩定性**  
✅ **提升使用者體驗**  
✅ **增強擴展能力**  
✅ **預防安全漏洞**  
✅ **提升品牌聲譽**  

本篇文章將探討**非功能測試的核心目標、特點、優勢及類型**。

---

## 非功能測試的核心目標
### 主要目標：
1. **提升可用性與效能**：確保系統易於使用、有效率、可維護，並能夠適用於不同環境。  
2. **降低生產風險與成本**：及早發現非功能性問題，減少部署後的故障與修復成本。  
3. **改善產品的安裝與操作**：確保產品的安裝、配置與執行流暢，並能夠有效管理與監控。  
4. **測量與分析系統指標**：收集效能數據，分析系統行為，優化系統開發。  
5. **理解技術與產品行為**：確保產品與現有技術相容，並滿足效能需求。  

---

## 非功能測試的特點
- **應具備可量化性**，避免使用「好」、「更好」、「最佳」等模糊詞彙。  
- **需求的確切數據可能在初期無法完全確定**。  
- **需要確定優先級**，確保關鍵的測試項目得到驗證。  
- **在軟體工程中，品質屬性應被準確識別**。  

---

## 非功能測試的類型

### 1. **效能測試（Performance Testing）**
確保軟體的執行速度不會過慢或受限，例如：  
**範例**：1000 名使用者同時使用應用程式時，載入時間不超過 5 秒。  
**常用工具**：LoadRunner、Apache JMeter、WebLOAD。

### 2. **負載測試（Load Testing）**
測試系統在**高並發**使用者下的承載能力。  
**常用工具**：Neoload、Load Multiplier。

### 3. **安全測試（Security Testing）**
找出軟體系統的安全漏洞，評估其**防禦攻擊**的能力。  
**常用工具**：ImmuniWeb、Vega、Wapiti。

### 4. **可移植性測試（Portability Testing）**
測試軟體在不同操作系統與硬體上的運行能力。  
**常用工具**：SQLMap。

### 5. **可靠性測試（Reliability Testing）**
檢測系統在**預定條件**下的穩定性，例如所有網頁連結是否有效。  
**常用工具**：Test-retest、Inter-rater。

### 6. **效率測試（Efficiency Testing）**
測試系統資源的使用效率，例如處理速度與記憶體占用率。  
**常用工具**：WebLOAD、LoadNinja。

### 7. **資料量測試（Volume Testing）**
測試系統在**大量數據負載**下的表現，例如擴增資料庫容量來觀察系統是否崩潰。  
**常用工具**：HammerDB、JdbcSlim。

### 8. **恢復測試（Recovery Testing）**
測試系統在崩潰後的**恢復能力**，例如測試電源中斷後的資料回復。  
**常用工具**：Box Backup、Bacula。

### 9. **響應式測試（Responsive Testing）**
測試網站在不同**螢幕尺寸**下的適應性，確保使用者體驗一致。  
**常用工具**：Responsinator、Screenfly、Google DevTools。

### 10. **視覺測試（Visual Testing）**
確保使用者介面（UI）顯示正確，不會產生**視覺錯誤**（Visual Bugs）。  
**常用工具**：Percy、PhantomCSS、Gemini、Needle（Python）。  

---

## 非功能測試的關鍵指標

| 測試參數 | 說明 | 測試方式 |
|----------|------|----------|
| **安全性（Security）** | 保護系統免受內部與外部攻擊 | 安全測試 |
| **可靠性（Reliability）** | 保證系統長時間運行不出錯 | 可靠性測試 |
| **效率（Efficiency）** | 測試系統處理速度與資源消耗 | 效能測試 |
| **可用性（Usability）** | 評估使用者與系統的互動體驗 | 可用性測試 |
| **可擴展性（Scalability）** | 測試系統是否能應對使用量增長 | 負載測試 |

---

## 非功能測試的優勢
🔹 **提升安全性**：確保系統免受網路攻擊，保護數據與用戶信任。  
🔹 **改善負載處理能力**：確保系統能夠應對高並發使用者。  
🔹 **提升效率**：優化系統運行，使其能夠在不同條件下快速處理任務。  
🔹 **測試案例可重用**：減少重複編寫測試案例的需求。  
🔹 **減少測試時間**：相較於其他測試方法，非功能測試通常需要較少時間。  

---

## 總結
非功能測試是確保**軟體穩定性、可擴展性、安全性與可用性**的關鍵步驟。透過不同類型的測試（如效能測試、安全測試等），我們可以發現並解決系統中的非功能性問題，從而提升軟體品質，確保最終用戶獲得最佳體驗。
