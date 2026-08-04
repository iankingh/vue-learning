# vue-learning

Vue 2 基礎學習筆記與可直接在瀏覽器開啟的練習頁面。範例透過本地 `js/vue.js` 載入 **Vue.js 2.7.14**，不是 Vue CLI、Vite 或 Vue 3 專案。

## 學習內容

| 路徑 | 內容 |
|---|---|
| `01-vue/vue.html` | 建立空白 `new Vue` instance 與掛載節點 |
| `01-vue/v.vue` | 未接入建置流程的 table 單檔元件草稿，示範 props、`v-for` 與自訂事件 |
| `09-監視屬性-watch/Vue-天氣範例.html` | computed property 與事件切換 |
| `09-監視屬性-watch/Vue-watch.html` | watch 選項範例 |
| `09-監視屬性-watch/Vue-watch-深度監視.html` | 物件的 deep watch |
| `11-列表渲染/基本列表.html` | 使用 `v-for` 渲染陣列與物件 |
| `js/vue.js` | 本地 Vue.js 2.7.14 development build |

## 環境需求與執行

只需現代瀏覽器，不需 Node.js 或 npm：

1. Clone 或下載此倉庫。
2. 直接以瀏覽器開啟任一 `.html` 範例。
3. watch 範例的輸出請在瀏覽器 DevTools Console 查看。

本倉庫沒有 `package.json`、環境變數或安裝步驟，也沒有 dev server、build、test、lint 或 production deployment 設定。

## 專案狀態與限制

- 內容是獨立的 Vue 2 練習片段，不構成單一應用程式。
- `01-vue/v.vue` 需要另行建立支援 Vue SFC 的專案才能編譯；本倉庫未提供該工具鏈。
- `Vue-watch.html` 的 watcher key 目前寫成 `isHo`，因此切換 `isHot` 時不會觸發 watcher；保留為現有練習狀態。
- `基本列表.html` 第二個 `v-for` 的 key 綁定寫成 `::key`，瀏覽器會忽略該錯誤屬性。

## 延伸資源

- [Vue 2 文件](https://v2.vuejs.org/)
- [Vue 官方文件](https://vuejs.org/)
- [重新認識 Vue.js](https://book.vue.tw/)
