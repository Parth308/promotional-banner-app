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

## 🎨 Theme Editor Integration

The banner seamlessly integrates with Shopify's theme editor, allowing you to customize all aspects without touching code:

![image](https://github.com/user-attachments/assets/1842a375-4f39-4ac4-9410-90ab5494d3b9)


### What You Can Edit:

- **📝 Main Banner Text**: Change your primary promotional message
- **📄 Sub Text**: Add supporting details or call-to-action text
- **⚡ Animations**: Toggle bounce and shine effects on/off
- **❌ Close Button**: Enable/disable dismissible banner option

### Real-Time Preview

All changes are instantly visible in the theme editor preview, making it easy to:
- Test different color combinations
- Preview text changes
- See how animations look
- Check mobile responsiveness

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

## 🎨 Customization Options

### Theme Editor Settings

Access these settings through **Customize Theme** > **Add Block** > **Promotional Banner**:

| Setting | Type | Default | Description |
|---------|------|---------|-------------|
| Main Banner Text | Text Input | "Free Shipping on All Orders" | Primary promotional message displayed prominently |
| Sub Text | Text Input | "Limited Time Offer • Shop Now & Save" | Secondary descriptive text or call-to-action |
| Banner Start Color | Color Picker | #8b5cf6 | Gradient start color (left side) |
| Banner End Color | Color Picker | #c084fc | Gradient end color (right side) |
| Enable Animations | Toggle | ✅ Enabled | Control bounce and shine animations |
| Show Shipping Icons | Toggle | ✅ Enabled | Display animated truck icons |
| Show Close Button | Toggle | ❌ Disabled | Allow users to dismiss the banner |

### Live Customization Benefits

- **No Code Required**: Make changes directly in the theme editor
- **Instant Preview**: See changes in real-time as you edit
- **Brand Consistency**: Easily match your store's color scheme
- **A/B Testing**: Quick text changes for testing different messages
- **Seasonal Updates**: Rapidly update for holidays and sales events

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

**Customization not working:**
- Refresh the theme editor page
- Check if you're editing the correct theme
- Ensure the block is selected in the editor

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
- Theme editor integration with live preview
- Customizable settings panel
- SVG icons
- Close button functionality

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Test thoroughly across different themes
5. Submit a pull request

## 📄 License

This promotional banner extension is released under the MIT License.

## 💡 Usage Examples

### E-commerce Promotions
```liquid
<!-- Free shipping offer -->
Main Text: "Free Shipping Worldwide"
Sub Text: "On orders over $50 • Limited time"
Colors: Blue to Purple gradient
```

### Seasonal Sales
```liquid
<!-- Holiday promotion -->
Main Text: "Black Friday Sale - 50% Off"
Sub Text: "Biggest sale of the year • Ends soon"
Colors: Red to Orange gradient
```

### New Product Launch
```liquid
<!-- Product announcement -->
Main Text: "New Collection Available"
Sub Text: "Fresh styles just dropped • Shop now"
Colors: Green to Teal gradient
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
