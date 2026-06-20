# Milestone 3 — Theme Toggle Button

**Status:** ✅ Complete

## What this milestone does

Adds a sun/moon icon button to the navbar that switches between dark and light themes. Preference is saved to `localStorage` so it persists across page reloads.

## Implementation Details

### HTML
A `<button id="theme-toggle">` added inside the `<nav>` on the right side. Uses FontAwesome icons:
- Dark mode active → show `fa-sun` (click to go light)
- Light mode active → show `fa-moon` (click to go dark)

### CSS
- Button positioned to the right of nav links (flexbox with `margin-left: auto`)
- Circular button, no border, accent-colored icon
- Smooth icon swap via CSS visibility or JS class toggle

### JS Logic
```js
const root = document.documentElement;
const btn = document.getElementById('theme-toggle');
const saved = localStorage.getItem('theme') || 'dark';

root.setAttribute('data-theme', saved);
updateIcon(saved);

btn.addEventListener('click', () => {
  const next = root.getAttribute('data-theme') === 'dark' ? 'light' : 'dark';
  root.setAttribute('data-theme', next);
  localStorage.setItem('theme', next);
  updateIcon(next);
});

function updateIcon(theme) {
  btn.innerHTML = theme === 'dark'
    ? '<i class="fas fa-sun"></i>'
    : '<i class="fas fa-moon"></i>';
}
```

## Tasks

- [x] Add theme toggle button HTML to navbar
- [x] Add button CSS (positioned right, circular, accent icon)
- [x] Add JS: read localStorage on load, toggle on click, update icon
- [x] Verify smooth transition (0.3s) when toggling

## Verification

1. Load page — should default to dark theme
2. Click toggle — switches to light, icon changes to moon
3. Reload page — light theme persists
4. Click again — back to dark, icon changes to sun
