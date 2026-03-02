# PrecisionGrid-HTML

A lightweight, high-precision millimetric grid generator for printing.

This tool solves common scaling and memory issues found in spreadsheet-based grid generators. It uses native CSS millimetric units and vector rendering to ensure 1:1 physical accuracy on paper.

## Features

- **Metric Precision:** Uses native `mm` units. 1cm on screen corresponds to 1cm on paper.
- **Memory Efficient:** Renders optimized vector lines instead of individual cells to prevent browser or system crashes.
- **Portable:** Single HTML file. No dependencies, no installation required. Works in Chrome, Edge, and Firefox.
- **Safety Margins:** Hardcoded 5mm safety buffer to prevent printer clipping.
- **Multi-Format:** Instant switching between A4/A3 and Portrait/Landscape layouts.

## Usage

1. Open `index.html` in a web browser.
2. Enter the desired square dimensions (e.g., `5` for 5x5mm).
3. Click **PRINT**.

### Critical Print Settings

To maintain physical accuracy, the following browser print settings are mandatory:

- **Margins:** Set to **None**. (The 5mm safety margin is already handled by the code).
- **Scale:** Set to **100%** (or **Default**). Do not use "Fit to page".

## Technical Specifications

- **Engine:** HTML5 / CSS3 / Vanilla JavaScript.
- **Rendering:** CSS Grid and absolute positioning for sub-pixel accuracy.
- **Format Support:** A4 (210x297mm), A3 (297x420mm).

## License

Distributed under the MIT License.
