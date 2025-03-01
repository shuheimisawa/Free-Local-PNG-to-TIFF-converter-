# PNG to TIFF Converter

A lightweight, browser-based tool that converts PNG images to TIFF format without uploading files to any server. All processing happens locally in your browser.

![image](https://github.com/user-attachments/assets/b9cae910-0777-4126-a85f-542042566f5f)

## Features

- ✅ Batch convert multiple PNG files at once
- ✅ No server uploads - 100% client-side processing
- ✅ Download individual TIFF files or all as ZIP
- ✅ Preserves image quality and dimensions
- ✅ Works offline after initial page load
- ✅ Fast conversion using WebAssembly-optimized libraries

## Usage

1. Select PNG files using the file picker or drag-and-drop
2. Review your selected files in the preview grid
3. Click "Convert to TIFF" to process all files
4. Download individual TIFF files or all as a ZIP archive

## Installation

### Option 1: Direct download

1. Download or clone this repository
2. Open `index.html` in any modern browser

### Option 2: Using npm

```bash
# Install dependencies
npm install

# Start development server
npm start

# Build for production
npm run build
```

## How It Works

This converter uses the following key technologies:

- [UTIF.js](https://github.com/photopea/UTIF.js) - For TIFF encoding
- [JSZip](https://stuk.github.io/jszip/) - For creating ZIP archives
- [TailwindCSS](https://tailwindcss.com/) - For styling
- HTML5 Canvas API - For image processing

The conversion process:
1. Load PNG into an HTML Canvas
2. Extract raw pixel data from the Canvas
3. Process with UTIF.js to create TIFF format
4. Generate downloadable files

## Browser Compatibility

- ✅ Chrome (recommended)
- ✅ Firefox
- ✅ Edge
- ✅ Safari
- ✅ Opera

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

- [UTIF.js](https://github.com/photopea/UTIF.js) for the TIFF encoding library
- [JSZip](https://stuk.github.io/jszip/) for the ZIP creation functionality
- [TailwindCSS](https://tailwindcss.com/) for the utility-first CSS framework
