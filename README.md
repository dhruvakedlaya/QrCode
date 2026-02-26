# ⚡ Advanced QR Code Generator

A beautiful, feature-rich, and fully responsive QR code generator with a stunning animated UI. Generate QR codes instantly with customizable sizes, colors, and quick-action templates.

![QR Code Generator](https://img.shields.io/badge/version-1.0.0-blue.svg)
![License](https://img.shields.io/badge/license-MIT-green.svg)
![Responsive](https://img.shields.io/badge/responsive-yes-brightgreen.svg)

## ✨ Features

### 🎨 **Stunning Visual Design**
- Animated starfield background with gradient transitions
- Neon glow effects and smooth animations
- Glassmorphism UI with backdrop blur effects
- Fully responsive design that works on all devices

### 🚀 **Core Functionality**
- **Instant QR Generation**: Create QR codes in real-time
- **Multiple Size Options**: Small (150px), Medium (300px), Large (500px), XL (800px)
- **Color Customization**: Choose from 6 preset colors (Black, Cyan, Pink, Red, Purple, Blue)
- **Quick Actions**: Pre-configured templates for:
  - 🌐 Website URLs
  - 📧 Email addresses
  - 📱 Phone numbers
  - 📶 WiFi credentials

### 💾 **Advanced Features**
- **Download QR Codes**: Save as PNG files
- **Share Functionality**: Copy QR code links to clipboard
- **History Tracking**: Automatically saves your last 12 QR codes
- **LocalStorage Integration**: Your history persists across sessions
- **Click-to-Reload**: Quickly regenerate previous QR codes from history

### 📱 **Responsive Design**
- Optimized for mobile devices (phones and tablets)
- Touch-friendly interface with proper touch targets
- Landscape mode support
- Adaptive typography and spacing using `clamp()`
- iOS zoom prevention on form inputs

## 🎯 Demo

Simply open `index.html` in any modern web browser to start generating QR codes!

## 🛠️ Technologies Used

- **HTML5**: Semantic markup
- **CSS3**: Advanced animations, gradients, and transitions
- **Vanilla JavaScript**: No dependencies required
- **QR Server API**: For QR code generation
- **LocalStorage API**: For history persistence

## 📦 Installation

1. **Clone or Download**
   ```bash
   git clone https://github.com/yourusername/qr-code-generator.git
   ```
   Or simply download the `index.html` file.

2. **Open in Browser**
   ```bash
   # No build process required!
   open index.html
   ```
   Or double-click the file to open in your default browser.

## 🎮 Usage

### Basic Usage
1. Enter text, URL, or data in the text area
2. Select your desired QR code size
3. Choose a color scheme
4. Click "GENERATE QR CODE"
5. Download or share your QR code

### Quick Actions
- **Website URL**: Automatically prefills `https://`
- **Email**: Prefills `mailto:` for email QR codes
- **Phone**: Prefills `tel:` for phone numbers
- **WiFi**: Provides WiFi configuration format

### WiFi QR Code Format
```
WIFI:T:WPA;S:NetworkName;P:Password;;
```
- `T`: Security type (WPA, WEP, or nopass)
- `S`: Network SSID (name)
- `P`: Password

### History Feature
- Automatically saves your last 12 QR codes
- Click any history item to reload that QR code
- History persists across browser sessions

## 🎨 Customization

### Change Colors
Modify the color options in the HTML:
```html
<button class="color-btn" data-color="YOUR_HEX" style="background: #YOUR_HEX;"></button>
```

### Adjust Sizes
Change size options in the HTML:
```html
<button class="size-btn" data-size="YOUR_SIZE">Label</button>
```

### Modify Animations
Edit the CSS keyframe animations:
```css
@keyframes yourAnimation {
    /* Your animation properties */
}
```

## 🌐 Browser Support

- ✅ Chrome (latest)
- ✅ Firefox (latest)
- ✅ Safari (latest)
- ✅ Edge (latest)
- ✅ Opera (latest)
- ✅ Mobile browsers (iOS Safari, Chrome Mobile)

## 📱 Mobile Optimization

The app is fully optimized for mobile devices with:
- Touch-friendly buttons (minimum 44px touch targets)
- Responsive grid layouts
- Adaptive font sizing
- iOS zoom prevention on inputs
- Landscape orientation support
- Mobile-specific CSS optimizations

## 🔧 API Reference

### QR Server API
This project uses the free QR Server API:
```
https://api.qrserver.com/v1/create-qr-code/
```

**Parameters:**
- `size`: Width and height in pixels (e.g., `300x300`)
- `data`: URL-encoded content for the QR code
- `color`: Hex color code without the `#` symbol

**Example:**
```
https://api.qrserver.com/v1/create-qr-code/?size=300x300&data=Hello%20World&color=000000
```

## 💡 Tips

1. **For URLs**: Always include `https://` or `http://`
2. **For Emails**: Use `mailto:email@example.com`
3. **For Phone Numbers**: Use `tel:+1234567890`
4. **For WiFi**: Follow the format strictly for device compatibility
5. **Testing**: Always test generated QR codes with your phone before sharing

## 🐛 Troubleshooting

### QR Code Not Generating
- Check your internet connection (API requires internet)
- Ensure you've entered valid data
- Try refreshing the page

### Download Not Working
- Check browser download permissions
- Try a different browser
- Ensure pop-ups are not blocked

### History Not Saving
- Check if LocalStorage is enabled in your browser
- Clear browser cache and try again
- Check if you're in private/incognito mode

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

## 🤝 Contributing

Contributions, issues, and feature requests are welcome!

1. Fork the project
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 🙏 Acknowledgments

- QR code generation powered by [QR Server API](https://goqr.me/api/)
- Inspired by modern glassmorphism design trends
- Built with love for the open-source community

## 📧 Contact

For questions or feedback, please open an issue on GitHub.

---

**Made with ⚡ and ❤️**

*Happy QR Code Generating!*
