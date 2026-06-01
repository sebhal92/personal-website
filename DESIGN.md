# DESIGN.MD

## Brand & Style
The brand identity is built for a professional system and infrastructure engineer, focusing on corporate reliability, structure, and high accessibility.

The design style follows an **Enterprise Light Minimalism** philosophy. It rejects dark "hacker-style" setups in favor of a clean, bright, corporate dashboard look. It utilizes crisp white and light-gray content blocks, strict vertical rhythms, and sharp blue accents to convey competence, organization, and alignment with modern enterprise cloud ecosystems.

## Colors
The palette is a high-fidelity light mode optimized for corporate readability and professional presentation.

| Token Name | Hex Code | Tailwind Equivalent | Usage |
| :--- | :--- | :--- | :--- |
| **Background** | `#f8fafc` | `slate-50` | Main canvas background. |
| **On-Background** | `#0f172a` | `slate-900` | Headings and high-contrast text. |
| **Primary Accent**| `#3b82f6` | `blue-600` | Hyperlinks, buttons, and active nodes. |
| **Primary Hover** | `#2563eb` | `blue-700` | Button interactive hover states. |
| **Secondary Text**| `#475569` | `slate-600` | Subtitles, dates, and descriptions. |
| **Muted Text** | `#94a3b8` | `slate-400` | Structural lines and passive icons. |

## Typography
The typography system uses a dual-font approach to balance editorial structure with technical precision.

- **Headlines & Body**: **Inter** (400, 600, 700). Ensures perfect legibility from 48px hero text down to standard paragraphs.
- **UI Labels & Tags**: **Geist** (400, 500). Used for technical metadata, button labels, and skill tags.

## Layout & Spacing
- **Containers**: Central content is bound within `max-w-5xl` (1024px) for sections, and `max-w-3xl` (768px) for the hero.
- **Grid Layout**: 4-column expertise grid (`lg:grid-cols-4`) on desktops, adapting to single-column on mobile.
- **Timeline**: Centered vertical path (`left-50%`) with mobile override to left-aligned (`left-[24px]`).

## Elevation & Depth
- **Surface Tiers**: Content blocks use white backgrounds with light borders (`border-slate-100`).
- **Interactive State**: Expertise cards utilize a `hover:translate-y-[-4px]` transition over `0.2s` to indicate clickability.

## Components & Interaction
### Buttons
- **Primary**: Solid corporate blue background with high-contrast white text.
- **Secondary (LinkedIn)**: White surface with thin border, transitioning to blue outline on hover.

### Secure Email Reveal (code_3.html)
A tactical JavaScript security component to prevent scraping:
1. **Trigger**: Replaces `data-t` placeholder with `contact@halaczkiewicz.it`.
2. **Clipboard**: Native `navigator.clipboard` integration.
3. **Feedback**: Dynamic text change for 2 seconds (e.g., "Copied!" / "Skopiowano!").

### Internationalization (i18n)
The site implements a `translations` object allowing dynamic switching between English and Polish without page refreshes, targeting `data-t` attributes.
