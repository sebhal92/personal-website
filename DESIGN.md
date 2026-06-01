# DESIGN.MD: Enterprise Light Minimalist System

## 1. Overview & Philosophy
The **Enterprise Light Minimalist** design system provides a professional, highly readable framework for technical portfolios. It moves away from dark-mode "developer aesthetic" toward a high-trust, corporate-ready interface.

- **Design Tone**: Reliable, structured, precise, clean.
- **Primary Use Case**: System Administration, Cloud Infrastructure, Engineering Portfolios.

## 2. Color Palette & Tokens
Used across the `tailwind.config` or inline styling:

| Token | Hex | Tailwind | Role |
| :--- | :--- | :--- | :--- |
| **Surface** | `#f8fafc` | `slate-50` | Main application background. |
| **Canvas** | `#ffffff` | `white` | Content container background. |
| **Text Primary** | `#0f172a` | `slate-900` | Headings and primary data. |
| **Text Secondary**| `#475569` | `slate-600` | Paragraphs and supporting text. |
| **Action Blue** | `#3b82f6` | `blue-600` | Primary buttons, links, accents. |
| **Action Active** | `#2563eb` | `blue-700` | Hover/Interaction states. |
| **Border** | `#f1f5f9` | `slate-100` | Structural dividers. |

## 3. Typography Strategy
- **Base Font**: `Inter` (sans-serif). Geometric, high legibility.
- **Technical Font**: `Geist` (sans-serif). Modern, monospaced-feel for metrics and labels.

| Element | Font | Size | Weight | Line Height |
| :--- | :--- | :--- | :--- | :--- |
| **Display XL** | Inter | 48px | 700 | 1.2 |
| **Headline MD** | Inter | 24px | 600 | 32px |
| **Body LG** | Inter | 18px | 400 | 28px |
| **Label MD** | Geist | 14px | 500 | 20px |

## 4. Component Library Architecture

### Buttons
- **Primary**: `bg-blue-600` + `text-white` + `rounded-lg` + `shadow-lg shadow-blue-200`.
- **Secondary**: `bg-white` + `border-slate-200` + `hover:border-blue-600`.

### Expertise Cards
- **Structure**: Container `bg-slate-50` + border `slate-100`.
- **Animation**: `transition-transform duration-200 hover:translate-y-[-4px]`.

### Timeline System (code_3.html)
- **Path**: Vertical line `left-50%` (desktop) to `left-24px` (mobile).
- **Node**: 12px dot with 2px border, `bg-blue-600`.
- **Content**: Flex-based row alternation using `md:flex-row-reverse`.

## 5. Global Technical Patterns

### Internationalization (i18n)
To support multi-language, store all strings in a centralized `translations` JS object.
- **Implementation**: Every localizable element must carry a `data-t="key"` attribute.
- **Function**: `setLanguage(lang)` performs `element.innerHTML = translations[lang][key]`.

### Secure Contact (Anti-Scraping)
To prevent bot-scraping of your email:
1. **Masking**: Use a placeholder button ("Reveal Email").
2. **Dynamic Injection**: On click, inject `contact@halaczkiewicz.it`.
3. **Clipboard**: Use `navigator.clipboard` with an `isSecureContext` check.
4. **UX Loop**: Temporarily show "Copied!" and revert to the email address after 2s.

## 6. Layout Scaling
- **Container**: Use `max-w-5xl` for main sections, `max-w-3xl` for prose/hero.
- **Spacing**: Use standard Tailwind spacing (sm: 8px, md: 16px, lg: 32px, xl: 48px).
- **Mobile**: Use `flex-col` on all major section containers, snapping to `flex-row` at `md` (768px) breakpoint.

## 7. Future Deployment Checklist
1. **Repository**: Ensure `tailwind.config.js` or CDN script is linked.
2. **Metadata**: Update `<title>` and `<meta name="viewport">`.
3. **Assets**: Verify font imports from Google Fonts.
4. **Security**: Ensure all external links have `rel="noopener noreferrer"`.
