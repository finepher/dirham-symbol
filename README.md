# 💰 UAE Dirham Symbol Icon Font

A lightweight, beautifully crafted icon font for the UAE Dirham (AED) currency symbol. Perfect for displaying prices in Arabic, Gulf, and Middle Eastern applications.

![Preview](https://img.shields.io/badge/Version-1.0.9-brightgreen) ![License](https://img.shields.io/badge/License-MIT-blue) ![Size](https://img.shields.io/badge/Size-%3C5KB-orange)

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
<link rel="stylesheet" href="https://cdn.jsdelivr.net/gh/finepher/dirham-symbol@v1.0.9/style.min.css">
<link rel="preload" href="https://cdn.jsdelivr.net/gh/finepher/dirham-symbol@v1.0.9/fonts/font-uae-dirham.woff2" as="font" type="font/woff2" crossorigin="anonymous">
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

## Why use a font instead of SVG?

The Dirham symbol is a **currency character**, not a UI icon.

Using a font provides several advantages when displaying prices throughout an application.

### Smaller HTML

With SVG, every price may require additional markup.

```html
<svg viewBox="0 0 16 14" fill="none" width="36.571429" height="32" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink"><path fill="currentColor" d="M15.8643 6.5957 15.7437 6.4844c-0.1949-0.1856-0.4268-0.2783-0.6773-0.2783l-1.2988 0c0.0185 0.2226 0.0278 0.4453 0.0278 0.6865s-93e-4 0.4638-0.0278 0.6958l0.8813 0c0.668 0 1.2154 0.6308 1.2154 1.4194v0.3526l-0.1206-0.1206c-0.1949-0.1763-0.4268-0.2691-0.6773-0.2691h-1.4936c-0.7144 3.1265-3.21 4.8242-7.1436 4.8242H1.3823c0 0 0.6865-0.5288 0.6865-2.3008l-1e-4-2.5234H1.2246C0.5474 8.9707 0 8.3306 0 7.5513V7.1987l0.1299 0.1114c0.1855 0.1762 0.4175 0.2783 0.668 0.2783l1.2709 0-1e-4-1.3823-0.8443 0C0.5474 6.2061 0 5.5659 0 4.7866V4.4341l0.1299 0.1206c0.1855 0.1763 0.4175 0.269 0.668 0.269l1.2709 0-1e-4-2.4214C2.0689 0.5747 1.3823-5e-4 1.3823-5e-4l5.0469 0c3.8223 0 6.3828 1.6792 7.1343 4.8242l1.0854 0c0.668 0 1.2154 0.6309 1.2154 1.4195zM6.2437 0.686l-2.106 0v4.1377l7.0786 0C10.7339 1.9478 9.0918 0.686 6.2437 0.686zM11.3833 6.8926c0-0.2412-93e-4-0.4639-0.0186-0.6866l-7.227 0v1.3823l7.227 0c93e-4-0.232 0.0186-0.4546 0.0186-0.6958zM4.1377 13.0991h2.1245c3.0151-0.0742 4.4995-1.5215 4.9541-4.1284H4.1377z" />
</svg>
```
so, if you show the icon with 20 products. this html reander 20 times.

With the Dirham font:

```html
<span class="dh"></span> 
```

The font file is downloaded once and cached by the browser, while the HTML remains compact.

### Better for Product-Heavy Pages

E-commerce websites often display hundreds of prices on a single page.

A cached font means the browser only needs to load the symbol glyph once, instead of rendering many SVG elements throughout the document.

### Behaves Like Text

The symbol:

- Aligns naturally with numbers
- Inherits font size
- Inherits text color
- Scales with typography
- Works with line-height and text layouts

```html
<span class="price">
  <span class="dh"></span> 
</span>
```

### Simple Integration

Just include the stylesheet:

```html
<link
  rel="stylesheet"
  href="https://cdn.jsdelivr.net/gh/finepher/dirham-symbol@v1.0.1/style.min.css"
/>
```

and use:

```html
<span class="dh"></span>
```

No SVG imports, React components, build plugins, or asset pipelines required.

### Cached Across Pages

Once loaded, the font can be reused across the entire website.

For stores displaying prices on every page, the symbol becomes a shared cached asset.

### Best Use Case

While SVG is excellent for icons, logos, and illustrations, a currency symbol behaves more like a character than an icon.

For displaying UAE Dirham prices throughout a website or application, a lightweight font-based implementation provides a simple, text-friendly, and cache-efficient solution.


## 🎉 Changelog

### v1.0.9

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