# Substance Painter Custom Exporter

A specialized plugin for Adobe Substance Painter that provides a custom interface for batch exporting texture maps with fine-grained control over resolution, format, and UDIM selection.

## Features

- **Custom UI**: Integrates directly into the Substance Painter interface with a dedicated dock widget and toolbar button.
- **Batch Exporting**: Streamlines the process of exporting multiple texture sets or UDIMs simultaneously.
- **Flexible Configuration**:
    - **Resolution Control**: Export at document resolution or override with custom dimensions.
    - **Format Selection**: Support for various image formats (e.g., TIFF, PNG).
    - **Bit Depth**: Adjustable bit depth (8-bit, 16-bit) for high-quality maps.
- **UDIM Filtering**: Easily toggle which UDIMs or texture sets to include in the export process.
- **Preset Integration**: Works with existing Substance Painter export presets (e.g., PBR MetalRough).
- **Console Logging**: Provides detailed feedback and error reporting via the Substance Painter log.

## Project Structure

- `main.qml`: The plugin's entry point, handling application lifecycle events and UI integration.
- `export.js`: Core logic for interacting with the Substance Painter API (`alg.mapexport`, `alg.resources`).
- `dockWidget.qml`: Defines the main user interface for export settings and UDIM selection.
- `button.qml`: Simple toolbar button to toggle the plugin's visibility.

## How to Install

1.  Locate your Substance Painter plugins folder (usually in `Documents/Allegorithmic/Substance Painter/python/plugins` or similar, though this is a JavaScript/QML plugin).
2.  Copy the contents of this repository into a new folder within the `plugins` directory.
3.  Restart Substance Painter or use the **Plugins -> Reload Plugins** option.

## Usage

1.  Open the **Custom Exporter** dock widget from the Substance Painter UI.
2.  Configure your export directory, file format, and resolution.
3.  Select/deselect the texture sets (UDIMs) you wish to export.
4.  Click the export button to begin the batch process.

---
*Developed to enhance the texture export workflow in Substance Painter.*
