# Release Notes

[日本語](#jp-日本語) | [English](#en-english)

---

## JP 日本語

### 🎉 Version 7.2.0

**Updated: 2026-07-26**

Images2.0 from ChatGPT プロンプトメーカー v7.2.0では、ブラウザ変更時にもデータを共有できるローカルJSON保存を追加しました。

### 💾 ローカル保存

- `start_images2_prompt_manager.bat`から起動すると、入力内容・強度・プリセット・履歴・ユーザープール・表示設定を`data/images2-prompt-manager.json`へ自動保存
- 変更前の状態を`data/images2-prompt-manager.previous.json`へ自動退避
- ブラウザの`localStorage`も補助キャッシュとして維持
- GitHub Pages版と`index.html`直接起動は、従来どおりブラウザ保存で動作
- 入力・強度・プリセット・履歴・ユーザープール・表示設定をまとめた全データバックアップ／復元を追加
- 対応ブラウザでは、全データ・履歴・プリセットのJSON保存先とファイル名を選択可能

### 🔄 旧データ移行

- ローカルJSONが空の場合だけ、旧ブラウザのデータを自動移行
- 新しいブラウザが先に開いても、初期状態で旧データを上書きしない安全策を追加
- BAT起動後、旧ブラウザで`http://localhost:4175/`を開くことで移行可能

### 🚀 起動・ドキュメント

- Node.jsだけで動くローカルサーバーとWindows用BATを追加
- サーバーの起動完了を待ってからブラウザを開くよう対応
- 通常保存の成功表示や移行案内は常駐させず、ブラウザ保存・エラー時だけ小さな表示を追加
- READMEへ初心者向けNode.js導入、BAT起動、移行、バックアップ手順を4言語で追加
- PWAキャッシュをv7.2.0向けに更新

---

### 🎉 Version 7.1.0

**Updated: 2026-06-04**

Images2.0 from ChatGPT プロンプトメーカー v7.1.0 では、公開準備、PWA対応、UI調整、プロンプト編集体験の改善をまとめて行いました。

### ✨ 新機能・追加

- 🧰 **自由記入欄のプール対応**  
  自由記入欄でも、内容の保存・プールからの呼び出し・ランダム差し替えが使えるようになりました。

- 🎲 **描画スタイル / クオリティ強化 / ネガティブプロンプトのランダム対応**  
  3項目にもランダム候補とプール選択を追加しました。

- 📱 **PWA用PNGアイコンを追加**  
  `192x192` と `512x512` のPNGアイコンを追加し、PWA表示の安定性を上げました。

- 📚 **READMEを追加**  
  日本語、英語、繁體中文（台灣）、スペイン語の4言語READMEを作成しました。

- 📝 **リリースノートを追加**  
  v7.1.0 の変更点を日本語・英語でまとめました。

### 🎨 UI改善

- 🧩 **項目右側のアイコンボタンを統一**  
  🎲 / 📋 / 💾 ボタンの幅・高さを揃えました。

- 🪟 **プールモーダルの表示位置と角丸を調整**  
  モーダルを中央寄せにし、角丸を `13px` に統一しました。

- 🧱 **ヘッダーの見た目を変更**  
  ピンク背景、強めのぼかし、白文字に変更しました。

- 🏷️ **編集パネル / 完成プロンプト見出しを強調**  
  見出しのフォントサイズとウェイトを上げ、補足テキストを削除しました。

- 📐 **プロンプト入力欄の高さを調整**  
  入力しやすい高さに広げつつ、過度に大きくなりすぎないよう再調整しました。

- 📱 **モバイル表示を整理**  
  モバイルではタブ・入力ツールバーの固定を解除し、完成プロンプト側の重複ボタンを非表示にしました。

- 🧲 **sticky要素の隙間を調整**  
  スクロール時にヘッダーと固定要素の間に出る微妙な隙間を詰めました。

### 🧠 プロンプト生成・保存まわり

- 👻 **空欄項目を完成プロンプトから除外**  
  入力が空の項目は、見出しごと完成プロンプトに出ないようにしました。

- ↩️ **ネガティブプロンプト仕様を復元**  
  ネガティブON/OFFまわりの文言を以前の仕様に戻しました。

- 💾 **Service Workerキャッシュを更新**  
  `CACHE_NAME` を `v710` に変更し、追加アイコンもキャッシュ対象に含めました。

### 🛠️ 公開準備

- 🌐 **GitHub Pages向けのREADME整備**  
  ブラウザ保存、PWAキャッシュ、非公式ツールであること、利用上の注意をREADMEに記載しました。

- 🔒 **保存仕様を明記**  
  履歴・プリセット・ユーザープールはブラウザの `localStorage` に保存され、サーバー同期はないことを説明しました。

---

## EN English

### 🎉 Version 7.2.0

**Updated: 2026-07-26**

Images2.0 from ChatGPT Prompt Maker v7.2.0 adds browser-independent local JSON storage while preserving the existing GitHub Pages experience.

### 💾 Local Storage

- Launching with `start_images2_prompt_manager.bat` automatically saves inputs, strengths, presets, history, user pools, and display settings to `data/images2-prompt-manager.json`
- Automatically keeps the previous state in `data/images2-prompt-manager.previous.json`
- Retains browser `localStorage` as a secondary cache
- GitHub Pages and direct `index.html` continue to use browser-only storage
- Added full backup and restore for inputs, strengths, presets, history, user pools, and display settings
- Supported browsers can choose the destination and file name for full-data, history, and preset JSON exports

### 🔄 Legacy Data Migration

- Automatically migrates legacy browser data only when local JSON is empty
- Prevents a new browser's initial state from replacing recoverable old data
- Old data can be migrated by opening `http://localhost:4175/` in the previous browser while the BAT is running

### 🚀 Startup & Documentation

- Added a dependency-free Node.js local server and Windows BAT launcher
- Waits for the server before opening the browser
- Keeps success and migration notices out of the way, showing a compact notice only for browser-only storage or errors
- Added beginner-friendly Node.js, BAT, migration, and backup instructions in four README languages
- Updated the PWA cache for v7.2.0

---

### 🎉 Version 7.1.0

**Updated: 2026-06-04**

Images2.0 from ChatGPT Prompt Maker v7.1.0 focuses on release preparation, PWA support, UI polish, and a smoother prompt editing experience.

### ✨ New Features

- 🧰 **Custom free-text pool support**  
  The free-text field now supports saving, selecting from a pool, and random replacement.

- 🎲 **Random pools for style, quality, and negative prompts**  
  Drawing style, quality enhancement, and negative prompt fields now include random candidates and pool selection.

- 📱 **Added PWA PNG icons**  
  Added `192x192` and `512x512` PNG icons for more stable PWA installation and display.

- 📚 **Added README**  
  Added a multilingual README in Japanese, English, Traditional Chinese for Taiwan, and Spanish.

- 📝 **Added release notes**  
  Added bilingual release notes for v7.1.0.

### 🎨 UI Improvements

- 🧩 **Unified field action buttons**  
  Standardized the size of 🎲 / 📋 / 💾 buttons.

- 🪟 **Improved pool modal layout**  
  Moved the modal closer to the center and unified the border radius to `13px`.

- 🧱 **Updated header design**  
  Changed the header to a pink translucent style with stronger blur and white text.

- 🏷️ **Stronger panel headings**  
  Increased the font size and weight of “Edit Panel” and “Final Prompt” headings, and removed extra side labels.

- 📐 **Adjusted prompt textarea height**  
  Increased the input area height, then tuned it back to a more comfortable size.

- 📱 **Cleaned up mobile layout**  
  Disabled sticky tabs/toolbars on mobile and removed duplicate top buttons in the final prompt area.

- 🧲 **Fixed tiny sticky gaps**  
  Reduced the small visual gap that appeared between the header and sticky elements while scrolling.

### 🧠 Prompt Generation & Storage

- 👻 **Hide empty fields from final prompt**  
  Empty input fields are now omitted from the final prompt, including their section headings.

- ↩️ **Restored negative prompt behavior**  
  Reverted the negative prompt ON/OFF behavior and wording to the previous specification.

- 💾 **Updated Service Worker cache**  
  Changed `CACHE_NAME` to `v710` and added the new PNG icons to the cache list.

### 🛠️ Release Preparation

- 🌐 **Prepared README for GitHub Pages**  
  Documented browser storage, PWA cache behavior, unofficial tool status, and usage notes.

- 🔒 **Clarified storage behavior**  
  Explained that history, presets, and custom pools are stored in browser `localStorage` and are not synced to a server.
