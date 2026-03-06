# PrecisionGrid-HTML

A no-nonsense, high-precision browser tool for designing and printing custom millimetric grids. 

Most spreadsheet software or image editors struggle with physical scaling, often resulting in "almost" 5mm squares that drift across the page. **PrecisionGrid-HTML** uses internal border calculations to ensure that a 10mm cell is exactly 10mm on paper, period.

### Why this?
- **True-to-Life Scaling**: Built using native CSS millimetric units. The math holds up from screen to paper.
- **Interactive Workflow**: Draw, paint, and erase cells directly in the browser. It’s a grid generator and a layout editor in one.
- **Zero Bloat**: A single-file utility. No `npm install`, no tracking, no external dependencies.
- **Print-First Logic**: Automatically clips "partial" cells that wouldn't fit within a safe printing margin, preventing awkward half-squares at the edge of the page.

### Quick Start
1. Download or copy `index.html`.
2. Open it in any modern browser (Chrome/Edge recommended).
3. Define your cell dimensions (e.g., `5 x 5` for standard graph paper).
4. Use the **Pencil** or **Eraser** to customize your layout.
5. Hit **Print**.

### Critical Print Settings
To prevent the browser from shrinking your grid, you **must** use these settings in the print dialog:
*   **Margins**: None
*   **Scale**: 100% (or Default)
*   **Headers/Footers**: Off

### Technical Specifications
- **Engine**: HTML5 / CSS3 / Vanilla JavaScript.
- **Precision logic**: Uses `box-shadow: inset` for borders. This ensures that the border occupies space *inside* the cell, keeping the external dimensions mathematically perfect.
- **Layouts**: Supports A4 Portrait and Landscape.

### License
Distributed under the **MIT License**.
