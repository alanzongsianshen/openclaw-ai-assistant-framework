# **OpenClaw AI 助理框架 (OpenClaw AI Assistant Framework)**

一個專業、高效、具備自主成長能力的 AI 助理框架

## **✨ 框架簡介**

OpenClaw AI Assistant Framework 是一款基於 OpenClaw 建構的專業級 AI 助理框架，旨在提供高效且能持續進化的開發底座，適用於各類 AI 應用場景。

### **核心特性**

**🚀 OpenClaw 深度使用 7 步法**

1. **智慧備份機制** \- 24 小時內偵測到 10K 次檔案變動即觸發，採用 7 天循環覆蓋。  
2. **四層模型池體系** \- 包含高速池、強大智能池、純文字池、多模態視覺池。  
3. **對話辨識規則** \- 系統自動判斷並切換至最合適的模型池。  
4. **上下文壓縮 (Context Compression)** \- 有效節省 22% 的 Token 消耗。  
5. **任務鐵律** \- 嚴格執行 5 次重試限制，單次上限 20,000 Tokens。  
6. **陌生任務處理** \- 優先檢索 ClawHub 資源，具備自動學習能力。  
7. **自我演化** \- 每日 22:00 自動產出「進化報告」。

**🧠 三層記憶體系**

* **L1 工作記憶 (Working Memory)** \- 當前對話的暫存內容。  
* **L2 短期記憶 (Short-term)** \- 每日記憶存檔（路徑：memory/YYYY-MM-DD.md）。  
* **L3 長期記憶 (Long-term)** \- 永久性記憶檔案（MEMORY.md）。

**🔄 Heartbeat 記憶維護機制**

* **每 30 分鐘**：檢查緊急待辦事項、整理記憶碎片、清理 Log 紀錄。  
* **每日**：將核心決策與重要資訊提取至 MEMORY.md。  
* **每週**：回顧 MEMORY.md，並清理超過 30 天的冗餘資訊。

**📚 AI 自我成長機制**

* **技能深度學習**：並非單純安裝工具，而是對 Skill 進行深度邏輯拆解與理解。  
* **經驗總結**：每 30 分鐘進行自我反思，詳實紀錄經驗教訓。  
* **知識整合**：主動發現跨領域關聯，創造全新的解決方案。

## **🎯 24 小時定向學習計畫**

框架採用「分時段學習策略」，依據不同時段自動排程學習相關領域技能：

### **前 12 小時 (00:00-12:00) — 視覺創意時段 🎨**

* **00:00-04:00**：AI 算圖、提示詞工程 (Prompt Engineering)。  
* **04:00-08:00**：影片製作、剪輯工具應用。  
* **08:00-12:00**：視覺優化、平面設計工具。

### **後 12 小時 (12:00-24:00) — 自媒體營運時段 📱**

* **12:00-16:00**：內容創作、社群文案撰寫。  
* **16:00-20:00**：社群媒體操作、互動與經營。  
* **20:00-24:00**：數據分析、自動化行銷 (Marketing Automation)。

## **🚀 快速上手**

### **1\. 複製儲存庫 (Clone)**

git clone git@github.com:alanzongsianshen/openclaw-ai-assistant-framework.git  
cd openclaw-ai-assistant-framework

### **2\. 執行安裝腳本**

chmod \+x install.sh  
./install.sh

**安裝腳本功能說明：**

* ✅ 自動建立目錄結構。  
* ✅ 產生核心設定檔（具備保護機制，不會覆蓋現有檔案）。  
* ✅ 安裝 ClawHub CLI 工具。  
* ✅ 預載核心技能組。  
* ✅ 配置 Cron Job 定時任務排程。

### **3\. 設定模型池 (Model Pools)**

編輯 config/model-pools.json：
```
{
  "version": 1,
  "pools": {
    "fast": {
      "name": "高效",
      "primary": "google/gemini-3-flash-preview",
      "fallback": "anthropic/claude-haiku-4-5"
    },
    "smart": {
      "name": "深度規劃",
      "primary": "google/gemini-3.1-pro-preview",
      "fallback": "anthropic/claude-opus-4-6"
    }
  }
}
```

### **4\. 設定 24 小時學習時程**

編輯 config/skill-learning-schedule.json：

```
{  
  "hourly\_rotation": {  
    "00-04": \["image", "prompt", "ai-art", "generation"\],  
    "04-08": \["video", "editing", "production", "creative"\],  
    "08-12": \["design", "graphics", "photo", "visual"\],  
    "12-16": \["content", "writing", "copywriting", "blog"\],  
    "16-20": \["social", "twitter", "weibo", "engagement"\],  
    "20-24": \["analytics", "automation", "seo", "marketing"\]  
  }  
}
```

## **📚 說明文件**

### **核心文件**

* [完整框架文檔](https://www.google.com/search?q=docs/openclaw-ai-assistant-framework.md) \- OpenClaw 7 步深度操作指南  
* [AI 自我進化計畫](https://www.google.com/search?q=docs/ai-self-evolution-plan.md) \- 涵蓋 6 大成長維度  
* [AI 自我進化實作](https://www.google.com/search?q=docs/ai-self-evolution-implementation.md) \- 程式碼與技術細節  
* [Skill 深度學習](https://www.google.com/search?q=docs/skill-deep-learning.md) \- 知識萃取與模組整合  
* [上下文壓縮機制](https://www.google.com/search?q=docs/context-compression-mechanism.md) \- 框架運作固化原理  
* [每日成長報告](https://www.google.com/search?q=docs/daily-growth-report-mechanism.md) \- 學習進度視覺化  
* [經驗總結機制](https://www.google.com/search?q=docs/experience-summary-mechanism.md) \- 經驗庫管理流程

### **設定文件**

* [模型池設定](https://www.google.com/search?q=config/model-pools.md) \- 4 層級模型調度體系  
* [對話路由 (Routing)](https://www.google.com/search?q=config/session-routing.md) \- 自動化模型切換規則  
* [任務鐵律](https://www.google.com/search?q=config/task-iron-law.md) \- 5 次重試容錯機制  
* [上下文壓縮](https://www.google.com/search?q=config/context-compression.md) \- 壓縮演算法規則  
* [自我演化](https://www.google.com/search?q=config/self-evolution.md) \- 系統進化邏輯  
* [陌生任務處理](https://www.google.com/search?q=config/unfamiliar-task-handling.md) \- 未知問題解決流程  
* [大腦肌肉配置](https://www.google.com/search?q=config/brain-muscle-config.md) \- 行為模式與風格設定

## **⏰ 定時任務體系 (共 8 項)**

### **維護類**

1. **heartbeat-notify** \- 每 30 分鐘（執行記憶維護）。  
2. **smart-backup** \- 每小時（執行智慧增量備份）。  
3. **model-health-check** \- 每 6 小時（檢查模型端點健康度）。

### **進化類**

4. **install-skills-infinite** \- 每小時（自動探索並學習新技能）。  
5. **daily-evolution** \- 每天 22:00（產生今日進化報告）。

### **數據類**

6. **daily-growth-report** \- 每天 09:00（產出成長進度表）。  
7. **daily-report-gen** \- 每天 09:30（產生系統日報）。

### **迭代類**

8. **mission-control-weekly** \- 每週一 20:00（執行大版本迭代回顧）。

## **🔧 核心腳本 (Scripts)**

### **學習相關**

* scripts/batch-extract-knowledge.py \- 批次知識萃取。  
* scripts/extract-skill-knowledge.py \- 單項技能知識分析。  
* scripts/extract-skill-knowledge-enhanced.py \- 強化版知識分析工具。  
* scripts/integrate-knowledge.py \- 跨領域知識整合。

### **維護相關**

* scripts/daily-evolution.py \- 處理每日進化報告邏輯。  
* scripts/model-health-check.py \- 執行模型池壓力與連線測試。

### **測試相關**

* scripts/test-compression.py \- 測試上下文壓縮效率。  
* scripts/test-iron-law.py \- 測試任務重試與容錯機制。  
* scripts/test-session-routing.py \- 測試對話路由判斷準確率。  
* scripts/test-unfamiliar-task.py \- 模擬處理未知任務的流程。

## **🎯 核心原則 (Preferences)**

本框架嚴格遵循以下設計思維：

* ✅ **精簡結構化溝通** \- 追求最高資訊傳達效率。  
* ✅ **數據驅動、成本敏感、風控優先** \- 以理性與投報率為核心決策導向。  
* ✅ **公式優於硬編碼、工具鏈分層、全面自動化** \- 強烈的工程技術導向。

## **🚀 版本紀錄**

### **v3.0 (2026-02-28) — 自我成長版**

* ✅ 上線 24 小時定向學習系統。  
* ✅ 實作 AI 自我成長與進化機制。  
* ✅ 導入 Skill 深度學習與經驗總結系統。  
* ✅ 知識整合與每日成長報告功能完備。

### **v2.0 (2026-02-27) — 框架固化版**

* ✅ 確立 7 步深度使用標準流程。  
* ✅ 建構 4 層模型池與 3 層記憶體系。  
* ✅ 導入 Heartbeat 記憶自動維護機制。

## **🛡️ 安全合規保證**

**當前版本已通過各項安全性檢查：**

* ✅ 絕無真實 API TOKEN（僅保留範例預留位置）。  
* ✅ 不含個人隱私敏感數據。  
* ✅ 無任何具破壞性的系統指令。  
* ✅ 腳本來源透明，無第三方後門。  
* ✅ install.sh 腳本經過安全性驗證。  
* ✅ 具備檔案保護，不會隨意刪除或覆蓋使用者既有資料。

## **🤝 貢獻指南**

我們非常歡迎社群提交 Issue 或 Pull Request (PR)！

**貢獻步驟：**

1. Fork 本專案儲存庫。  
2. 建立功能分支 (git checkout \-b feature/AmazingFeature)。  
3. 提交變更 (git commit \-m 'Add some AmazingFeature')。  
4. 推送至分支 (git push origin feature/AmazingFeature)。  
5. 發起 Pull Request。

## **📄 授權協議**

本專案採 **MIT License** 授權。
