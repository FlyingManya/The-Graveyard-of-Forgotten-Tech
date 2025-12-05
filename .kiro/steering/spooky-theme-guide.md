---
inclusion: fileMatch
fileMatchPattern: "**/*.html"
---

# 👻 Spooky Theme Implementation Guide

This guide is automatically included when working with HTML files to ensure consistent spooky theming.

## Color Palette

### Primary Colors
```css
--spooky-purple: #8a2be2;
--spooky-purple-dark: #4b0082;
--spooky-purple-light: rgba(138, 43, 226, 0.3);
--spooky-black: #0a0a0f;
--spooky-dark-purple: #1a0f1f;
--spooky-amber: #ffaa00;
--spooky-red: #ff3333;
```

### Background Gradients
```css
/* Main background */
background: linear-gradient(135deg, #0a0a0f 0%, #1a0f1f 50%, #0f0a1a 100%);

/* Overlay glow */
background: radial-gradient(circle at 20% 30%, rgba(138, 43, 226, 0.03) 0%, transparent 50%);
```

## Animation Effects

### Spooky Pulse
```css
@keyframes spookyPulse {
    0%, 100% { opacity: 0.5; }
    50% { opacity: 0.8; }
}
animation: spookyPulse 8s ease-in-out infinite;
```

### Flicker (for text/lights)
```css
@keyframes flicker {
    0%, 100% { opacity: 1; }
    50% { opacity: 0.95; }
}
animation: flicker 3s ease-in-out infinite;
```

### Glow Effect
```css
box-shadow: 0 0 15px rgba(138, 43, 226, 0.2);
text-shadow: 0 0 20px rgba(138, 43, 226, 0.6);
```

## UI Components

### Buttons
```css
.spooky-button {
    background: linear-gradient(135deg, rgba(138, 43, 226, 0.4) 0%, rgba(75, 0, 130, 0.4) 100%);
    border: 2px solid rgba(138, 43, 226, 0.5);
    color: white;
    padding: 12px 24px;
    border-radius: 8px;
    cursor: pointer;
    transition: all 0.3s ease;
    backdrop-filter: blur(10px);
}

.spooky-button:hover {
    background: linear-gradient(135deg, rgba(138, 43, 226, 0.6) 0%, rgba(75, 0, 130, 0.6) 100%);
    transform: translateY(-2px);
}
```

### Cards/Panels
```css
.spooky-panel {
    background: rgba(10, 10, 15, 0.9);
    padding: 40px;
    border-radius: 20px;
    border: 2px solid rgba(138, 43, 226, 0.2);
    box-shadow: 0 8px 32px rgba(0, 0, 0, 0.6);
    backdrop-filter: blur(10px);
}
```

## Emojis to Use
- 👻 Ghost (primary mascot)
- 🪦 Tombstone (graves)
- 🕷️ Spider
- 🦇 Bat
- 🌙 Moon
- ⭐ Stars
- 🎃 Pumpkin
- 💀 Skull
- 🕯️ Candle
- 🔮 Crystal ball

## Typography
- Primary font: `'Georgia', serif` (elegant, vintage feel)
- Monospace: `'Courier New', monospace` (for technical displays)
- Headers: Large, with glow effect
- Body: Readable, good contrast

## Accessibility
- Maintain sufficient contrast ratios
- Provide hover states for interactive elements
- Include keyboard navigation
- Use semantic HTML
- Add ARIA labels where needed

## Performance
- Preload critical images
- Use CSS animations over JavaScript when possible
- Optimize image sizes
- Lazy load non-critical content
