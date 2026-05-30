---
name: Enterprise Light Minimalist
colors:
  background: '#f8fafc'
  on-background: '#0f172a'
  primary: '#3b82f6'
  primary-hover: '#2563eb'
  surface-card: '#f8fafc'
  border-card: '#f1f5f9'
  text-primary: '#0f172a'
  text-secondary: '#475569'
  text-muted: '#94a3b8'
  linkedin-blue: '#0077b5'
typography:
  display-xl:
    fontFamily: Inter
    fontSize: 48px
    fontWeight: '700'
    lineHeight: 1.2
  display-xl-mobile:
    fontFamily: Inter
    fontSize: 36px
    fontWeight: '700'
    lineHeight: 1.2
  headline-md:
    fontFamily: Inter
    fontSize: 24px
    fontWeight: '600'
    lineHeight: 32px
  body-lg:
    fontFamily: Inter
    fontSize: 18px
    fontWeight: '400'
    lineHeight: 28px
  body-md:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: '400'
    lineHeight: 24px
  label-md:
    fontFamily: Geist
    fontSize: 14px
    fontWeight: '500'
    lineHeight: 20px
rounded:
  sm: 0.25rem
  md: 0.375rem
  lg: 0.5rem
  xl: 0.75rem
  full: 9999px
spacing:
  xs: 4px
  sm: 8px
  md: 16px
  lg: 32px
  xl: 48px
  container-max: 1024px
---

## Brand & Style
The brand identity is built for a professional system and infrastructure engineer, focusing on corporate reliability, structure, and high accessibility.

The design style follows an **Enterprise Light Minimalism** philosophy. It rejects dark "hacker-style" setups in favor of a clean, bright, corporate dashboard look. It utilizes crisp white and light-gray content blocks, strict vertical rhythms, and sharp blue accents to convey competence, organization, and alignment with modern enterprise cloud ecosystems (such as Microsoft Azure and corporate IT environments).

## Colors
The palette is a high-fidelity light mode optimized for corporate readability and professional presentation.

| Token Name | Hex Code | Tailwind Equivalent | Usage |
| :--- | :--- | :--- | :--- |
| **Background** | `#f8fafc` | `slate-50` | Main canvas background, clean and soft for the eyes. |
| **On-Background** | `#0f172a` | `slate-900` | Deep slate color for headings and high-contrast text. |
| **Primary Accent**| `#3b82f6` | `blue-600` | Enterprise Blue for hyperlinks, main buttons, and active timeline nodes. |
| **Primary Hover** | `#2563eb` | `blue-700` | Deeper blue utilized for button interactive hover states. |
| **Secondary Text**| `#475569` | `slate-600` | Subtitles, dates, and supportive descriptions. |
| **Muted Text** | `#94a3b8` | `slate-400` | Timeline structural lines and passive icons. |

## Typography
The typography system uses a dual-font approach to balance editorial structure with technical precision.

- **Headlines & Body**: **Inter** is the primary font family. It offers clean neo-grotesque geometric shapes, ensuring perfect legibility from massive 48px hero text down to standard paragraphs.
- **UI Labels & Tags**: **Geist** is implemented to handle technical metadata, buttons, skills tags, and interactive UI components, establishing a precise, engineer-focused presentation layer.

## Layout & Spacing
The structure uses a highly responsive, fluid layout designed to scale flawlessly from massive workstation monitors down to mobile devices.

- **Max-Width Containers**: Central content is bound strictly within a `max-w-5xl` (1024px) container for major sections, and a tighter `max-w-3xl` (768px) layout for the introduction to maximize reading comfort.
- **Grid Layout**: The expertise area maps out into a 4-column layout (`lg:grid-cols-4`) on desktops, adapting to a 2-column or 1-column layout on smaller viewports.
- **Responsive Timeline**: A perfectly centered vertical path (`left-50%`) that dynamically shifts to a left-aligned vertical anchor (`left-[24px]`) when viewed on mobile screens.

## Elevation & Depth
The interface gains structural depth through flat container segregation and subtle semantic transformations rather than heavy drop shadows.

- **Surface Tiers**: Content blocks use a clean white background wrapped with extremely soft, light borders (`border-slate-100`) to create a clear information hierarchy over the canvas.
- **Interactive State**: Mapped elements like the expertise grid components utilize active elevation transforms. Hovering pushes the element upwards (`hover:translate-y-[-4px]`) smoothly over a `0.2s` transition loop.

## Shapes
Geometric rules are modern but strict, mirroring professional enterprise infrastructure layouts.

- **Action Elements**: Interactive buttons leverage a standard `rounded-lg` (0.5rem) radius to feel firm and clickable.
- **Skill Badges**: Pill shapes (`rounded-full`) are reserved exclusively for technical keywords to separate skills chips from clickable cards.
- **Content Blocks**: Structural layout sections are soft-framed using a balanced `rounded-xl` (0.75rem) configuration.

## Components
- **Buttons**:
  - **Primary**: Solid corporate blue background (`bg-blue-600`) with high-contrast white typography, morphing into `bg-blue-700` on mouse hover.
  - **Secondary (LinkedIn)**: Clean white surface with a thin border anchor (`border-slate-200`) which converts into a sharp `hover:border-blue-600` outline upon interaction.
- **Expertise Blocks**: Individual layout cards leveraging a subtle `bg-slate-50` backdrop fill coupled with structural transformation triggers.
- **Timeline Path**: High-contrast blue indicator nodes (`bg-blue-600`) pinned along a clean vertical separator lane, creating an easily scan-able professional history.
- **Secure Email Reveal**: A tactical JavaScript security component that prevents spam-bots from scraping information, featuring native `navigator.clipboard` integration and instant UI text confirmation updates.
