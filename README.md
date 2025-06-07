# Promotional Banner Extension

A professional and customizable promotional banner for Shopify stores, designed to showcase special offers, free shipping, and limited-time promotions.

## 🎯 Overview

This promotional banner extension provides a sleek, modern way to display promotional messages at the top of your Shopify store. It features smooth animations, responsive design, and easy customization through the Shopify theme editor.

## ✨ Features

- **Professional Design**: Clean, modern aesthetic that complements any store theme
- **Fully Responsive**: Optimized for desktop, tablet, and mobile devices
- **Smooth Animations**: Subtle bounce effects and shine animations
- **Easy Customization**: Configure colors, text, and animations through Shopify admin
- **Performance Optimized**: Lightweight CSS and minimal JavaScript
- **Accessibility Friendly**: Good contrast ratios and semantic markup

## 🚀 Installation

### Method 1: Manual Installation

1. Create the extension directory structure:
   ```
   extensions/
   └── promotional-banner/
       └── blocks/
           └── banner.liquid
   ```

2. Copy the provided code into `banner.liquid`

3. Add the extension to your theme through the Shopify admin:
   - Go to **Online Store** > **Themes**
   - Click **Customize** on your active theme
   - Add the **Promotional Banner** block where desired

### Method 2: Shopify CLI (Recommended)

```bash
# Create new extension
shopify app scaffold extension --type=theme_app_extension

# Navigate to extension directory
cd extensions/promotional-banner

# Copy the banner.liquid file to blocks/
```

## 🎨 Customization

### Theme Editor Settings

Access these settings through **Customize Theme** > **Add Block** > **Promotional Banner**:

| Setting | Type | Default | Description |
|---------|------|---------|-------------|
| Main Banner Text | Text | "Free Shipping on All Orders" | Primary promotional message |
| Sub Text | Text | "Limited Time Offer • Shop Now & Save" | Secondary descriptive text |
| Banner Start Color | Color | #8b5cf6 | Gradient start color |
| Banner End Color | Color | #c084fc | Gradient end color |
| Enable Animations | Checkbox | True | Toggle bounce and shine animations |
| Show Shipping Icons | Checkbox | True | Display truck icons |

### Advanced Customization

#### Changing Colors
```css
/* Modify the gradient in the style attribute */
background: linear-gradient(90deg, #your-color-1 0%, #your-color-2 50%, #your-color-3 100%);
```

#### Custom Animations
```css
/* Add custom keyframes */
@keyframes your-animation {
  0% { /* start state */ }
  100% { /* end state */ }
}
```

#### Typography Adjustments
```css
/* Modify font sizes and weights */
font-size: 15px;
font-weight: 600;
letter-spacing: 0.5px;
```

## 📱 Responsive Breakpoints

The banner automatically adjusts for different screen sizes:

- **Desktop**: Full size with all animations
- **Tablet (≤768px)**: Reduced padding and font sizes
- **Mobile (≤480px)**: Compact layout with optimized spacing

## 🔧 Technical Details

### Browser Support
- Chrome 60+
- Firefox 55+
- Safari 12+
- Edge 79+

### Performance
- **CSS Size**: ~2KB minified
- **Load Impact**: Minimal, loads with page
- **Animation**: GPU-accelerated transforms

### Dependencies
- None (Pure CSS/HTML)
- Uses system fonts for faster loading
- SVG icons for crisp display

## 🎭 Animation Details

### Bounce Animation
- **Duration**: 2 seconds
- **Timing**: Infinite loop
- **Effect**: Subtle vertical movement on shipping icons

### Shine Effect
- **Duration**: 3 seconds
- **Timing**: Infinite loop
- **Effect**: Gradient highlight sweep across banner

### Hover Effects
- **Transform**: 1px upward movement
- **Shadow**: Purple glow effect
- **Timing**: 0.3s cubic-bezier transition

## 🛠️ Troubleshooting

### Common Issues

**Banner not displaying:**
- Ensure the extension is properly installed
- Check that the block is added to your theme
- Verify theme compatibility

**Animations not working:**
- Check if animations are enabled in settings
- Verify browser supports CSS animations
- Ensure no conflicting CSS

**Mobile display issues:**
- Clear browser cache
- Test on actual devices
- Check responsive breakpoints

### Debug Mode

Add this CSS for debugging:
```css
.promotional-banner {
  border: 2px solid red !important;
}
```

## 📋 Changelog

### v1.0.0 (Current)
- Initial release
- Professional gradient design
- Responsive layout
- Smooth animations
- Customizable settings
- SVG icons
- Theme editor integration

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Test thoroughly
5. Submit a pull request

## 📄 License

This promotional banner extension is released under the MIT License.

## 💡 Usage Examples

### E-commerce Promotions
```liquid
<!-- Free shipping offer -->
Main Text: "Free Shipping Worldwide"
Sub Text: "On orders over $50 • Limited time"
```

### Seasonal Sales
```liquid
<!-- Holiday promotion -->
Main Text: "Black Friday Sale - 50% Off"
Sub Text: "Biggest sale of the year • Ends soon"
```

### New Product Launch
```liquid
<!-- Product announcement -->
Main Text: "New Collection Available"
Sub Text: "Fresh styles just dropped • Shop now"
```

## 🔗 Related Resources

- [Shopify Theme Development](https://shopify.dev/themes)
- [Shopify App Extensions](https://shopify.dev/apps/app-extensions)
- [CSS Animations Guide](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Animations)

## 📞 Support

For support and questions:
- Create an issue in the repository
- Check the troubleshooting section
- Review Shopify's theme documentation

---

**Made with ❤️ By Parth For Shopify**