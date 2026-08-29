# ls.illusd.com

LessLS 網站，包含首頁與 GitHub OAuth 登入回跳頁面。

## 路由

| 路徑 | 說明 |
|------|------|
| `/home` | LessLS 官網首頁 |
| `/oauth/callback` | GitHub OAuth 登入回跳，顯示授權碼供使用者複製 |

## 登入流程

1. `lss login` → 取得授權連結，跳轉 GitHub
2. GitHub 授權 → 回跳 `https://ls.illusd.com/oauth/callback?code=XXXXX`
3. 頁面顯示授權碼，一鍵複製
4. `lss login XXXXX` 完成登入

## 部署

Vercel：https://ls.illusd.com
