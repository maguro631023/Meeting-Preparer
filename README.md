# Meeting Preparer — AI 智能會議準備系統

> 會議前自動整合客戶與交易對手的背景摘要，由 OpenAI GPT 驅動

## ✨ 功能特色

- 🤖 **真實 AI API 串接** — 使用您自己的 OpenAI API Key，呼叫 GPT-4o 生成結構化會議簡報
- 📝 **完整 CRUD** — 建立、檢視、編輯、刪除會議記錄
- 📄 **PDF 匯出** — 一鍵匯出會議簡報為 PDF 檔案（含完整排版）
- 🌙 **深色 / 淺色模式** — 系統偏好自動切換，手動覆寫
- 📱 **響應式設計** — 桌面、平板、手機全面支援
- 🔐 **隱私優先** — API Key 僅存於記憶體，不持久化儲存

## 🚀 快速開始

### 本地開發

```bash
# Clone 此倉庫
git clone https://github.com/<your-username>/meeting-preparer.git
cd meeting-preparer

# 直接在瀏覽器開啟（無需 build）
open meeting-preparer.html
```

### GitHub Pages 部署

1. Fork 或 push 此倉庫至您的 GitHub 帳號
2. 前往 **Settings → Pages**
3. Source 選擇 **GitHub Actions**
4. 推送任何 commit，CI/CD 自動部署

或直接在 **Settings → Pages** 選 `main` branch / `/(root)` 即可。

## 🔑 取得 OpenAI API Key

1. 前往 [platform.openai.com](https://platform.openai.com)
2. 登入後點擊右上角 → **API Keys**
3. 建立新金鑰並複製
4. 在應用程式設定頁面貼上 API Key

## 📁 檔案結構

```
meeting-preparer/
├── meeting-preparer.html      # 主應用程式（單頁）
├── README.md                  # 此說明文件
└── .github/
    └── workflows/
        └── deploy.yml         # GitHub Pages 自動部署
```

## 🛠 技術棧

- **前端**: 純 HTML5 + CSS3 + Vanilla JavaScript（無框架）
- **AI**: OpenAI Chat Completions API (GPT-4o)
- **PDF**: jsPDF + html2canvas（CDN）
- **圖示**: Lucide Icons（CDN）
- **字型**: Satoshi (Fontshare)

## ⚠️ 注意事項

- API Key 僅儲存於瀏覽器記憶體，重新整理後需重新輸入
- 此工具為前端應用，API 呼叫直接從瀏覽器發出（需注意 CORS 與費用）
- 建議生產環境使用後端 Proxy 保護 API Key

## 📄 授權

MIT License
