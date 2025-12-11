# Image to G-Code Converter

Convert your images into G-Code for CNC machines and plotters with this simple, static web application.

## 🚀 Live Demo

Visit the live application: [Image to G-Code Converter](https://peb-wvu.github.io/-https-github.com-peb-wvu-barker_wvu-/)

## ✨ Features

- **Image Upload**: Support for JPG, PNG, GIF, and most common image formats
- **Edge Detection**: Automatic edge detection using Sobel operator
- **Customizable Settings**:
  - Edge threshold control
  - Feed rate and draw speed adjustment
  - Resolution options (High/Medium/Low/Very Low)
  - Maximum width configuration
  - Image inversion option
- **Visual Previews**:
  - Original image display
  - Processed image with edge detection
  - G-Code path preview showing the actual toolpath
- **Statistics**: View total commands, estimated time, and file size
- **Download**: One-click download of generated .gcode file
- **100% Static**: No server required, works completely offline

## 🛠️ How to Use

1. **Upload an Image**: Click the "Choose Image" button or drag and drop an image file
2. **Adjust Settings**: Configure the edge threshold, feed rates, resolution, and other parameters
3. **Generate G-Code**: Click the "Generate G-Code" button to process your image
4. **Review Previews**: Check the processed image and G-Code path preview
5. **Download**: Click "Download G-Code File" to save the .gcode file

## 📋 G-Code Settings

- **Edge Threshold** (50-200): Controls the sensitivity of edge detection. Higher values detect fewer edges.
- **Feed Rate** (100-5000 mm/min): Rapid movement speed for non-drawing moves
- **Draw Speed** (100-3000 mm/min): Speed when the pen/tool is down and drawing
- **Resolution** (1-5 px): Step size for scanning the image. Higher values = faster but less detailed
- **Max Width** (10-500 mm): Maximum width of the output in millimeters
- **Invert Image**: Swap black and white pixels before processing

## 🔧 Technical Details

- **Image Processing**: Grayscale conversion → Threshold → Sobel edge detection
- **G-Code Format**: Standard RepRap/Marlin compatible
- **Coordinate System**: Absolute positioning (G90), millimeters (G21)
- **Pen Control**: Uses M3 commands (S0 = pen up, S1000 = pen down)
- **No Dependencies**: Pure HTML/CSS/JavaScript, works offline

## 📦 Deployment

This is a static webpage that can be deployed anywhere:

1. **GitHub Pages**: Already configured - just push to main branch
2. **Any Web Server**: Simply upload `index.html` to any web server
3. **Local Use**: Open `index.html` directly in a browser

## 🤝 Contributing

Feel free to submit issues or pull requests to improve the converter!

## 📄 License

MIT License - Free to use and modify
