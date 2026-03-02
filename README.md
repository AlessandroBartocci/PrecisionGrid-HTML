# 📏 PrecisionGrid-HTML

**Ultra-lightweight millimetric grid generator for high-precision printing.**

Stop fighting with Excel crashes, memory errors, or approximate measurements. This tool leverages native browser vector rendering to generate millimetric grids that are 100% accurate on paper.

## 🚀 Why PrecisionGrid?

*   **True Metric Precision:** Uses native CSS `mm` units. 1cm on screen = 1cm on paper.
*   **Zero Installation:** A single, portable HTML file. Works in any modern browser (Chrome, Edge, Firefox).
*   **Crash-Proof:** Optimized to render long vector lines instead of thousands of individual cells. No more "Out of Memory" errors.
*   **Built-in Safety Margins:** Automatically includes a 5mm "safe zone" to prevent printers from clipping the grid edges.
*   **Instant Layouts:** Switch between A4 and A3 (Portrait/Landscape) with one click.

## 🛠️ How to Use

1.  Download the `Grid.html` file.
2.  Open it with your browser (Chrome or Edge recommended).
3.  Enter your desired square size (e.g., `5` for 5x5mm).
4.  Click **PRINT**.

### ⚠️ Critical Print Settings (IMPORTANT)

To ensure the measurements remain 100% accurate, you **MUST** configure these in the browser print dialog:

*   **Margins:** Set to `None` (or `Nessuno`). The code already handles the 5mm safety margin.
*   **Scale:** Set to `100%` (or `Default`). **DO NOT** use "Fit to page" or "Fit to area".
*   **Background Graphics:** Not strictly required (lines are rendered as real objects), but recommended for better visibility.

## 📂 Project Structure

*   `Grid.html`: The main application (HTML5/CSS3/JavaScript).
*   `README.md`: This documentation file.

## 📄 License

Distributed under the MIT License. Feel free to use, modify, and share.

---
*Created to solve the limitations of spreadsheet-based grid printing.*
