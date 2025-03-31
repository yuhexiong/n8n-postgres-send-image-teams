# N8N Postgres Send Image Teams

部署 n8n 並編寫一個工作流程，讓它每天自動呼叫 API 取得狗狗圖片並將其發送到 Microsoft Teams。 

## Overview

- 工具: n8n v1.82.3


## Run

### Run Docker
```
docker compose up -d
```
伺服器運行於 `http://localhost:5678`.  

## UI


1. 創建一個新的工作流程並從檔案導入: [dog_image.json](./dog_image.json)。
2. 使用 Microsoft Teams 的 `incoming webhook` 來獲取 API URL 並在節點中更新它。
3. 啟動工作流程。

![UI](./ui.png)


## References

- [The Dog API](https://thedogapi.com/)