# StreamLife Design System

## Overview

StreamLife uses **"The Ethereal Broadcaster"** design system - a high-end, editorial framework that transforms audio interfaces into a sculpted digital environment with depth, translucency, and intentional asymmetry.

## Design Philosophy

We reject the rigid "box-and-border" constraints of standard web design, embracing:
- **Depth** through glassmorphic layering
- **Translucency** with backdrop blur effects
- **Intentional Asymmetry** breaking the grid for premium feel
- **Premium Audio Equipment Aesthetic** where content floats in light and glass

## Color Palette

### Primary Colors
- **Primary Blue**: `#b2c5ff` - Signal color for active states, live indicators, CTAs
- **Primary Container**: `#0045b0` - Deep blue for depth
- **Background**: `#131313` - Base dark background
- **Surface**: `#131313` - Main content area

### Surface Hierarchy
- **Background**: `#131313` - Base layer
- **Surface Container Low**: `#1c1b1b` - Sectioning
- **Surface Container**: `#201f1f` - Interactive cards
- **Surface Container High**: `#2a2a2a` - Elevated elements
- **Surface Bright**: `#393939` - Hover states

### Supporting Colors
- **Error**: `#ffb4ab` - Alerts and destructive actions
- **Outline**: `#8c909d` - Text dimmed/secondary
- **On Surface**: `#e5e2e1` - Primary text color

## Typography

### Font Stack
- **Headlines**: Manrope (400, 500, 700, 800)
  - Display, Title, Headline sizes for artist names and categories
  - Geometric yet warm for modern, high-end feel
  
- **Body & Labels**: Inter (400, 500, 600)
  - Body text, track lists, metadata
  - Excellent legibility on dark backgrounds

### Size Scale
- **Display Large**: 3.5rem (56px)
- **Display Medium**: 2.8rem (45px)
- **Display Small**: 2.25rem (36px)
- **Headline Large**: 2rem (32px)
- **Headline Medium**: 1.75rem (28px)
- **Headline Small**: 1.5rem (24px)
- **Title Large**: 1.375rem (22px)
- **Title Medium**: 1rem (16px)
- **Body Large**: 1rem (16px)
- **Body Medium**: 0.875rem (14px)
- **Label Large**: 0.875rem (14px)

## Component Guidelines

### Buttons

#### Primary Button
```
Background: primary (#b2c5ff)
Text: on-primary (#002b74)
Padding: 1rem (16px)
Radius: 0.75rem (12px)
Hover: scale(1.05)
Active: scale(0.95)
```

#### Ghost/Tertiary Button
```
Background: transparent
Text: primary (#b2c5ff)
Padding: 1rem (16px)
Radius: 0.75rem (12px)
Hover: background-color: rgba(255, 255, 255, 0.1)
```

### Glass Panel Rule

All floating panels must follow:
```css
backdrop-filter: blur(24px);
-webkit-backdrop-filter: blur(24px);
background-color: rgba(surface, 0.4-0.6);
```

### Card Styling

**No Dividers Rule**: Never use 1px solid borders. Boundaries are defined through:
1. Background color shifts
2. Spacing (4-8 units of padding)
3. Subtle ghost borders: `outline_variant` at 15% opacity

### Stream Cards

```
Layout: Horizontal flex with gap-6
Padding: 1.5rem (24px)
Border: 1px solid outline-variant/20
Border Radius: 1.25rem (20px)
Hover: background-color shift to surface-bright/20
Active: box-shadow glow with primary color
Icon Container: w-12 h-12 bg-primary/10
Transition: all 0.3s ease
```

### Progress Bar

```
Rail: h-1 bg-secondary-container (#46494d)
Progress: Gradient from primary to primary-container
Thumb: w-3 h-3 circle, opacity-0 → opacity-100 on hover
Radius: full (9999px)
```

### Now Playing Section

```
Height: 380px (hero section)
Gradient: to bottom from primary/40 via primary-container/30
Overlay: gradient to transparent
Typography: Display sizes for artist name
Buttons: Primary + Ghost secondary
Verified Badge: primary/20 bg with backdrop blur
```

## Depth & Layering

### Shadow System

**Ambient Shadows** (soft, diffused):
```css
box-shadow: 0 20px 40px rgba(0, 0, 0, 0.6);
```

**Elevation Levels**:
1. **Base**: background (#131313)
2. **Level 1**: surface-container-low (#1c1b1b)
3. **Level 2**: surface-container (#201f1f)
4. **Level 3**: surface-container-high (#2a2a2a)
5. **Floating**: surface with backdrop-blur

## Spacing Scale

```
0.25rem = 4px
0.5rem = 8px
0.75rem = 12px
1rem = 16px
1.5rem = 24px
2rem = 32px
3rem = 48px
4rem = 64px
```

## Do's & Don'ts

### ✅ Do

- Use asymmetrical layouts; let imagery bleed off container edges
- Apply backdrop-filter blur to any overlay element
- Use spacing strictly (8, 12, 16, 24, 32, 48 units)
- Create depth through color shifting, not borders
- Use gradients sparingly for "soul" (play buttons, badges)
- Maintain high contrast for accessibility

### ❌ Don't

- Use standard 1px solid borders for cards or sections
- Use pure black (#000000) - use background or surface-container-lowest
- Clutter interfaces - hide secondary info behind actions
- Use fully opaque strokes - max 15% opacity for ghost borders
- Mix serif and sans-serif fonts
- Add drop shadows to everything - use sparingly for floating elements

## Responsive Design

### Breakpoints (Tailwind)
- **sm**: 640px
- **md**: 768px
- **lg**: 1024px
- **xl**: 1280px

### Layout Strategy
- **Mobile**: Single column, full-width streams
- **Tablet**: 2-3 column grid, visible sidebar
- **Desktop**: 3-4 column grid with fixed sidebar navigation

### Player Bar
- **Fixed bottom**: 32px (bottom-8)
- **Width**: 92% max-w-6xl
- **Z-index**: 50 (above all content)
- **Responsive**: Flex direction changes on small screens

## Accessibility

- **Color Contrast**: Minimum 4.5:1 WCAG AA
- **Focus States**: Visible outline or background shift
- **Icon Labels**: All icons have semantic meaning or aria-labels
- **Motion**: Transitions max 300ms
- **Text**: Minimum 14px for body text

## Animation Guidelines

```
Transitions: all 0.3s ease
Hover: scale(1.05) or opacity shift
Active: scale(0.95) 
Entry: fade + slide for important elements
Duration: 200-300ms max
```

## Customization

To customize StreamLife for your brand:

1. **Color Scheme**: Update color tokens in `<script id="tailwind-config">`
2. **Fonts**: Change font URLs in `<head>`
3. **Icons**: Swap Material Symbols for your icon set
4. **Branding**: Update title, logo, tagline in sidebar
5. **Streams**: Modify `streams.json` with your radio stations

---

**Version**: 1.0.0  
**Last Updated**: 2026  
**System**: The Ethereal Broadcaster
