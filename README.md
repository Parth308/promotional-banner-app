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

![image](https://github.com/user-attachments/assets/df725454-da50-4c94-9f1f-42dc43fce3c3)


### What You Can Edit:

- **📝 Main Banner Text**: Change your primary promotional message
- **📄 Sub Text**: Add supporting details or call-to-action text
- **🎨 Color Settings**: Advanced gradient customization with presets
- **⚡ Animations**: Toggle bounce and shine effects on/off
- **❌ Close Button**: Enable/disable dismissible banner option

### Real-Time Preview

All changes are instantly visible in the theme editor preview, making it easy to:
- Test different gradient presets and custom color combinations
- Preview text changes with proper formatting
- See how animations look and feel
- Check mobile responsiveness
- Fine-tune three-point gradient transitions

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

#### Text Content
| Setting | Type | Default | Description |
|---------|------|---------|-------------|
| Main Banner Text | Text Input | "Free Shipping on All Orders!" | Primary promotional message displayed prominently |
| Sub Text | Text Input | "Limited Time Offer • Shop Now & Save!" | Secondary descriptive text or call-to-action |

#### Color Settings
| Setting | Type | Default | Description |
|---------|------|---------|-------------|
| Gradient Preset | Dropdown | "Purple (Default)" | Pre-configured color combinations |
| Primary Color (Left) | Color Picker | #4C1D95 | Gradient start color - only when "Custom Colors" selected |
| Secondary Color (Center) | Color Picker | #7C3AED | Gradient middle color - only when "Custom Colors" selected |
| Tertiary Color (Right) | Color Picker | #7E2ACE | Gradient end color - only when "Custom Colors" selected |

#### Banner Options
| Setting | Type | Default | Description |
|---------|------|---------|-------------|
| Show Close Button | Toggle | ✅ Enabled | Allow users to dismiss the banner |
| Enable Animations | Toggle | ✅ Enabled | Control bounce and shine animations |

### Live Customization Benefits

- **No Code Required**: Make changes directly in the theme editor
- **Instant Preview**: See changes in real-time as you edit
- **Gradient Presets**: Choose from pre-configured color combinations or create custom gradients
- **Advanced Color Control**: Fine-tune three-point gradients for perfect brand matching
- **Smart Color Logic**: Custom color pickers only appear when needed
- **A/B Testing**: Quick text changes for testing different messages
- **Seasonal Updates**: Rapidly update for holidays and sales events

### Advanced Customization

#### Advanced Gradient Customization
```css
/* Three-point gradient system */
background: linear-gradient(90deg, 
  #4C1D95 0%,     /* Primary Color (Left) */
  #7C3AED 50%,    /* Secondary Color (Center) */
  #7E2ACE 100%    /* Tertiary Color (Right) */
);

/* Custom gradient presets */
.gradient-purple { background: linear-gradient(90deg, #4C1D95, #7C3AED, #7E2ACE); }
.gradient-blue { background: linear-gradient(90deg, #1E3A8A, #3B82F6, #06B6D4); }
.gradient-green { background: linear-gradient(90deg, #166534, #22C55E, #10B981); }
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
