# UI Checklist (Mandatory)

Every component and page MUST pass this checklist before delivery.

## Icons
- [ ] **No emojis as icons** — use SVG icons or an icon library (Lucide React, Heroicons, React Icons)
- [ ] Icons have consistent size and stroke width across the app
- [ ] Icons include `aria-hidden="true"` when decorative, or `aria-label` when meaningful

## Interactivity
- [ ] **`cursor: pointer`** on all clickable elements (buttons, links, cards, toggles, tabs)
- [ ] Focus-visible styles for keyboard navigation (`outline` or `ring`)
- [ ] Disabled states are visually distinct (`opacity-50 cursor-not-allowed`)

## Transitions & Animation
- [ ] **Smooth hover transitions** on all interactive elements (duration 150-300ms)
- [ ] **Smooth click/active feedback** on buttons (scale or color change)
- [ ] **Progress bars animate** width changes (minimum 300ms ease)
- [ ] **Header transitions** smoothly on scroll (background, shadow)
- [ ] **Footer links** have hover color transitions
- [ ] **Navigation** has active state indicators with smooth transitions
- [ ] **Page content** fades/slides in on mount (subtle, 200-400ms)
- [ ] No janky or abrupt visual changes — all state changes are transitioned

## Responsive Design
- [ ] **Mobile-first** approach — design for 320px, then scale up
- [ ] Breakpoints: `sm: 640px`, `md: 768px`, `lg: 1024px`, `xl: 1280px`
- [ ] Touch targets minimum 44x44px on mobile
- [ ] Navigation collapses to hamburger/drawer on mobile
- [ ] Text remains readable without horizontal scrolling
- [ ] Images and media scale proportionally
- [ ] Spacing adjusts appropriately per breakpoint

## Accessibility
- [ ] Color contrast meets WCAG AA (4.5:1 body text, 3:1 large text)
- [ ] All interactive elements are keyboard accessible
- [ ] Form inputs have visible labels
- [ ] Error messages are descriptive and associated with fields

## General Polish
- [ ] Consistent border-radius across similar components
- [ ] Consistent spacing using Tailwind's spacing scale
- [ ] Loading states for all async operations (skeletons preferred over spinners)
- [ ] Empty states have helpful messaging and/or illustration
- [ ] No orphaned or widowed text in headings at common viewport widths
