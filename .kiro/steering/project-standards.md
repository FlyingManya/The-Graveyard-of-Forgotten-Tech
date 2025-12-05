---
inclusion: always
---

# 👻 Graveyard of Forgotten Tech - Project Standards

## Project Overview
This is a spooky-themed interactive website that reimagines vintage technology with modern capabilities. Each invention has three stages: Grave → Haunted House → Lab → Invention Demo.

## Code Standards

### HTML Structure
- All pages must include the ghost emoji 👻 in the title
- Title format: `👻 [Page Name] - Graveyard of Forgotten Tech`
- Use semantic HTML5 elements
- Include proper meta tags for viewport and charset

### CSS Standards
- Use spooky theme colors:
  - Primary: `#8a2be2` (purple)
  - Background: `linear-gradient(135deg, #0a0a0f 0%, #1a0f1f 50%, #0f0a1a 100%)`
  - Accent: `#ffaa00` (amber/orange)
- Add subtle animations for atmosphere (flicker, pulse, glow)
- Use `backdrop-filter: blur(10px)` for glassmorphism effects

### JavaScript Standards
- Use vanilla JavaScript (no frameworks)
- Store user data in localStorage when needed
- Add keyboard shortcuts for better UX
- Use event delegation for dynamic elements

### File Organization
```
/html - Main navigation pages
/Labs - Interactive lab pages for each invention
/haunted_house - Story/lore pages for each invention
/graves - Memorial pages for each invention
/inventions - Working demos of reimagined tech
/buttons - SVG button assets
/css - Shared stylesheets
/gifs - Animated assets
```

### Navigation Flow
1. Home → Introduction → Menu
2. Menu → Graveyard (select invention)
3. Graveyard → Grave (read history)
4. Grave → Haunted House (hear ghost story)
5. Haunted House → Lab (see controls)
6. Lab → Invention (interact with demo)

## Invention Standards

### Each Invention Must Have:
1. **Description file** - Markdown with full concept
2. **Grave page** - Historical context
3. **Haunted House page** - Ghost/inventor story
4. **Lab page** - Preview/controls
5. **Working demo** - Interactive HTML/CSS/JS

### Demo Requirements
- Spooky purple theme
- Back button to lab
- Interactive controls
- Visual feedback on actions
- localStorage for persistence (if applicable)
- Responsive design

## Current Inventions
- 📷 Camera (Film → Digital Hybrid)
- 📻 Radio (Vintage → AI Storyteller)
- 📞 Telephone (Rotary → Smart Home Controller)
- 💿 CD (Player → Offline Media Hub)
- 📼 Cassette (Recorder → AI Thought Journal)
- 💾 Floppy Disk (Storage → Cloud Key)
- 💡 Lamp (Lava → Mood Tracker)
- ✉️ Letter (Mail → Digital Pen Pal)
- 📽️ Projector (Slide → AR Story Viewer)

## Testing Guidelines
- Test all navigation paths
- Verify localStorage persistence
- Check responsive design on mobile
- Test keyboard shortcuts
- Validate all links work correctly

## Deployment
- Hosted on Vercel
- Root index.html redirects to html/index.html
- All assets use relative paths
- Images preloaded for performance
