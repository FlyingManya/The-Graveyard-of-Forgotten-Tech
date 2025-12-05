<img width="1917" height="1075" alt="Screenshot 2025-11-09 164556" src="https://github.com/user-attachments/assets/d8a8c5ba-5cca-4f48-98a6-4746ce105324" />

# 👻 The Graveyard of Forgotten Tech

"The Graveyard of Forgotten Tech" is a spooky interactive web experience where forgotten inventions tell their stories — and show how they've been reborn for the modern world.

## 🎃 About

Step into a haunted graveyard where vintage technology rests... but not in peace. Each invention has been reimagined with modern capabilities while preserving its nostalgic charm. Explore interactive demos, hear ghost stories from the inventors themselves, and discover how old tech can solve new problems.

## 🕷️ Features

### Interactive Journey
- **Graveyard** - Browse tombstones of forgotten tech
- **Graves** - Learn the history of each invention
- **Haunted House** - Hear spooky stories from inventor ghosts
- **Labs** - Preview the reimagined inventions
- **Demos** - Interact with fully functional prototypes

### Current Inventions

| Invention | Original → Reimagined |
|-----------|----------------------|
| 📷 Camera | Film Camera → Digital Film Hybrid |
| 📻 Radio | Vintage Radio → AI Storyteller & Podcast Player |
| 📞 Telephone | Rotary Phone → Smart Home Controller |
| 💿 CD | CD Player → Offline Media Hub |
| 📼 Cassette | Cassette Recorder → AI Thought Journal |
| 💾 Floppy Disk | Floppy Disk → Cloud Storage Key |
| 💡 Lamp | Lava Lamp → Mood Tracking Light |
| ✉️ Letter | Handwritten Letter → Digital Pen Pal System |
| 📽️ Projector | Slide Projector → Interactive AR Story Viewer |

## 🛠️ Tech Stack

- **Frontend**: Pure HTML5, CSS3, JavaScript (Vanilla)
- **Storage**: LocalStorage for persistence
- **Deployment**: Vercel
- **Design**: Spooky purple theme with glassmorphism effects

## 🎨 Design Philosophy

- **Spooky Aesthetic**: Dark purple gradients, glowing effects, ghost emojis
- **Nostalgic Feel**: Vintage typography, retro UI elements
- **Modern UX**: Smooth animations, responsive design, keyboard shortcuts
- **Accessibility**: Semantic HTML, proper contrast, ARIA labels

## 📁 Project Structure

```
├── html/              # Main navigation pages
├── graveyard/         # Graveyard selection page
├── graves/            # Individual grave pages
├── haunted_house/     # Ghost story pages
├── Labs/              # Lab preview pages
├── inventions/        # Interactive demos
├── buttons/           # SVG button assets
├── css/               # Shared stylesheets
├── gifs/              # Animated assets
├── .kiro/
│   ├── specs/         # Feature specifications
│   ├── steering/      # Development guidelines
│   └── hooks/         # Agent automation hooks
└── README.md
```

## 🚀 Getting Started

### Prerequisites
- Modern web browser (Chrome, Firefox, Safari, Edge)
- No build tools required!

### Local Development
1. Clone the repository
```bash
git clone https://github.com/yourusername/The-Graveyard-of-Forgotten-Tech.git
cd The-Graveyard-of-Forgotten-Tech
```

2. Open in browser
```bash
# Simply open html/index.html in your browser
# Or use a local server:
python -m http.server 8000
# Then visit http://localhost:8000/html/
```

### Deployment
The project is configured for Vercel deployment with automatic redirects from root to `/html/`.

## 🎯 Kiro Features Used

This project leverages Kiro's advanced development features:

### 📋 Spec-Driven Development
- Requirements documented in `.kiro/specs/`
- Clear acceptance criteria for each feature
- Structured development workflow

### 📚 Steering Documents
- **project-standards.md** - Always included, defines coding standards
- **spooky-theme-guide.md** - Auto-included for HTML files, ensures consistent theming

### 🤖 Agent Hooks
- **check-spooky-theme** - Validates theme compliance on HTML save
- **test-invention-demo** - Reminds to test functionality when demos are updated
- **update-readme** - Manual trigger to keep documentation current

## 🎮 Interactive Demos

Each invention includes a fully functional demo:

- **Camera**: Dual capture system with film filters
- **Radio**: Tunable channels with story content
- **Telephone**: Rotary dial smart home controls
- **CD**: Media player with sync features
- **Cassette**: Voice recording with AI transcription
- **Floppy Disk**: Cloud authentication system
- **Lamp**: Mood tracking calendar
- **Letter**: Anonymous pen pal messaging
- **Projector**: Slide-based storytelling (coming soon)

## 🤝 Contributing

Contributions are welcome! Please follow the project standards in `.kiro/steering/project-standards.md`.

## 📝 License

This project is open source and available under the MIT License.

## 🙏 Acknowledgments

- Inspired by the nostalgia of vintage technology
- Built with Kiro AI development tools
- Spooky theme perfect for Halloween and beyond

## 🔗 Links

- [Live Demo](https://your-vercel-url.vercel.app)
- [Project Documentation](.kiro/specs/)
- [Development Guidelines](.kiro/steering/)

---

Made with 👻 and ❤️ for forgotten tech
