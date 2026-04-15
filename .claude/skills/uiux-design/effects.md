# Effects Catalog

## Hover Effects

```css
/* Subtle lift — for cards, list items */
.hover-lift {
  transition: transform 0.2s ease, box-shadow 0.2s ease;
}
.hover-lift:hover {
  transform: translateY(-2px);
  box-shadow: 0 4px 12px rgba(0, 0, 0, 0.1);
}

/* Scale — for buttons, icons */
.hover-scale {
  transition: transform 0.15s ease;
}
.hover-scale:hover {
  transform: scale(1.05);
}

/* Background fade — for nav items, menu links */
.hover-bg {
  transition: background-color 0.2s ease, color 0.2s ease;
}
```

## Click / Active Effects

```css
/* Press down — for buttons */
.active-press:active {
  transform: scale(0.97);
  transition: transform 0.1s ease;
}

/* Ripple — use with JS for material-style feedback */
```

## Progress Bar Animation

```css
/* Smooth width transition */
.progress-bar {
  transition: width 0.5s cubic-bezier(0.4, 0, 0.2, 1);
}

/* With glow pulse for active progress */
.progress-bar-glow {
  transition: width 0.5s cubic-bezier(0.4, 0, 0.2, 1);
  animation: pulse-glow 2s ease-in-out infinite;
}

@keyframes pulse-glow {
  0%, 100% { box-shadow: 0 0 4px rgba(79, 70, 229, 0.3); }
  50%      { box-shadow: 0 0 12px rgba(79, 70, 229, 0.6); }
}
```

## Header & Navigation Transitions

```css
/* Sticky header with backdrop blur on scroll */
.header-scroll {
  transition: background-color 0.3s ease, backdrop-filter 0.3s ease, box-shadow 0.3s ease;
}

/* Nav link underline slide */
.nav-link::after {
  content: '';
  position: absolute;
  bottom: 0;
  left: 50%;
  width: 0;
  height: 2px;
  background: var(--color-primary);
  transition: width 0.3s ease, left 0.3s ease;
}
.nav-link:hover::after,
.nav-link.active::after {
  width: 100%;
  left: 0;
}

/* Mobile nav slide-in */
.mobile-nav {
  transform: translateX(-100%);
  transition: transform 0.3s cubic-bezier(0.4, 0, 0.2, 1);
}
.mobile-nav.open {
  transform: translateX(0);
}
```

## Footer Transitions

```css
/* Footer link hover */
.footer-link {
  transition: color 0.2s ease, transform 0.2s ease;
}
.footer-link:hover {
  color: var(--color-primary);
}
```

## Page & Component Transitions

```css
/* Fade in on mount */
@keyframes fadeIn {
  from { opacity: 0; transform: translateY(8px); }
  to   { opacity: 1; transform: translateY(0); }
}
.animate-fade-in {
  animation: fadeIn 0.3s ease-out;
}

/* Slide in from side */
@keyframes slideInRight {
  from { opacity: 0; transform: translateX(16px); }
  to   { opacity: 1; transform: translateX(0); }
}

/* Skeleton loading shimmer */
@keyframes shimmer {
  0%   { background-position: -200% 0; }
  100% { background-position: 200% 0; }
}
.skeleton {
  background: linear-gradient(90deg, #e2e8f0 25%, #f1f5f9 50%, #e2e8f0 75%);
  background-size: 200% 100%;
  animation: shimmer 1.5s infinite;
}
```
