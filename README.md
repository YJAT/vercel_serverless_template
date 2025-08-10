# Vercel Serverless 專案

簡單的 Vercel Serverless 專案，提供基本的 API 端點和前端頁面，日後可基於此專案快速部署到 Vercel。

## 專案結構

```
vercel_serverless/
├── api/
│   └── index.js          # Serverless API 端點
├── index.html            # 首頁
├── package.json          # 專案設定
└── README.md             # 專案說明
```

## 安裝與設定

### 需求

- Node.js (建議版本 16 或以上)
- npm 或 yarn

### 安裝

```bash
# clone this repo
git clone [your-repository-url]
cd vercel_serverless

# install dependences
npm install

# start server
npm start
```

這將會啟動 `api/index.js` 中的伺服器。

### API 端點

- **GET** `/api`
  - 查詢參數: `name` (可選)
  - 範例: `/api?name=YourName`

### 回應格式

```json
{
  "message": "Hello World!"
}
```

或帶有自定義名稱：

```json
{
  "message": "Hello YourName!"
}
```

## 部署到 Vercel

1. 安裝 Vercel CLI：
```bash
npm i -g vercel
```

2. 部署專案：
```bash
vercel
```