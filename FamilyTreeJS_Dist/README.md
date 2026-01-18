# FamilyTreeJS (家系圖作成)

A lightweight, single-file HTML5 application for creating, managing, and visualizing family trees. Runs entirely in your browser with no installation required.

![License](https://img.shields.io/badge/license-MIT-blue.svg)

## ✨ Features

- **No Installation Needed**: Just open the HTML file in any modern browser.
- **Privacy Focused**: All data is processed locally. No data is sent to any server.
- **Drag & Drop Interface**: Easily rearrange family members and relationships.
- **View Modes**:
  - **Tree View**: Standard hierarchical family tree.
  - **Vertical Mode (直書)**: Traditional East Asian vertical writing layout.
- **Customizable Aesthetics**: Choose from multiple built-in themes (Standard, Chic, Miyabi, Dynasty, etc.) and font styles.
- **Import & Export**:
  - **Excel Support**: Import and export family data using `.xlsx` files.
  - **Image Export**: Save your tree as a high-quality PNG image (supports tiling for large trees).
  - **PDF Export**: Generate PDF documents of your family tree.
  - **SVG Export**: Export scalable vector graphics.
- **Advanced Editing**:
  - Support for multiple partners, adopted children, and complex relationships.
  - Auto-generated IDs with manual override capabilities.
  - Era name support (Japanese, Qing Dynasty, ROC) with automatic Western year conversion.

## 🚀 How to Use

1. **Download**: Download `Family_Tree_CHN.html`.
2. **Open**: Double-click the file to open it in Chrome, Edge, Firefox, or Safari.
3. **Start Creating**:
   - The app loads with sample data. Click "Initialize" (初始化) to reset or reload sample data.
   - **Edit**: Click on any person card to edit details, add parents, spouses, or children.
   - **Move**: Drag and drop cards to rearrange or re-link relationships.
   - **Zoom/Pan**: Use Ctrl + Scroll to zoom, and drag the background to pan.

## 📂 Data Format (Excel)

You can manage your family tree data in Excel and import it. The required columns are:

| Column Header | Description | Example |
|---|---|---|
| **ID** | Unique identifier for the person | `A-1` |
| **世代** | Generation number (1, 2, 3...) | `1` |
| **姓名** | Full Name | `Sun Yat-sen` |
| **性別** | Gender (`male` or `female`) | `male` |
| **父ID** | ID of the father | `A-0` |
| **母ID** | ID of the mother | `A-0=1` |
| **配偶** | Is this node a spouse? (`TRUE`/`FALSE`) | `FALSE` |
| **配偶ID** | ID of the partner (if spouse) | `A-1` |
| **順序** | Birth order among siblings | `1` |
| **關係** | Relation type (`親生` or `養子`) | `親生` |

*(See the built-in sample data for a complete template)*

## 🛠️ Technology Stack

- **Vanilla JavaScript**: Core logic and DOM manipulation.
- **SheetJS (xlsx)**: For Excel file parsing and generation.
- **html2canvas**: For capturing the DOM as images.
- **jsPDF**: For PDF generation.

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

---

# FamilyTreeJS (家系図作成ソフト)

ウェブブラウザだけで動作する、インストール不要の軽量な家系図作成アプリケーションです。

## ✨ 特徴

- **インストール不要**: HTMLファイルをブラウザで開くだけですぐに使えます。
- **プライバシー重視**: データはすべてローカルで処理され、サーバーに送信されることはありません。
- **ドラッグ＆ドロップ操作**: 直感的な操作で家族の配置や関係性を整理できます。
- **表示モード**:
  - **ツリー表示**: 一般的な階層型の家系図。
  - **縦書きモード**: 日本や東アジアの伝統的な縦書きレイアウトに対応。
- **デザインカスタマイズ**: 複数のテーマ（標準、シック、雅、王朝など）やフォントスタイルを選択可能。
- **インポート・エクスポート**:
  - **Excel連携**: `.xlsx`形式でデータの読み込み・保存が可能。
  - **画像出力**: 高品質なPNG画像として保存（分割出力対応）。
  - **PDF出力**: 家系図をPDFドキュメントとして保存。
  - **SVG出力**: ベクター形式での出力に対応。
- **高度な編集機能**:
  - 複数の配偶者、養子縁組、複雑な関係性に対応。
  - ID自動生成（手動での上書きも可能）。
  - 和暦・元号（日本、清朝、中華民国）のサポートと西暦自動変換。

## 🚀 使い方

1. **ダウンロード**: `Family_Tree_CHN.html` をダウンロードします。
2. **開く**: ファイルをダブルクリックして、Chrome, Edge, Firefox, Safariなどのブラウザで開きます。
3. **作成開始**:
   - 初期状態ではサンプルデータが表示されます。「初期化 (初始化)」ボタンでリセット可能です。
   - **編集**: 人物カードをクリックして詳細を編集したり、親・配偶者・子供を追加できます。
   - **移動**: カードをドラッグ＆ドロップして配置や関係を修正できます。
   - **ズーム/移動**: Ctrl + スクロールで拡大縮小、背景をドラッグして画面移動。

## 📂 データ形式 (Excel)

Excelで家系図データを管理し、インポートすることができます。必要な列は以下の通りです：

| 列ヘッダー | 説明 | 例 |
|---|---|---|
| **ID** | 各人物の固有ID | `A-1` |
| **世代** | 世代番号 (1, 2, 3...) | `1` |
| **姓名** | 氏名 | `坂本 龍馬` |
| **性別** | 性別 (`male` または `female`) | `male` |
| **父ID** | 父親のID | `A-0` |
| **母ID** | 母親のID | `A-0=1` |
| **配偶** | 配偶者ノードかどうか (`TRUE`/`FALSE`) | `FALSE` |
| **配偶ID** | パートナーのID（配偶者の場合） | `A-1` |
| **順序** | 兄弟間の出生順 | `1` |
| **關係** | 親子関係 (`親生` または `養子`) | `親生` |

*(詳細なテンプレートは内蔵のサンプルデータを参照してください)*

---

# FamilyTreeJS (家系圖作成)

這是一個輕量級、單文件的 HTML5 應用程序，無需安裝即可在瀏覽器中運行，用於創建、管理和可視化家系圖。

## ✨ 特色

- **無需安裝**: 只需在任何現代瀏覽器中打開 HTML 文件即可。
- **隱私優先**: 所有數據均在本地處理，不會發送到任何服務器。
- **拖放界面**: 輕鬆重新排列家庭成員和關係。
- **顯示模式**:
  - **樹狀視圖**: 標準層級結構家系圖。
  - **直書模式**: 傳統東亞直書排版。
- **自定義外觀**: 內建多種主題（標準、時尚、雅致、王朝等）和字體風格。
- **導入與導出**:
  - **Excel 支持**: 使用 `.xlsx` 文件導入和導出家族數據。
  - **圖片導出**: 將家系圖保存為高質量的 PNG 圖片（支持大圖分割）。
  - **PDF 導出**: 生成家系圖 PDF 文檔。
  - **SVG 導出**: 導出可縮放矢量圖形。
- **高級編輯**:
  - 支持多位配偶、養子和複雜關係。
  - 自動生成 ID，並支持手動覆蓋。
  - 支持年號（日本、清朝、中華民國），並自動轉換西元紀年。

## 🚀 如何使用

1. **下載**: 下載 `Family_Tree_CHN.html`。
2. **打開**: 雙擊文件以在 Chrome、Edge、Firefox 或 Safari 中打開。
3. **開始創建**:
   - 應用加載時會顯示示例數據。點擊「初始化」可重置或重新加載示例數據。
   - **編輯**: 點擊任何人名卡片以編輯詳細信息，或添加父母、配偶或子女。
   - **移動**: 拖放卡片以重新排列或重新鏈接關係。
   - **縮放/平移**: 使用 Ctrl + 滾輪進行縮放，拖動背景進行平移。

## 📂 數據格式 (Excel)

您可以在 Excel 中管理家系圖數據並將其導入。所需列如下：

| 列標題 | 描述 | 示例 |
|---|---|---|
| **ID** | 人物的唯一標識符 | `A-1` |
| **世代** | 世代編號 (1, 2, 3...) | `1` |
| **姓名** | 全名 | `孫中山` |
| **性別** | 性別 (`male` 或 `female`) | `male` |
| **父ID** | 父親的 ID | `A-0` |
| **母ID** | 母親的 ID | `A-0=1` |
| **配偶** | 是否為配偶節點 (`TRUE`/`FALSE`) | `FALSE` |
| **配偶ID** | 伴侶的 ID（如果是配偶） | `A-1` |
| **順序** | 兄弟姐妹中的出生順序 | `1` |
| **關係** | 關係類型 (`親生` 或 `養子`) | `親生` |

*(完整模板請參考內建示例數據)*

---
*Created by Antigravity*
