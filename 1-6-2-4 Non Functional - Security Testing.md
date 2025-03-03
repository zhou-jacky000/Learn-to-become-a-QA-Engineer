### 什麼是安全測試 (Security Testing)？
安全測試是一種軟體測試方法，用於發現軟體應用程式的漏洞、威脅和風險，並防止惡意攻擊者的入侵。其目標是找出軟體系統中可能的安全缺陷，避免因內部或外部攻擊而導致資訊、收入或企業聲譽的損失。

---

### 為什麼安全測試很重要？
安全測試的主要目標是識別系統中的威脅，評估其潛在漏洞，確保系統不會受到攻擊而停止運行或被惡意利用。此外，它還能幫助開發人員發現安全風險，並透過程式碼修正來強化系統安全性。

---

### 軟體測試中的安全測試類型
根據 **開源安全測試方法手冊 (Open Source Security Testing Methodology Manual, OSSTMM)**，安全測試可分為以下七種主要類型：

1. **漏洞掃描 (Vulnerability Scanning)**  
   透過自動化工具掃描系統，檢查已知的漏洞。

2. **安全掃描 (Security Scanning)**  
   透過手動或自動方式識別網路與系統的弱點，並提供降低風險的解決方案。

3. **滲透測試 (Penetration Testing)**  
   模擬惡意駭客攻擊，以分析系統對外部攻擊的防禦能力。

4. **風險評估 (Risk Assessment)**  
   針對組織內的安全風險進行分析，並將風險分級為 **低、中、高**，提供應對建議。

5. **安全稽核 (Security Auditing)**  
   內部檢查應用程式與作業系統的安全性，可能包含程式碼逐行檢查。

6. **道德駭客 (Ethical Hacking)**  
   在取得授權的情況下對企業軟體系統進行駭客測試，以找出安全漏洞。

7. **安全狀態評估 (Posture Assessment)**  
   結合 **安全掃描、道德駭客、風險評估**，全面評估組織的安全狀態。

---

### 如何執行安全測試？
安全測試應該納入 **軟體開發生命週期 (SDLC)**，並在各階段採取對應的安全措施，以降低開發後期發現漏洞所帶來的成本。

| **SDLC 階段**      | **安全測試措施** |
|------------------|---------------|
| **需求分析**      | 進行安全需求分析，檢查濫用/誤用案例 |
| **設計**         | 設計風險分析，制定包含安全測試的測試計畫 |
| **編碼與單元測試** | 進行靜態與動態測試，以及安全白箱測試 |
| **整合測試**      | 黑箱測試 |
| **系統測試**      | 黑箱測試與漏洞掃描 |
| **部署**         | 滲透測試與漏洞掃描 |
| **維護與支援**    | 修補程式影響分析 |

#### 測試計畫應包含：
- 安全相關測試案例與測試情境
- 測試所需的安全性資料
- 所需的安全測試工具
- 來自不同安全測試工具的測試結果分析

---

### 安全測試案例示例
以下是一些常見的安全測試場景：

- **密碼應以加密格式存儲**
- **系統應防止未經授權的用戶訪問**
- **檢查應用程式的 Cookie 和 Session 時間**
- **金融網站應禁止瀏覽器的返回按鈕，以防止重複交易**

---

### 安全測試方法與技術
不同的安全測試方法如下：

- **Tiger Box 測試**  
  使用內建多個作業系統與駭客工具的筆記型電腦來評估系統漏洞與攻擊風險。

- **黑箱測試 (Black Box Testing)**  
  測試人員在不了解系統內部結構的情況下，對系統進行測試。

- **灰箱測試 (Grey Box Testing)**  
  測試人員獲得部分系統資訊，進行結合白箱與黑箱測試的混合測試。

---

### 安全測試角色
- **駭客 (Hacker)**：未經授權即存取電腦系統或網路的個人。
- **破解者 (Cracker)**：入侵系統以竊取或破壞數據的人。
- **道德駭客 (Ethical Hacker)**：在合法授權下進行系統攻擊測試，以找出安全漏洞。
- **新手駭客 (Script Kiddies / Packet Monkeys)**：缺乏經驗的駭客，通常依賴現成的駭客工具進行攻擊。

---

### 安全測試的迷思與事實
| **迷思** | **事實** |
|---------|---------|
| **迷思 1：我們的企業規模很小，不需要安全策略** | **事實：無論規模大小，每家公司都需要安全策略** |
| **迷思 2：安全測試沒有投資回報 (ROI)** | **事實：安全測試能夠提高效率，減少停機時間，提升最大效能** |
| **迷思 3：唯一的安全方式就是斷開網路連線** | **事實：最好的安全方法是找到“完美安全性”，透過評估與合規來確保安全** |
| **迷思 4：只要購買安全軟體或硬體，我的系統就安全了** | **事實：僅購買安全產品並不能解決安全問題，企業應先理解安全風險並採取適當的防護措施** |

---

### 結論
安全測試對於保護軟體系統免受攻擊至關重要，它能夠：
- 檢測與修復系統中的安全漏洞
- 評估系統抵禦攻擊的能力
- 確保應用程式的數據與用戶資訊安全
- 幫助企業避免財務與聲譽損失

透過適當的安全測試策略，企業可以有效降低風險，確保系統的安全性與穩定性。
