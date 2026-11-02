# Google Sheets Clone

A web-based spreadsheet application inspired by Google Sheets, built using HTML, CSS, and JavaScript. It provides spreadsheet functionalities such as editable cells, formula evaluation, cell formatting, dependency tracking, and an AI-powered assistant that enables users to interact with spreadsheet data using natural language.

## Project Objective

The objective of this project is to build a functional spreadsheet application from scratch while exploring JavaScript concepts, data structures, graph-based dependency management, formula evaluation, and AI integration.

It combines traditional spreadsheet functionalities with AI-powered natural language interaction to make spreadsheet data analysis more intuitive and accessible.

## Features

### 1. Spreadsheet Functionalities

- **Editable Cells:** Users can select and edit individual cells directly within the spreadsheet.
- **Formula Bar:** Allows users to enter and edit formulas. The calculated result is reflected in the corresponding cell.
- **Cell Formatting:** A toolbar provides basic text formatting options:
  - Bold
  - Italic
  - Underline
- **Address Bar:** Displays the address of the currently selected cell (e.g., A1, B2, C3).
- **Dependency Tracking:** Maintains relationships between dependent cells and tracks how changes in one cell affect other cells.
- **Automatic Recalculation:** Updates dependent cell values whenever their parent cell values change.

### 2. AI-Powered Spreadsheet Assistant

- **AI Assistant Integration:** Users can access the AI assistant through an option in the spreadsheet toolbar.
- **Draggable Interface:** Users can move the AI assistant window across the application.
- **Resizable Input:** The assistant's input area can be resized according to user requirements.
- **Multi-Cell Selection:** Users can select multiple cells to provide spreadsheet data as context for their queries.
- **Natural Language Queries:** Users can ask questions about spreadsheet data using plain English.
- **AI-Generated Results:** The assistant analyzes the selected spreadsheet data and provides results in the desired location within the sheet.

## Tech Stack

- **HTML5:** Structures the spreadsheet interface.
- **CSS3:** Handles styling, layout, and visual presentation.
- **JavaScript (Vanilla JS):** Implements cell operations, formula evaluation, dependency tracking, and application logic.
- **AI Integration:** Enables natural language interaction and AI-powered spreadsheet analysis.

## Data Structures and Models

### 1. Two-Dimensional Array

The spreadsheet is represented using a two-dimensional array, where each element represents an individual cell.

This structure provides an organized way to access and manage spreadsheet data using row and column indices.

### 2. Cell Object Schema

Each cell is represented as an object with the following properties:

```javascript
{
    value: "value of the cell",
    formula: "formula of the cell",
    children: ["list of dependent cells"],
    parents: ["list of parent cells"]
}
```

### 3. Property Description

| Property | Description |
|---|---|
| `value` | Stores the current value or evaluated result of the cell. |
| `formula` | Stores the formula entered by the user, if any. |
| `children` | Stores the cells that depend on the current cell. |
| `parents` | Stores the cells on which the current cell depends. |

### 4. Dependency Management

Dependency tracking is implemented using a directed graph concept.

For example, consider the following spreadsheet:

| Cell | Content |
|---|---|
| A1 | 10 |
| B1 | =A1*2 |

Here:
- `A1` is the parent cell.
- `B1` is the dependent (child) cell.
- `B1` evaluates to `20`.

The dependency relationship is represented as:

```text
A1 → B1
```

When the value of `A1` changes, the application tracks its dependent cells and recalculates their values accordingly.

## Project Structure

```text
GoogleSheet/
│
├── index.html
├── style.css
├── GoogleSheet.js
└── README.md
```

## Getting Started

### Prerequisites

- A modern web browser (Google Chrome, Microsoft Edge, Firefox, etc.).
- Visual Studio Code.
- Live Server extension for VS Code.

**Note:** Node.js and npm are not required to run the current HTML, CSS, and JavaScript application.

### Installation and Setup

1. Clone the repository:

```bash
git clone https://github.com/Isha0016/Google-Sheets-Clone
```

2. Navigate to the project directory:

```bash
cd GoogleSheet
```

3. Open the project folder in Visual Studio Code.

4. Install the Live Server extension.

5. Open `index.html`, right-click, and select **Open with Live Server**.

6. The application will open in your default browser.

## Key Concepts

- Two-dimensional arrays and object modeling.
- Formula parsing and evaluation.
- Directed graphs and dependency management.
- Automatic recalculation of dependent cells.
- DOM manipulation and event handling.
- Cell selection and formatting.
- Multi-cell data handling.
- Draggable and resizable UI components.
- AI integration and natural language interaction.


## 🔮 Future Enhancements

- **Advanced Formula Support:** Introduce additional spreadsheet functions such as SUM, AVERAGE, COUNT, MAX, MIN, and IF.

- **Multiple Worksheets:** Support creating, renaming, and switching between multiple sheets.

- **Undo and Redo:** Allow users to undo and redo spreadsheet operations.

- **Copy and Paste:** Support copying and pasting cell values, formulas, and formatting.

- **Advanced Cell Formatting:** Introduce font customization, background colors, borders, alignment, and number formatting.

- **Data Visualization:** Add charts and graphs to represent spreadsheet data visually.

- **Import and Export:** Support importing and exporting spreadsheet data in CSV and Excel formats.

- **Data Persistence:** Implement storage to preserve spreadsheet data across sessions.

- **AI Enhancements:** Extend the AI assistant to support advanced data analysis, formula generation, data cleaning, and automated spreadsheet operations.

- **Collaboration:** Enable multiple users to work on the same spreadsheet in real time.

## 🤝 Support

If you encounter any issues, have questions, or want to suggest improvements, feel free to:

- Open an issue in the GitHub repository.

- Submit a pull request with improvements or bug fixes.

- Share suggestions for new features and enhancements.

Your feedback and contributions are always welcome!

## 👨‍💻 Author

**Isha**

- GitHub: https://github.com/Isha0016

# ⭐ Project

If you find this project helpful, feel free to explore the repository, share your feedback, or contribute to its improvement.

---