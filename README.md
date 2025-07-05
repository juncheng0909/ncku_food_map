# 成大人の美食地圖 🍜
歡迎來到「成大人の美食地圖」！這是一個專為成功大學周邊設計的互動式美食推薦網站。使用者可以瀏覽推薦的餐廳、即時投票表達喜好，甚至可以新增自己喜歡的店家，與大家共享美食情報。

專案前端使用純 HTML, CSS, JavaScript 打造，後端與資料庫則由 Google Firebase Realtime Database 提供支援，實現了資料的即時同步。

## 主要功能

*   **瀏覽餐廳列表**：清晰地展示餐廳的基本資訊，包括地址、營業時間和推薦餐點。
*   **即時投票系統**：點擊「👍推」或「👎不推」按鈕，你的選擇會即時更新到資料庫，並同步給所有使用者。
*   **新增美食推薦**：透過右側工具列的「➕新增餐廳」按鈕，任何人都可以將自己喜愛的美食店家新增到列表中。
*   **快速搜尋餐廳**：使用「🔍搜尋餐廳」功能，輸入關鍵字即可快速篩選出想找的店家。
*   **查看地圖**：點擊「查看地圖」按鈕，會直接在新分頁開啟該餐廳的 Google Maps 連結，方便導航。
*   **動態更新**：網站與 Firebase 即時連動，當有人新增餐廳或投票時，你的頁面無需重新整理即可看到最新狀態。

## 📖 使用者指南

1.  **瀏覽與探索**：
    *   進入網站後，你會看到目前已收錄的餐廳列表。
    *   每張卡片都包含了店家的重要資訊。

2.  **分享你的意見**：
    *   如果你喜歡某家餐廳，請點擊「👍 推」按鈕。
    *   如果覺得不合胃口，可以點擊「👎 不推」按鈕。
    *   你會發現數字會立刻變化！

3.  **新增你的私房店家**：
    *   點擊畫面右側的「➕ 新增餐廳」按鈕。
    *   在彈出的視窗中，依序填入餐廳名稱、地址、營業時間、推薦餐點和 Google Maps 連結。
    *   點擊「確認新增」，你的推薦就會出現在大家眼前！

4.  **快速找到目標**：
    *   點擊右側的「🔍 搜尋餐廳」按鈕。
    *   在跳出的輸入框中，輸入店名關鍵字（例如：「拉麵」）。
    *   網站將會自動篩選出符合條件的餐廳。

## 🛠️ 技術

*   **前端**：
    *   HTML5
    *   CSS3
    *   JavaScript (ES6)
*   **後端與資料庫**：
    *   Firebase - Realtime Database

## 🚀 本地開發設定

如果你想在自己的電腦上運行或修改這個專案，請遵循以下步驟：

1.  **複製專案**：
    ```bash
    git clone https://your-repository-url.git
    ```

2.  **設定 Firebase**：
    *   前往 [Firebase 官方網站](https://firebase.google.com/) 並建立你自己的專案。
    *   在專案中啟用 **Realtime Database**。
    *   將你的 Firebase 專案設定物件 (firebaseConfig) 複製下來。

3.  **修改 `index.html`**：
    *   打開 `index.html` 檔案。
    *   找到 `<script>` 標籤內的 `firebaseConfig` 物件。
    *   **用你自己的 Firebase 設定物件取代它**。

    ```javascript
    // 找到這段程式碼，並換成你自己的設定
    const firebaseConfig = {
      apiKey: "YOUR_API_KEY",
      authDomain: "YOUR_AUTH_DOMAIN",
      databaseURL: "YOUR_DATABASE_URL",
      projectId: "YOUR_PROJECT_ID",
      storageBucket: "YOUR_STORAGE_BUCKET",
      messagingSenderId: "YOUR_MESSAGING_SENDER_ID",
      appId: "YOUR_APP_ID"
    };
    ```

4.  **運行網站**：
    *   直接在瀏覽器中打開 `index.html` 檔案即可。
    *   （推薦）使用 VS Code 的 `Live Server` 擴充功能來運行，可以獲得更好的開發體驗。

## 🌟 未來可改進功能

*   使用者登入系統，限制每人對同一餐廳只能投一次票。
*   允許上傳餐廳圖片。
*   更進階的篩選功能（例如：依評分、距離排序）。
*   留言與討論區功能。

---
