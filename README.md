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

1. **Download**: Download `Family_Tree_1.0_CHN.html`.
2. **Open**: Double-click the file to open it in Chrome, Edge, Firefox, or Safari.
3. **Start Creating**:
   - The app loads with sample data. Click "Initialize" (初始化) to reset or reload sample data.
   - **Edit**: Click on any person card to edit details, add parents, spouses, or children.
   - **Move**: Drag and drop cards to rearrange or re-link relationships.
   - **Zoom/Pan**: Use Ctrl + Scroll to zoom, and drag the background to pan.

## 📂 Data Format (Excel)

You can manage your family tree data in Excel and import it. The required columns are:

| Column Header | Description | Example |
|str|str|str|
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
*Created by Antigravity*
