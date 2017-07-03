## Practice 1: TODOs

### Requirement

- 可建立數個 TodoList
- 可修改單一 TodoList title
- 可刪除單一 TodoList
- 每個 TodoList 內有數個 TodoItem
- 可新增刪除任意 TodoItem
- 可勾選已完成的 TodoItem
- 統計並顯示所有 TodoList 上未完成的 TodoItem 數量
- 統計並顯示所有 TodoList 上已完成的 TodoItem 數量

### 建議有這四個 component

- TodoApp - 掌管所有 state
- TodoList - 一個 todo list
- TodoItem - 一個 todo
- CountDisplay - 顯示 todo 數量狀態

### Hint

用 component 的角度思考，   
先建出一個足夠顯示上述 UI 的資料當做 TodoApp initial state   
只有 TodoApp 是 stateful component (有 state) 的版本，其他 componet 都接收它傳下去的 props

### UI
  
- [參考](http://i.imgur.com/G6Sc083.png)
- 樣式不限

### 繳交方式
- 上傳到 github repo 並設定 gh-pages
- 期限 7/16

## Practice 2: 留言板

> 沒有登入系統跟資料庫的留言板

### Requirement

- 後台必須使用 express (or koa)

### data

- 維護在後台 server 上
- 用一個變數儲存 (server 重啟後消失是正常的)

```js
const data = {};
```
- data 上面應該必須擁有足以顯示畫面所需的資料
- 透過 api 可以存取操作 data 

### api

- `GET /api/comments` 取得所有評論
- `POST /api/comments` 新增評論
- 格式 JSON，參數以及結構自定

### UI 

- 透過 `fetch` 或是 `axios` 跟 API 溝通
- 顯示留言時間
- 顯示留言內容
- 可以新增留言
- 新增的留言會出現在畫面上
- (Advanced) 巢狀結構

### UI 參考
- Hacker News

![](https://i.imgur.com/90afgks.png)

- Facebook Comments Plugin

![](https://ps.w.org/lazy-facebook-comments/trunk/screenshot-3.png?rev=1631157)

- Disqus

![](https://www.sketchappsources.com/resources/source-image/bstefan_disqus.png)

- 樣式不限

### 繳交方式
- 上傳到 github repo 並利用 zeit/now (或其他雲端資源) 進行 deploy
- 期限 7/23

## Practice 3: 部落格

> 實作串接資料庫系統的部落格

### Requirement
- 需連接 database（種類不限）
- 需實現所見及所得編輯
- 實作 Restful API

### UI
- 發文頁面
- 文章總欄頁面（advance: 分頁）
- 單一文章頁面（advance: 留言功能）

### Optional
- 登入系統

### 繳交方式
- 上傳到 github repo 並利用 Heroku (或其他雲端資源) 進行 deploy
- 期限 7/30

