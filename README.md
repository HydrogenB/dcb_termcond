# DCB Term & Condition Page

Static HTML page for TrueMove H Mobile Payment terms and conditions.

---

## Design Guidelines

### Typography

| Element                  | Font Family                                                                       | Size | Weight | Line Height | Color     |
| ------------------------ | --------------------------------------------------------------------------------- | ---- | ------ | ----------- | --------- |
| **Body**                 | BetterTogether, -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, sans-serif | 16px | 400    | 1.4         | `#303c46` |
| **Paragraph (.txt-prg)** | BetterTogether, sans-serif                                                        | 16px | 400    | 1.5         | `#303c46` |
| **Title H1 (.title-1)**  | BetterTogether, sans-serif                                                        | 20px | 700    | 1.2         | `#303c46` |
| **Heading H2**           | BetterTogether, sans-serif                                                        | 16px | 700    | 1.4         | `#303c46` |

### Font Sources

```css
/* BetterTogether Regular (400) */
https://assets.contentstack.io/v3/assets/blt8ba403bee4433fd8/blt8e331dd27e18e852/68998446f5108cedd790d745/BetterTogether-Regular.woff2
https://www.true.th/fonts/BetterTogether-Regular.woff2

/* BetterTogether Medium (500) */
https://assets.contentstack.io/v3/assets/blt8ba403bee4433fd8/blt547f83cf5392ab91/6899843efa6331f97f4061d8/BetterTogether-Medium.woff2
https://www.true.th/fonts/BetterTogether-Medium.woff2

/* BetterTogether Bold (700) */
https://assets.contentstack.io/v3/assets/blt8ba403bee4433fd8/blt6e4e59f67740f5dc/689984356605f97da6acb650/BetterTogether-Bold.woff2
https://www.true.th/fonts/BetterTogether-Bold.woff2
```

### Colors

| Token              | Hex Code  | Usage            |
| ------------------ | --------- | ---------------- |
| Text Primary       | `#303c46` | All text content |
| Background Main    | `#f5f5f5` | Page background  |
| Background Content | `#ffffff` | Content sections |

### Layout & Spacing

| Property                | Mobile    | Desktop (≥760px) |
| ----------------------- | --------- | ---------------- |
| Content Max Width       | 100%      | 1140px           |
| Content Padding         | 30px 20px | 50px             |
| Text Indent             | 25px      | 25px             |
| H1 Margin Bottom        | 20px      | 20px             |
| H2 Margin Top           | 20px      | 20px             |
| H2 Margin Bottom        | 15px      | 15px             |
| Paragraph Break Spacing | 15px      | 15px             |

### CSS Classes

| Class                    | Purpose                              |
| ------------------------ | ------------------------------------ |
| `.main-block`            | Outer container with gray background |
| `.section-content`       | White content wrapper                |
| `.section-content-inner` | Centered, padded content area        |
| `.txt-prg`               | Paragraph text styling               |
| `.title-1`               | Main title (H1) styling              |
| `.txt-indent`            | Indented text blocks (sub-items)     |

### Mobile Meta Tags

```html
<meta name="viewport" content="width=device-width, initial-scale=1.0" />
<meta name="apple-mobile-web-app-capable" content="yes" />
<meta name="apple-mobile-web-app-status-bar-style" content="black" />
<meta name="format-detection" content="telephone=no" />
```

---

## Structure

```
.main-block (background: #f5f5f5)
└── .section-content (background: #ffffff)
    └── .section-content-inner.txt-prg
        ├── h1.title-1 (page title)
        ├── p (intro paragraph)
        ├── h2 > strong (section title)
        ├── p (numbered items)
        └── div.txt-indent (sub-items like 5.1, 5.2)
```
