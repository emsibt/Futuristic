# Typography Presets

All fonts are **free Google Fonts**. Each preset pairs a heading font with a body font.

## 1. Inter + Inter (Clean & Versatile)
```css
/* Best for: Any modern web app */
@import url('https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700&display=swap');

--font-heading: 'Inter', sans-serif;
--font-body: 'Inter', sans-serif;
```
- Highly readable at all sizes, excellent for UI text
- Differentiate hierarchy with weight (400 body, 600 headings, 700 hero)

## 2. Plus Jakarta Sans + Inter (Friendly & Modern)
```css
/* Best for: Learning platforms, educational apps */
@import url('https://fonts.googleapis.com/css2?family=Plus+Jakarta+Sans:wght@500;600;700;800&family=Inter:wght@400;500;600&display=swap');

--font-heading: 'Plus Jakarta Sans', sans-serif;
--font-body: 'Inter', sans-serif;
```
- Jakarta Sans has geometric, friendly letterforms — great for headings
- Inter for body ensures readability in long text

## 3. Outfit + Source Sans 3 (Approachable & Clear)
```css
/* Best for: Study tools, community platforms */
@import url('https://fonts.googleapis.com/css2?family=Outfit:wght@400;500;600;700&family=Source+Sans+3:wght@400;500;600&display=swap');

--font-heading: 'Outfit', sans-serif;
--font-body: 'Source Sans 3', sans-serif;
```
- Outfit is geometric and warm — inviting for educational content
- Source Sans 3 is optimized for screen readability

## 4. Space Grotesk + DM Sans (Bold & Techy)
```css
/* Best for: Gamified learning, tech-focused apps */
@import url('https://fonts.googleapis.com/css2?family=Space+Grotesk:wght@500;600;700&family=DM+Sans:wght@400;500;600&display=swap');

--font-heading: 'Space Grotesk', sans-serif;
--font-body: 'DM Sans', sans-serif;
```
- Space Grotesk has a distinctive, modern character
- DM Sans is clean and neutral for body text

## Typography Scale

```
text-xs:   0.75rem  / 1rem      — fine print, labels
text-sm:   0.875rem / 1.25rem   — captions, helper text
text-base: 1rem     / 1.5rem    — body text
text-lg:   1.125rem / 1.75rem   — emphasized body
text-xl:   1.25rem  / 1.75rem   — card titles
text-2xl:  1.5rem   / 2rem      — section headings
text-3xl:  1.875rem / 2.25rem   — page headings
text-4xl:  2.25rem  / 2.5rem    — hero headings
```
