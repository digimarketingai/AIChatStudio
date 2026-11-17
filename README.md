# AI Chat Studio — OpenRouter Single-File Template

[English](#english) | [繁體中文](#繁體中文)

---

<a name="english"></a>
## English

A clean, modern, single-file (`index.html`) AI chat platform powered by the **OpenRouter API**, built specifically for **GitHub Pages** hosting and **Vibe Coding** customization.

### ✨ Features
- **Zero Build / Single File**: Everything (HTML, CSS, JS) lives in `index.html`. Upload and run immediately.
- **Streaming Responses**: Real-time token streaming with a Stop Generation button and Markdown/Code block rendering.
- **Free Models Ready**: Pre-configured with fast `:free` models plus live auto-fetching from OpenRouter's model catalog.
- **Flexible Auth (BYOK + OAuth PKCE)**: Users can paste their own OpenRouter API key or click **Sign in with OpenRouter**.
- **Optional Knowledge Base**: Toggleable context window where users can paste text or upload `.txt`, `.md`, `.json`, or `.csv` files for instant Q&A.
- **Dark & Light Mode**: Responsive UI for desktop and mobile, plus one-click `.md` chat export.

### 🚀 Deploy to GitHub Pages (3 Steps)
1. Create a new public repository on GitHub.
2. Upload `index.html` and `README.md` to the root of the repository.
3. Go to **Settings → Pages → Build and deployment**, set Source to **Deploy from a branch** (`main` / `/ (root)`), and save. Your site will be live in ~1 minute!

### ⚡ Proposed Fast Free Models
Free OpenRouter models (`:free`) cost **$0** per token (no credit card required, capped at 20 req/min and 50 req/day—or 1,000/day after a $10 lifetime top-up). Because free endpoints rotate, `openrouter/free` is set as the default auto-router.

| Model ID | Best For | Context | Notes |
| :--- | :--- | :--- | :--- |
| `openrouter/free` | **General / Reliability (Default)** | Dynamic | Auto-picks an available free model |
| `nvidia/nemotron-3.5-super-vl:free` | **Fast General & Vision** | 1M | Very fast response (~0.7–0.9s) |
| `nvidia/nemotron-3.5-lightning:free` | **Ultra-Fast Chat** | 1M | Optimized for low-latency speed |
| `nvidia/nemotron-3-ultra-550b-a55b:free` | **Complex Reasoning** | 1M | 550B MoE flagship reasoning |
| `cohere/north-mini-code:free` | **Coding & Debugging** | 256K | Lightweight coding specialist |
| `google/gemma-4-31b-it:free` | **Multilingual & Writing** | 262K | Strong general & Chinese/English |
| `google/gemma-4-26b-a4b-it:free` | **Fast All-Rounder** | 262K | Balanced speed and quality |

### 🎨 Vibe Coding Customization Guide
`index.html` is organized into 4 clearly labeled sections (`STYLES`, `SIDEBAR`, `MAIN CHAT`, `JAVASCRIPT ENGINE`) with a central `CONFIG` object. Try pasting `index.html` into your favorite AI coding tool with prompts like:
- *"Change the `CONFIG.APP_TITLE`, `STARTER_PROMPTS`, and `DEFAULT_SYSTEM_PROMPT` to turn this into a Customer Support Bot."*
- *"Update the `:root` CSS variables to use a warm emerald green and cream aesthetic."*
- *"Add a button in the chat header to switch the UI language between English and Traditional Chinese."*

---

<a name="繁體中文"></a>
## 繁體中文

這是一個專為 **GitHub Pages** 與 **Vibe Coding（AI 輔助開發）** 設計的單一檔案（`index.html`）AI 聊天平台範本，直接串接 **OpenRouter API**。

### ✨ 核心功能
- **零建置／單一檔案**：所有 HTML、CSS、JavaScript 都在 `index.html` 內，上傳即可使用，無需後端伺服器。
- **即時串流回覆（Streaming）**：支援即時打字機串流顯示、隨時中止生成，以及 Markdown 與程式碼區塊一鍵複製。
- **支援免費模型**：內建推薦的高速 `:free` 模型清單，並支援即時從 OpenRouter API 更新最新免費模型。
- **安全登入機制（BYOK + OAuth PKCE）**：使用者可自行貼上 OpenRouter API Key，或直接點擊 **Sign in with OpenRouter** 授權登入（金鑰僅儲存於使用者瀏覽器端）。
- **選配知識庫（Knowledge Base）**：可自由開啟或關閉，支援直接貼上參考文字或上傳 `.txt`、`.md`、`.json`、`.csv` 檔案作為 AI 回答依據。
- **深淺色主題與匯出**：支援深色／淺色模式切換、手機版響應式介面，以及一鍵匯出對話為 `.md` 檔案。

### 🚀 部署至 GitHub Pages（只需 3 步驟）
1. 在 GitHub 建立一個新的公開儲存庫（Repository）。
2. 將 `index.html` 與 `README.md` 上傳至儲存庫根目錄。
3. 前往 **Settings → Pages → Build and deployment**，將 Source 設為 **Deploy from a branch**（選擇 `main` 分支與 `/ (root)`）並儲存，約 1 分鐘後即可獲得免費網址！

### ⚡ 推薦高速免費模型清單
OpenRouter 的 `:free` 模型完全免費（免綁定信用卡，每分鐘上限 20 次請求；每日上限 50 次，若曾儲值過 $10 美金則永久提升至每日 1,000 次）。由於免費節點會不定期輪替，預設使用 `openrouter/free` 自動路由以確保最佳穩定度與速度。

| 模型 ID | 適用場景 | 上下文長度 | 備註 |
| :--- | :--- | :--- | :--- |
| `openrouter/free` | **日常通用／最穩定（預設）** | 動態 | 自動選擇當下可用且快速的免費模型 |
| `nvidia/nemotron-3.5-super-vl:free` | **高速問答與長文** | 1M | 回應速度極快（約 0.7–0.9 秒） |
| `nvidia/nemotron-3.5-lightning:free` | **極速對話** | 1M | 專為低延遲快速回應最佳化 |
| `nvidia/nemotron-3-ultra-550b-a55b:free` | **深度推理與邏輯** | 1M | 550B 參數級強大推理模型 |
| `cohere/north-mini-code:free` | **程式設計與除錯** | 256K | 專精程式碼生成的輕量模型 |
| `google/gemma-4-31b-it:free` | **多語言與繁中寫作** | 262K | 中英文語意理解與翻譯表現優異 |
| `google/gemma-4-26b-a4b-it:free` | **輕快全能助手** | 262K | 速度與品質均衡的通用模型 |

### 🎨 Vibe Coding 修改指南
`index.html` 內部已將程式碼劃分為 4 個清楚區塊，並在 `<script>` 最上方提供集中管理的 `CONFIG` 設定物件。你可以直接將檔案交給 AI 並下達類似指令：
- *「幫我把 `CONFIG.APP_TITLE`、`STARTER_PROMPTS` 和 `DEFAULT_SYSTEM_PROMPT` 改成繁體中文的法律諮詢小助手。」*
- *「修改 `:root` 的 CSS 變數，把整體配色改成溫暖的米白色搭配墨綠色。」*
- *「在聊天輸入框上方加上幾個快捷指令按鈕，例如：翻譯成英文、幫我潤稿、條列重點。」*

> **隱私提醒**：使用 `:free` 免費模型時，部分模型供應商可能會將提示詞用於模型訓練，請勿在對話或知識庫中輸入機密或個人敏感資料。
