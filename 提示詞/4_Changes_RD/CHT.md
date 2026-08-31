請製作一張 16:9、4K、企業級簡報資訊圖，全部使用繁體中文。

主題：

# RD 的四個轉變：從寫 Code 到設計工程約束

副標：
AI 可以快速產生實作；RD 更重要的工作，是讓正確實作容易、錯誤實作困難。

風格：
白底、企業科技簡報、顧問式 Infographic。
綠色／深綠色作為 RD 主色，深墨藍文字。
使用架構、程式碼、盾牌、邊界、齒輪、監控等扁平 Vector Icon。
2×2 四卡布局，每張卡大小完全一致。
每張卡都有 BEFORE → AFTER。

【01】
從寫功能 → 設計系統與邊界

BEFORE：
Feature 做出來了嗎？
Code → Feature ✓

AFTER：
它應該存在於哪裡？
Architecture
Interface
Dependency
Data Flow
Boundary

使用架構圖、模組方塊、連線與邊界 icon。

Key Message：
程式每一行都可能合理，但整體仍可能放錯地方。

【02】
從寫 Code → 定義工程約束

BEFORE：
模糊指示：
「請注意效能」
「不要亂跨 Layer」

AFTER：
把規則寫成可機械判斷的 Constraint：

API P95 < 200 ms
Domain Layer 不得依賴 Infrastructure Layer
Invariant
Type
Contract

使用尺規、鎖、盾牌、程式規則 icon。

Key Message：
不是一直提醒 AI，而是定義哪些東西「不允許被寫錯」。

【03】
從手動實作 → 建立工程護欄

BEFORE：
工程師手動遵守 Coding Guideline

AFTER：
畫出流水線：

Code
→ Compiler / Type
→ Linter
→ Architecture Test
→ CI Gate
→ Merge

強調每一關都是自動化 Guardrail。

Key Message：
從「人記得守規則」變成「系統自動守規則」。

【04】
從功能能跑 → 預設失敗

BEFORE：
Happy Path Works
大型綠色勾勾

AFTER：
Design for Failure

Timeout
Retry
Failure Mode
Observability
Rollback
Graceful Degradation

使用警告、監控圖表、復原箭頭、斷路器等 icon。

Key Message：
不只設計如何成功，也要設計如何失敗、如何被看見、如何恢復。

【底部】
RD 的核心價值：

設計「怎麼不容易做錯」。

Architecture / Interface / Invariant / Boundary / Guardrail / Observability

整體需有工程感，但不能像技術文件，要像高階企業內訓簡報。
