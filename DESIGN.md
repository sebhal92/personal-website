# DESIGN.MD

## Project: Personal Brand Website (Sebastian Hałaczkiewicz)

This document describes the structure and design principles of the personal website based on **Tailwind CSS**.

### 1. Project Goal
The website serves as a modern, responsive professional portfolio (Personal Brand) for a System Infrastructure Administrator. Its primary goal is to showcase professional experience, technical expertise, and provide a clear contact point.

### 2. Technical Architecture
* **CSS Framework**: Tailwind CSS (via CDN).
* **Typography**: 
    * `Inter` (primary body font).
    * `Geist` (specialized UI elements).
* **Interactivity**: Vanilla JavaScript handling:
    * Internationalization (EN/PL switching).
    * Secure e-mail reveal mechanism (with clipboard integration).
    * Smooth scrolling.

### 3. Page Structure

| Section | Component | Description |
| :--- | :--- | :--- |
| **Navigation** | Sticky Header | Backdrop-blur effect, language toggle, and internal links. |
| **Hero** | Header Section | Main title, professional tag, and primary Call-to-Action (CTA) buttons. |
| **Expertise** | Grid Layout | 4-column layout (responsive) detailing key MS ecosystem skills. |
| **Experience** | Vertical Timeline | Alternating cards showcasing professional path from current to past. |
| **Contact** | Feature Block | Dedicated section with a secure e-mail reveal and LinkedIn link. |

### 4. Internationalization (i18n)
The site supports two languages via a `translations` object:
* The `setLanguage(lang)` function dynamically updates `innerHTML` for elements marked with the `data-t` attribute.
* Default language: **English**.

### 5. E-mail Interaction Logic
To protect the e-mail address from scraping, we utilize a tactical security component:

1. **Trigger**: Clicking the button updates the DOM with `contact@halaczkiewicz.it`.
2. **Copy**: Native `navigator.clipboard` integration ensures quick UX.
3. **Feedback**: The button label provides real-time status updates:
   * EN: "(Copied!)"
   * PL: "(Skopiowano!)"

### 6. Design System & Constraints

| Category | Definition |
| :--- | :--- |
| **Primary Color** | `blue-600` (corporate blue) |
| **Background** | `slate-50` / `white` (clean enterprise feel) |
| **Spacing** | 1.25 line height for optimal readability |
| **Responsiveness** | Mobile-first with breakpoint adjustments for timeline nodes |
