# Icon Libraries & Tailwind Reference

## Icon Libraries (Recommended)

### Lucide React (Primary Recommendation)
```bash
npm install lucide-react
```
```tsx
import { Search, BookOpen, CheckCircle, Star } from 'lucide-react';

<Search className="w-5 h-5 text-slate-500" />
```
- 1000+ icons, consistent 24x24 grid, 2px stroke
- Tree-shakable, lightweight
- Perfect for learning/education apps

### Heroicons (Alternative)
```bash
npm install @heroicons/react
```
```tsx
import { AcademicCapIcon } from '@heroicons/react/24/outline';
```

### Custom SVG
For brand-specific icons, use inline SVG or create a reusable component:
```tsx
const CustomIcon = ({ className }: { className?: string }) => (
  <svg className={className} viewBox="0 0 24 24" fill="none" stroke="currentColor" strokeWidth={2}>
    {/* paths */}
  </svg>
);
```

## Tailwind CSS Utilities Quick Reference

### Transitions (use these instead of raw CSS when possible)
```
transition-all duration-200 ease-in-out     — general purpose
transition-colors duration-200              — color changes only
transition-transform duration-150           — movement only
transition-opacity duration-300             — fade effects
```

### Common Interactive Patterns
```
hover:bg-indigo-50 active:bg-indigo-100     — background feedback
hover:scale-105 active:scale-95            — size feedback
hover:shadow-md active:shadow-sm           — elevation feedback
hover:-translate-y-0.5                      — subtle lift
cursor-pointer                              — clickable indicator
focus-visible:ring-2 focus-visible:ring-indigo-500 — keyboard focus
```
