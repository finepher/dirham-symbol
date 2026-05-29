# 💰 UAE Dirham Symbol Icon Font

A lightweight, beautifully crafted icon font for the UAE Dirham (AED) currency symbol. Perfect for displaying prices in Arabic, Gulf, and Middle Eastern applications.

![Preview](https://img.shields.io/badge/Version-1.0.1-brightgreen) ![License](https://img.shields.io/badge/License-MIT-blue) ![Size](https://img.shields.io/badge/Size-%3C5KB-orange)

---

## ✨ Why Use This?

### 🎯 Key Benefits

- **🚀 Lightweight** - Minimal file size (< 5KB), loads in milliseconds
- **🎨 Scalable** - Scales to any size without losing quality (it's a font!)
- **🔤 Colorable** - Change colors with simple CSS—no image editing needed
- **♿ Accessible** - Proper semantic markup and ARIA support
- **🌐 Universal** - Works everywhere HTML and CSS work
- **⚡ Fast** - No render delays or performance impact
- **📱 Responsive** - Perfect for mobile, tablet, and desktop
- **🌙 Dark Mode Ready** - Automatically adapts to your design system
- **🔗 Framework Agnostic** - Works with any library or framework

### 💡 Perfect For

- **E-commerce sites** - Display prices in AED instantly
- **Billing dashboards** - Financial applications and accounting software
- **Multi-currency apps** - Add AED support alongside other currencies
- **Regional content** - UAE, Saudi Arabia, and Gulf-focused applications
- **Payment pages** - Checkout flows and invoice generation

---

## 📦 Installation

> **💡 Tip:** Currently, CDN and local file installation are recommended. NPM package is coming soon!

### Option 1: CDN (Fastest)

```html
<!-- Add to your <head> -->
<link rel="stylesheet" href="https://cdn.jsdelivr.net/gh/finepher/dirham-symbol@v1.0.1/style.css">
<link rel="preload" href="https://cdn.jsdelivr.net/gh/finepher/dirham-symbol@v1.0.1/fonts/Untitled.woff2" as="font" type="font/woff2" crossorigin="anonymous">
```

### Option 2: NPM (Coming Soon 🚀)

```bash
npm install uae-dirham-symbol
```

```html
<!-- Import in your project -->
<link rel="stylesheet" href="node_modules/uae-dirham-symbol/style.css">
```

> **Coming Soon:** NPM package will be available in the next release. For now, use CDN or local files.

### Option 3: Local Files

1. Download or clone this repository
2. Copy `style.css` and the `fonts/` folder to your project
3. Link the stylesheet:

```html
<link rel="stylesheet" href="./path/to/style.css">
```

---

## 🚀 Quick Start

### HTML

```html
<!-- Using font-uae-dirham class with explicit character -->
<span class="font-uae-dirham">&#xf000;</span>

<!-- Using icon-uae-dirham class (auto-generated content) -->
<span class="icon-uae-dirham" aria-hidden="true"></span>

<!-- In a price -->
<span class="font-uae-dirham">&#xf000;</span> 299.00
```

### CSS Styling

```css
/* Custom sizing */
.price-icon {
  font-size: 24px;
  color: #2c5282;
}

/* With hover effect */
.price-icon:hover {
  color: #c4922a;
  transition: color 0.2s ease;
}

/* Responsive sizing */
@media (max-width: 768px) {
  .price-icon {
    font-size: 18px;
  }
}
```

---

## 🛠️ Framework & Library Integration

### React.js

```jsx
import 'uae-dirham-symbol/style.css';

function PriceTag({ amount }) {
  return (
    <div className="price">
      <span className="font-uae-dirham">&#xf000;</span> {amount.toFixed(2)}
    </div>
  );
}

// Usage
<PriceTag amount={299.99} />
```

### Vue.js

```vue
<template>
  <div class="price">
    <span class="font-uae-dirham">&#xf000;</span> {{ amount }}
  </div>
</template>

<script>
import 'uae-dirham-symbol/style.css';

export default {
  props: {
    amount: Number
  }
}
</script>

<style scoped>
.price {
  font-size: 20px;
  font-weight: bold;
}
</style>
```

### Angular

```typescript
import { Component } from '@angular/core';
import 'uae-dirham-symbol/style.css';

@Component({
  selector: 'app-price',
  template: `<span class="font-uae-dirham">&#xf000;</span> {{ amount }}`,
  styles: [`
    :host {
      font-size: 20px;
      font-weight: bold;
    }
  `]
})
export class PriceComponent {
  amount = 299.99;
}
```

### Laravel / Blade

```blade
<!-- In your Blade template -->
<div class="product-price">
  <span class="font-uae-dirham">&#xf000;</span> {{ $product->price }}
</div>

<!-- With formatting -->
<span class="font-uae-dirham">&#xf000;</span> {{ number_format($amount, 2) }}
```

```html
<!-- Add to your main layout -->
<head>
  <link rel="stylesheet" href="{{ asset('css/dirham-symbol.css') }}">
</head>
```

### Next.js

```jsx
import 'uae-dirham-symbol/style.css';

export default function ProductCard({ price }) {
  return (
    <div className="product">
      <h3>Premium Item</h3>
      <p className="price">
        <span className="font-uae-dirham">&#xf000;</span> {price}
      </p>
    </div>
  );
}
```

### Svelte

```svelte
<script>
  import 'uae-dirham-symbol/style.css';
  
  let price = 199.99;
</script>

<div class="price">
  <span class="font-uae-dirham">&#xf000;</span> {price}
</div>

<style>
  .price {
    font-size: 20px;
    font-weight: bold;
  }
</style>
```

### Tailwind CSS

```html
<!-- With Tailwind utilities -->
<span class="font-uae-dirham text-2xl text-blue-900">&#xf000;</span>
<span class="font-uae-dirham text-lg text-gray-600 hover:text-amber-600 transition">&#xf000;</span> 299.00
```

### Bootstrap

```html
<div class="d-flex align-items-center gap-2">
  <span class="font-uae-dirham fs-4 text-primary">&#xf000;</span>
  <span>299.00</span>
</div>
```

---

## 📖 Usage Examples

### E-commerce Product Card

```html
<div class="product-card">
  <img src="product.jpg" alt="Product">
  <h3>Wireless Headphones</h3>
  <p class="description">Premium audio quality</p>
  
  <div class="price-section">
    <span class="original-price">
      <span class="strikethrough">
        <span class="font-uae-dirham">&#xf000;</span> 599.00
      </span>
    </span>
    <span class="sale-price">
      <span class="font-uae-dirham">&#xf000;</span> 399.00
      <span class="discount">-33%</span>
    </span>
  </div>
  
  <button>Add to Cart</button>
</div>
```

### Invoice/Receipt

```html
<table class="invoice">
  <tr>
    <td>Item Name</td>
    <td>Qty</td>
    <td>Price</td>
    <td>Total</td>
  </tr>
  <tr>
    <td>Product A</td>
    <td>2</td>
    <td><span class="font-uae-dirham">&#xf000;</span> 100</td>
    <td><span class="font-uae-dirham">&#xf000;</span> 200</td>
  </tr>
  <tr class="total-row">
    <td colspan="3">Total</td>
    <td><strong><span class="font-uae-dirham">&#xf000;</span> 200</strong></td>
  </tr>
</table>
```

### Price Range Display

```html
<p class="price-range">
  From <span class="font-uae-dirham">&#xf000;</span> 99.99 
  to <span class="font-uae-dirham">&#xf000;</span> 999.99
</p>
```

---

## 🎨 Customization

### Change Size

```css
.font-uae-dirham {
  font-size: 32px; /* Adjust as needed */
}
```

### Change Color

```css
.font-uae-dirham {
  color: #c4922a; /* Your color */
}
```

### Add Effects

```css
.font-uae-dirham {
  color: #2c5282;
  text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.1);
  transition: transform 0.2s ease;
}

.font-uae-dirham:hover {
  transform: scale(1.1);
}
```

### Dark Mode Support

```css
@media (prefers-color-scheme: dark) {
  .font-uae-dirham {
    color: #dba94a;
  }
}
```

---

## ♿ Accessibility

Always use proper semantic markup and ARIA attributes:

```html
<!-- When icon is decorative -->
<span class="font-uae-dirham" aria-hidden="true">&#xf000;</span> Price: 299

<!-- When icon is meaningful, include descriptive text -->
<span class="font-uae-dirham">&#xf000;</span> <span class="sr-only">AED</span> 299
```

---

## 📊 Browser Support

| Browser | Support | Notes |
|---------|---------|-------|
| Chrome | ✅ All versions | Full support |
| Firefox | ✅ All versions | Full support |
| Safari | ✅ All versions | Full support |
| Edge | ✅ All versions | Full support |
| Opera | ✅ All versions | Full support |
| IE 11 | ⚠️ Limited | Use EOT format |
| Mobile Browsers | ✅ All | Full support |

---

## 📋 Character Reference

| Property | Value |
|----------|-------|
| **Font Name** | Font-UAE-Dirham |
| **Unicode** | U+F000 |
| **HTML Entity** | `&#xf000;` |
| **CSS Content** | `"\f000"` |
| **Class Name** | `font-uae-dirham` or `icon-uae-dirham` |

---

## 🤝 Contributing

Found a bug? Have an improvement idea? We'd love your help!

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

---

## 📄 License

This project is licensed under the **MIT License** - see the [LICENSE](LICENSE) file for details.

---

## 💬 Questions & Support

- 📧 Email: support@example.com
- 🐙 GitHub Issues: [Report Issues](https://github.com/yourusername/dirham-symbol/issues)
- 💬 Discussions: [Ask Questions](https://github.com/yourusername/dirham-symbol/discussions)

---

## 🎉 Changelog

### v1.0.1
- ⚡ **Performance Optimization** - Further reduced font file size and improved loading times

### v1.0.0
- ✨ Initial release
- ✅ Support for all modern browsers
- ✅ Multiple class options (`font-uae-dirham` and `icon-uae-dirham`)
- ✅ CDN delivery via jsDelivr

---

## 🙏 Credits

Built with ❤️ for the Arabic and Middle Eastern development community.

---

**Made with 💚 for the UAE** 🇦🇪