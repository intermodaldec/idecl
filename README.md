# IDEC 公司網站

Intermodal Decoration Engineering Company Limited 官方網站，純靜態 HTML，可直接部署到 GitHub Pages。

## 檔案結構

```
/
├── index.html    # 網站主頁（單文件自包含，CSS/JS 全部內嵌）
└── README.md     # 本說明檔
```

## 部署到 GitHub Pages 步驟

### 方法一：網頁上傳（最簡單）

1. 登入 GitHub，按右上角 **+** → **New repository**
2. Repository name 隨意（例如 `idec-website`），設定為 **Public**，按 **Create repository**
3. 進入倉庫後，按 **uploading an existing file**
4. 將 `index.html` 拖入上傳區，按 **Commit changes**
5. 進入倉庫 **Settings** → 左邊選 **Pages**
6. **Source** 揀 `Deploy from a branch`
7. **Branch** 揀 `main`，資料夾揀 `/ (root)`，按 **Save**
8. 等待 1-3 分鐘，網站就會上線，網址格式：
   `https://你的用戶名.github.io/idec-website/`

### 方法二：Git 指令

```bash
git init
git add index.html
git commit -m "Initial commit"
git branch -M main
git remote add origin https://github.com/你的用戶名/idec-website.git
git push -u origin main
```

然後 follow 方法一嘅步驟 5-8 開啟 Pages。

## 網站內容

- **公司簡介**：IDEC 公司介紹、核心價值
- **服務項目**：6 大服務（室內裝修、樓宇維修、防水、電力、泥水、項目管理）
- **專業團隊**：5 位項目經理資料（姓名、職位、電話、電郵）
- **工程案例**：3 個精選項目展示
- **聯絡我們**：公司地址、電郵、電話、查詢表單（提交後自動開啟郵件客戶端）

## 修改內容

直接用文字編輯器打開 `index.html`，搜尋對應文字修改即可。
- 公司資料：搜尋 `Intermodal Decoration`
- 團隊成員：搜尋 `team-card`
- 聯絡資料：搜尋 `contact-item`

## 注意事項

- 查詢表單使用 `mailto:` 方式，提交後會開啟用戶嘅郵件軟件，發送到 `info@idecl.hk`
- 如需要真正嘅後端表單接收，可接入 Formspree、Netlify Forms 等第三方服務
- 網站已做響應式設計，手機、平板、電腦都正常顯示
