# Images2.0 from ChatGPT プロンプトメーカー

![スクリーンショット](example_screenshot.png)

🌸 ChatGPT の画像生成向けに、自然文プロンプトを組み立てるための静的Webアプリです。  
入力欄、ランダム生成、プリセット、履歴保存を使って、イラスト用プロンプトを整理できます。

[日本語](#jp-日本語) | [English](#en-english) | [繁體中文](#tw-繁體中文台灣) | [Español](#es-español)

---

## JP 日本語

### ✨ 主な機能
- 📝 テーマ、キャラクター、衣装、構図、光、ネガティブなどを項目ごとに編集
- 🎲 各項目のランダム生成と、保存したプールからの呼び出し
- 💾 プリセット、履歴、ユーザー追加プールをブラウザ内に保存
- 📤 JSONでプリセットや履歴をエクスポート・インポート
- 📱 PWA対応。ホーム画面に追加してアプリ風に利用可能

### 🧑‍🏫 かんたんな使い方
1. 🌐 GitHub Pagesのページをブラウザで開きます。
2. 📝 `入力・調整` で、イラストテーマ、キャラクター、衣装、構図などを書きます。
3. 🎲 迷った項目はサイコロボタンを押すと、ランダムで文章が入ります。
4. 📋 保存済みの文章を使いたい時は、メモのようなボタンからプールを開いて選びます。
5. 💾 よく使う文章は、フロッピーディスクのボタンでプールに保存できます。
6. 🎚️ `強度設定` で、アニメ感、迫力、エフェクト、ノイズ抑制などを調整します。
7. 👀 右側の `完成プロンプト` を確認します。入力を変えると自動で更新されます。
8. 📋 `全文コピー` を押して、ChatGPTの画像生成画面に貼り付けます。
9. ⭐ 気に入った状態は `プリセット` に保存すると、あとで同じ設定を呼び出せます。
10. 🕘 当たりプロンプトは `履歴` に保存しておくと、あとで見返せます。

### 💡 ボタンの意味
- 🎲 ランダム：その項目だけ別の文章に変えます。
- 📋 プール：保存済み・内蔵候補から文章を選びます。
- 💾 保存：今の文章を自分用のプールに保存します。
- ✨ 最適化：文章の余分な空白などを整え、安定しやすい設定にします。
- 🧹 全クリア：入力内容をまとめて消します。押す前に確認が出ます。

### 🔒 データ保存について
- 入力内容、履歴、プリセット、追加プールはブラウザの `localStorage` に保存されます。
- サーバー同期、アカウント同期、クラウド保存はありません。
- ブラウザのデータ削除や別端末利用では、保存内容は引き継がれません。

### 🧭 利用上のメモ
- このツールは画像生成プロンプト作成を補助する個人制作ツールです。
- ChatGPT、OpenAI、niji journey など各サービスの公式ツールではありません。
- 体型やシルエット表現の候補がありますが、全年齢向け・センシティブ回避を意識した表現で使う想定です。

### 🚀 GitHub Pagesで使う
このリポジトリをGitHub Pagesで公開すると、`index.html` をそのままWebアプリとして利用できます。

### 🔄 更新時の注意
公開後に `index.html`、`manifest.webmanifest`、アイコンなどを更新した場合は、`sw.js` の `CACHE_NAME` を変更すると、PWAキャッシュが更新されやすくなります。

## ☕ Support

このプロジェクトが役に立った場合は、Ko-fiで今後の開発を応援していただけると嬉しいです。

☕ https://ko-fi.com/puniq

ご支援ありがとうございます！
---

## EN English

### ✨ Features
- 📝 Edit prompt parts such as theme, character, costume, composition, lighting, and negative prompts
- 🎲 Randomize fields and reuse saved prompt pools
- 💾 Save presets, history, and custom pools in the browser
- 📤 Export and import presets/history as JSON
- 📱 PWA-ready, so it can be added to a home screen

### 🧑‍🏫 Simple How to Use
1. 🌐 Open the GitHub Pages site in your browser.
2. 📝 In `Input & Adjust`, write the theme, character, costume, composition, and other details.
3. 🎲 If you are not sure what to write, press a dice button to fill that field randomly.
4. 📋 To reuse saved text, open the pool button and choose an item.
5. 💾 To save useful text, press the floppy disk button and add it to your pool.
6. 🎚️ Use strength settings to adjust anime style, impact, effects, noise control, and more.
7. 👀 Check the `Final Prompt` area. It updates automatically when you edit the fields.
8. 📋 Press `Copy All` and paste the prompt into ChatGPT image generation.
9. ⭐ Save favorite setups as presets so you can load them again later.
10. 🕘 Save good prompts to history so you can review or reuse them later.

### 💡 Button Guide
- 🎲 Random: replaces only that field with another prompt text.
- 📋 Pool: lets you choose from built-in or saved prompt text.
- 💾 Save: saves the current field text to your personal pool.
- ✨ Optimize: cleans up spacing and adjusts settings for more stable results.
- 🧹 Clear All: clears the current inputs after a confirmation.

### 🔒 Data Storage
- Inputs, history, presets, and custom pools are stored in the browser `localStorage`.
- There is no server sync, account sync, or cloud storage.
- Saved data will not automatically move across browsers or devices.

### 🧭 Notes
- This is a personal prompt-helper tool for image generation workflows.
- It is not an official tool from ChatGPT, OpenAI, niji journey, or related services.
- Some prompt pools mention body shape and silhouette, but the intended use is all-ages and avoids sensitive explicit content.

### 🚀 GitHub Pages
When published with GitHub Pages, this repository works as a static web app using `index.html`.

### 🔄 Updating
After publishing, if you update `index.html`, `manifest.webmanifest`, icons, or other cached files, change the `CACHE_NAME` in `sw.js` so PWA caches refresh more reliably.

## ☕ Support

If you find this project useful and would like to support future development, you can support me on Ko-fi.

☕ https://ko-fi.com/puniq

Thank you for your support!
---

## TW 繁體中文（台灣）

### ✨ 主要功能
- 📝 分項編輯主題、角色、服裝、構圖、光線、負面提示詞等內容
- 🎲 可隨機產生各欄位，也可從已儲存的提示詞池呼叫
- 💾 將預設、歷史紀錄、使用者自訂提示詞池儲存在瀏覽器中
- 📤 支援以 JSON 匯出、匯入預設與歷史紀錄
- 📱 支援 PWA，可加入主畫面像 App 一樣使用

### 🧑‍🏫 簡單使用方法
1. 🌐 用瀏覽器打開 GitHub Pages 頁面。
2. 📝 在 `輸入・調整` 裡填寫主題、角色、服裝、構圖等內容。
3. 🎲 不知道要寫什麼時，可以按骰子按鈕，讓系統隨機填入文字。
4. 📋 想使用已儲存的文字時，按池子按鈕，從清單中選擇。
5. 💾 常用的文字可以按磁碟按鈕，存到自己的提示詞池。
6. 🎚️ 用強度設定調整動畫感、魄力、特效、降噪等方向。
7. 👀 右側的 `完成提示詞` 會自動更新，可以確認最後結果。
8. 📋 按 `全文複製`，再貼到 ChatGPT 的圖片生成畫面。
9. ⭐ 喜歡的設定可以存成預設，之後一鍵叫回來。
10. 🕘 好用的提示詞可以存到歷史紀錄，之後再看或再用。

### 💡 按鈕說明
- 🎲 隨機：只替換該欄位的文字。
- 📋 池子：從內建或自己儲存的文字中選擇。
- 💾 儲存：把目前欄位的文字存到自己的池子。
- ✨ 最佳化：整理多餘空白，並調整成較穩定的設定。
- 🧹 全部清除：確認後清空目前輸入內容。

### 🔒 資料儲存
- 輸入內容、歷史紀錄、預設與自訂提示詞池會儲存在瀏覽器的 `localStorage`。
- 沒有伺服器同步、帳號同步或雲端儲存。
- 若清除瀏覽器資料，或在其他裝置使用，資料不會自動同步。

### 🧭 使用說明
- 這是個人製作的圖片生成提示詞輔助工具。
- 本工具不是 ChatGPT、OpenAI、niji journey 或相關服務的官方工具。
- 部分提示詞池包含體型與輪廓描述，但預期用途是全年齡並避免敏感露骨內容。

### 🚀 GitHub Pages
透過 GitHub Pages 發佈後，這個 repository 可以直接以 `index.html` 作為靜態 Web App 使用。

### 🔄 更新提醒
公開後若更新 `index.html`、`manifest.webmanifest`、圖示或其他快取檔案，建議修改 `sw.js` 的 `CACHE_NAME`，讓 PWA 快取更容易更新。

## ☕ Support

如果這個專案對您有幫助，歡迎透過 Ko-fi 支持後續開發。

☕ https://ko-fi.com/puniq

感謝您的支持！
---

## ES Español

### ✨ Funciones principales
- 📝 Edita partes del prompt como tema, personaje, vestuario, composición, luz y prompt negativo
- 🎲 Genera campos al azar y reutiliza pools de prompts guardados
- 💾 Guarda presets, historial y pools personalizados en el navegador
- 📤 Exporta e importa presets e historial como JSON
- 📱 Compatible con PWA para añadirlo a la pantalla de inicio

### 🧑‍🏫 Uso fácil
1. 🌐 Abre la página de GitHub Pages en tu navegador.
2. 📝 En `Entrada y ajustes`, escribe el tema, personaje, vestuario, composición y otros detalles.
3. 🎲 Si no sabes qué escribir, pulsa el botón de dado para rellenar ese campo al azar.
4. 📋 Para usar texto guardado, abre el botón de pool y elige una opción.
5. 💾 Para guardar texto útil, pulsa el botón de disquete y añádelo a tu pool.
6. 🎚️ Usa los ajustes de fuerza para cambiar estilo anime, impacto, efectos, reducción de ruido y más.
7. 👀 Mira el área de `Prompt final`. Se actualiza automáticamente al editar los campos.
8. 📋 Pulsa `Copiar todo` y pega el prompt en la generación de imágenes de ChatGPT.
9. ⭐ Guarda tus configuraciones favoritas como presets para cargarlas después.
10. 🕘 Guarda buenos prompts en el historial para revisarlos o reutilizarlos.

### 💡 Guía de botones
- 🎲 Aleatorio: cambia solo ese campo por otro texto.
- 📋 Pool: permite elegir texto integrado o guardado.
- 💾 Guardar: guarda el texto actual en tu pool personal.
- ✨ Optimizar: limpia espacios y ajusta opciones para resultados más estables.
- 🧹 Borrar todo: borra las entradas actuales después de confirmar.

### 🔒 Almacenamiento de datos
- Las entradas, el historial, los presets y los pools personalizados se guardan en `localStorage` del navegador.
- No hay sincronización con servidor, cuenta ni nube.
- Los datos no se transfieren automáticamente entre navegadores o dispositivos.

### 🧭 Notas de uso
- Esta es una herramienta personal para ayudar a crear prompts de generación de imágenes.
- No es una herramienta oficial de ChatGPT, OpenAI, niji journey ni servicios relacionados.
- Algunos pools mencionan forma corporal y silueta, pero el uso previsto es para todo público y evita contenido explícito sensible.

### 🚀 GitHub Pages
Al publicarlo con GitHub Pages, este repositorio funciona como una app web estática usando `index.html`.

### 🔄 Actualizaciones
Después de publicar, si actualizas `index.html`, `manifest.webmanifest`, iconos u otros archivos cacheados, cambia el `CACHE_NAME` en `sw.js` para que la caché PWA se actualice con más fiabilidad.

## ☕ Support

Si este proyecto te resulta útil y deseas apoyar su desarrollo futuro, puedes apoyarme en Ko-fi.

☕ https://ko-fi.com/puniq

¡Muchas gracias por tu apoyo!
