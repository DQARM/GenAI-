```
請生成一張專業、清楚、適合技術簡報使用的資訊圖（infographic），風格簡潔、現代、工程技術感、白底或淺色底、配色以藍色、青色、灰色為主，重點資訊用橘色或綠色點綴。
版面乾淨、邏輯分區明確、圖示清楚、箭頭流向明確。
所有文字請使用繁體中文，英文技術名詞可保留，例如 Validation Governance, Security Governance, Explainability Governance, Compliance Governance, Audit Governance
請讓字體清晰可讀，適合放在投影片中展示。避免太花俏，重點是教學清楚、結構清楚。
請使用扁平化圖示、流程圖、方塊圖、層級圖與小型註解框。

主提示詞

請依照參考圖片的資訊架構，生成一張適合企業內訓、技術研討會與 PowerPoint 簡報使用的 4K、16:9 橫式資訊圖。

圖片主題

AI 產生測試的生態系：從生成到治理的實作工具總覽

副標題：

這些工具各自負責不同環節，組合起來可建構類似 GATF 的治理流程

整體視覺風格
解析度：3840 × 2160
比例：16:9
專業企業級科技資訊圖
白色或極淺灰背景
深藍色為主色，搭配亮藍、青綠、少量紫色
Clean vector illustration
現代、簡潔、工程感、架構圖風格
清楚的網格排版與資訊階層
使用一致的線性圖示
卡片採圓角矩形、細邊框、淡陰影
字型清晰、粗細分明
不要使用人物照片
不要卡通化
不要過度科幻
不要使用品牌 Logo 原圖，可使用簡化的抽象符號搭配正確工具名稱
所有中文使用繁體中文
英文工具名稱必須拼寫正確
留足夠留白，避免文字過度擁擠
上方：七階段治理流程

畫面上方放置一條由左至右的七階段流程，以箭頭連接，每個階段使用獨立圓角卡片與圖示。

1. 生成測試

小標：

AI 產生 Test Artifacts

圖示：AI 晶片、機器腦或程式碼文件。

2. 驗證測試

小標：

檢查測試是否有效

圖示：剪貼板、勾選清單。

3. 安全檢查

小標：

檢查風險與安全性

圖示：盾牌。

4. 政策治理

小標：

依組織政策做決策

圖示：天平或政策文件。

5. 評估與解釋

小標：

評估品質與可解釋性

圖示：放大鏡、分析圖。

6. 追蹤與稽核

小標：

完整紀錄與可追溯

圖示：稽核文件或日誌。

7. 執行測試

小標：

通過後執行到環境

圖示：綠色火箭或啟動按鈕。

第 7 階段使用綠色外框，表示通過治理後才允許執行。

中間：六欄工具分類總覽

將主要內容分成六個垂直欄位。每個欄位頂端使用深藍色標題列，下方放置工具卡片。

第一欄：AI 測試生成工具

副標：

負責產生測試案例／腳本

gstack

描述：

AI 原生的開發與測試助手

重點：

讀取程式變更 Git diff
產生並執行測試
產生 Regression Test
/qa、/ship、/review 等技能
TestSpark

描述：

JetBrains 開源外掛

重點：

使用 LLM／EvoSuite
產生 Java／Kotlin Unit Test
自動檢查測試是否有效
評估 Coverage／Mutation
第二欄：測試驗證工具

副標：

檢查測試是否可執行、有效

CoverUp

描述：

Python AI Test Generator

重點：

產生、執行、檢查與修正
確認 Coverage 是否增加
偵測 Flaky Test
隔離可能污染其他測試的案例
建議在 Docker 中執行
OSS-Fuzz-Gen

描述：

Google Fuzz Target 生成器

重點：

使用 LLM 產生 Fuzz Target
在 OSS-Fuzz 環境評估
檢查編譯、Crash 與 Coverage
支援多 Agent 比較
第三欄：安全檢查工具

副標：

掃描風險、漏洞與不安全行為

NeMo Guardrails

描述：

LLM／Agent 安全防護框架

重點：

Prompt Injection 防護
Jailbreak 偵測
敏感資訊防洩漏
Tool Calling 控制
Logging 與 Tracing
SAST／Dependency Scan

描述：

安全掃描工具組合

重點：

掃描測試腳本與依賴
檢查已知漏洞
偵測危險函式與指令
確保測試執行環境安全
第四欄：政策治理工具

副標：

依組織政策決定是否允許執行

Agent Governance Toolkit

描述：

Microsoft 開源 Agent 治理框架

重點：

攔截 Tool Call、API 與資源操作
政策判斷：Allow／Deny／Require Approval
權限控管與沙箱執行
完整 Audit Log
支援人工核准流程
Open Policy Agent（OPA）

描述：

政策即代碼引擎，CNCF 專案

重點：

使用 Rego 政策語言定義規則
將測試資訊轉成 JSON 輸入
決定是否允許執行
Decision Log 可查
適合建立企業級 Policy Gate
第五欄：評估與解釋工具

副標：

評估測試品質與可解釋性

Giskard

描述：

LLM／Agent 測試與評估框架

重點：

情境測試與弱點掃描
LLM-as-a-judge 評估
評估測試是否符合需求
支援自訂指標與報告
DeepEval

描述：

LLM 測試框架，使用方式類似 pytest

重點：

Task Completion 評估
Hallucination 檢測
Answer Relevancy 評估
支援 Agent 與自訂指標
第六欄：追蹤與稽核工具

副標：

保存紀錄、追溯與監控

MLflow

描述：

AI／LLM 生命週期平台

重點：

Dataset 與 Ground Truth 管理
自訂 Scorer 與評估結果保存
Trace Agent 執行流程
版本比較與人工回饋
Production Monitoring
建立完整可追溯紀錄
下方：組合成類似 GATF 的流程

在工具分類區下方加入一條簡化的流程帶，標題：

如何組合成類似 GATF 的流程？

以圖示與箭頭呈現：

1. 生成

gstack／TestSpark

小標：

產生測試

→

2. 驗證

CoverUp／TestSpark

小標：

驗證測試有效性

→

3. 安全檢查

NeMo Guardrails／SAST

小標：

掃描風險

→

4. 政策治理

Agent Governance Toolkit／OPA

小標：

政策判斷與核准

→

5. 評估與解釋

Giskard／DeepEval

小標：

評估品質與合理性

→

6. 追蹤與稽核

MLflow

小標：

保存所有紀錄

→

執行測試

使用綠色火箭圖示。

小標：

通過後執行到測試環境

最下方：重點結論

最底部設計一條橫向結論區，左側放置深藍色標籤：

重點結論

右側分成三個重點：

沒有單一工具涵蓋所有能力，需要組合使用才能完整落地。
生成能力已成熟，治理能力仍在快速發展中。
最終目標：讓 AI 產生的測試值得信任、可執行、可追溯。
排版要求
上方流程約占畫面高度 18%
中間六欄工具總覽約占 48%
下方組合流程約占 20%
最底部結論約占 10%
所有欄位寬度一致
卡片對齊整齊
箭頭方向清楚
標題與內文有明顯字級差異
工具名稱使用粗體
描述文字簡短易讀
不要產生錯字、亂碼或簡體中文
若文字過多，優先保留工具名稱、分類名稱與每個工具的前三項核心功能
整體必須能直接放入 PowerPoint 投影片，不需額外裁切

負面提示詞
低解析度、模糊、簡體中文、錯別字、亂碼、英文拼寫錯誤、文字重疊、文字超出卡片、過度擁擠、元素未對齊、卡通風、兒童教材風、手繪風、賽博龐克、霓虹城市、黑暗背景、過度漸層、過度立體、照片寫實人物、誇張機器人、品牌浮水印、商標錯誤、低品質圖示、不一致圖示、過小文字、複雜裝飾、資訊階層混亂。
```
