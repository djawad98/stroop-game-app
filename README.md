# 🎮 Stroop Effect Voice Game

An interactive, browser-based implementation of the Stroop Effect cognitive test using Web Speech API for voice recognition. Challenge yourself by reading the color you see, not the word written!

## 📋 About the Stroop Effect

The Stroop Effect is a cognitive psychology phenomenon where the mind takes more time to process conflicting information. In this game, you'll see color names written in different colors and must identify the actual color displayed, not the word itself.

**Example:**
- You see the word "Red" but it's colored **Blue**
- The correct answer is **Blue** (the color you see), not Red (the word)

## 🎯 Features

- **Voice Recognition**: Uses Web Speech API to capture and recognize color names from your voice
- **Three-Screen Flow**:
  - Welcome screen with game instructions
  - Game screen with interactive color challenges
  - Results screen with detailed performance analysis
  
- **Smart Game Generation**: Ensures no repeated colors in any single challenge
- **Real-time Feedback**: Shows recognized colors as you speak
- **Detailed Error Analysis**: 
  - Color-by-color comparison of expected vs. actual answers
  - Identifies common issues (wrong colors, missed colors, extra colors)
  - Provides helpful tips for improvement

- **Responsive Design**: Works on desktop, tablet, and mobile browsers
- **Dark Theme UI**: Easy on the eyes with smooth animations
- **No External Dependencies**: Runs entirely in the browser with a single HTML file

## 🚀 Getting Started

### Quick Start
1. Download or clone this repository
2. Open `index.html` in any modern web browser
3. Click "Start Game" and follow the on-screen instructions

### Browser Requirements
- **Chrome/Chromium**: Full support
- **Firefox**: Full support
- **Safari**: Full support
- **Edge**: Full support

**Note**: Web Speech API requires a browser that supports the Web Speech API. All modern browsers support this feature.

## 🎮 How to Play

1. **Start**: Click "Start Game" on the welcome screen
2. **View Colors**: See 5 color names displayed in different colors
3. **Record**: Click the "Record" button (🎤) to start listening
4. **Speak**: Say the color you **see** (not the word written), in order, for each item
5. **Results**: View your score and get detailed feedback on your performance

### Example Gameplay
```
You see:
- "Red" (but in blue color) → Say "Blue"
- "Green" (but in yellow color) → Say "Yellow"
- "Black" (but in red color) → Say "Red"
... and so on for 5 colors
```

## 📊 Scoring

- **Score**: Number of colors correctly identified out of 5
- **Perfect Score**: 5/5 - All colors identified correctly
- **Feedback**: Detailed analysis of which colors you got right/wrong

## 🛠️ Technical Stack

- **HTML5**: Semantic markup
- **CSS3**: Modern styling with animations and transitions
- **JavaScript (ES6+)**: Game logic and Web Speech API integration
- **Web APIs**:
  - Web Speech API for voice recognition
  - DOM APIs for UI interactions
  - LocalStorage (not used - game state managed in memory)

## 📁 Project Structure

```
stroop-effect-voice-game/
├── index.html          # Main game file (contains HTML, CSS, and JS)
├── README.md           # This file
└── (No external dependencies)
```

## 🔧 Customization

You can easily customize the game by editing `index.html`:

### Change Colors
Edit the `colors` array in the JavaScript section:
```javascript
const colors = ['Red', 'Green', 'Blue', 'Yellow', 'Black'];
```

### Change Color Hex Values
Edit the `colorHex` object:
```javascript
const colorHex = {
  Red: '#ef4444',
  Green: '#22c55e',
  Blue: '#3b82f6',
  Yellow: '#fbbf24',
  Black: '#1a1a1a'
};
```

### Change Game Difficulty
Modify the number of colors in each game (currently 5):
```javascript
for (let i = 0; i < 5; i++) {  // Change 5 to any number
  // ...
}
```

## 🚀 Deployment

### Deploy to GitHub Pages

1. Create a new GitHub repository
2. Push this code to GitHub:
   ```bash
   git init
   git add .
   git commit -m "Initial commit: Stroop Effect Voice Game"
   git remote add origin https://github.com/YOUR_USERNAME/stroop-effect-voice-game.git
   git push -u origin main
   ```

3. Enable GitHub Pages:
   - Go to repository **Settings** → **Pages**
   - Select `main` branch as source
   - Your game will be live at: `https://YOUR_USERNAME.github.io/stroop-effect-voice-game`

### Other Hosting Options
- **Netlify**: Drag and drop `index.html`
- **Vercel**: Connect your GitHub repository
- **Any Static Hosting**: Upload `index.html` and access via your domain

## 🎨 UI/UX Features

- **Smooth Animations**: Fade-in effects for screens, pop-in animations for buttons
- **Color Feedback**: Green for success, red for errors
- **Real-time Status**: See recognized colors as you speak
- **Mobile Responsive**: Optimized for all screen sizes
- **Dark Theme**: Reduces eye strain during extended play

## ⚙️ Browser Compatibility

| Feature | Chrome | Firefox | Safari | Edge |
|---------|--------|---------|--------|------|
| Web Speech API | ✅ | ✅ | ✅ | ✅ |
| CSS Grid | ✅ | ✅ | ✅ | ✅ |
| CSS Animations | ✅ | ✅ | ✅ | ✅ |
| ES6 JavaScript | ✅ | ✅ | ✅ | ✅ |

## 🐛 Troubleshooting

### Microphone Not Working
- Check browser microphone permissions
- Allow the website to access your microphone when prompted
- Restart the browser if permissions were denied

### Speech Recognition Not Recognized
- Speak clearly and at a normal pace
- Make sure background noise is minimal
- Try saying the color name alone without extra words

### Game Not Loading
- Make sure you're using a modern browser
- Clear browser cache and reload
- Try a different browser

## 📚 Educational Use

This game is great for:
- **Psychology Students**: Learning about the Stroop Effect
- **Cognitive Training**: Improving attention and focus
- **Speech Recognition Practice**: Testing voice input in web apps
- **Programming Learning**: Understanding Web Speech API implementation

## 🔐 Privacy

- **No Data Collection**: This game doesn't collect or send any personal data
- **Local Processing**: All speech recognition happens locally in your browser
- **No Tracking**: No analytics or third-party services

## 📝 License

This project is open source and available for educational and personal use.

## 🤝 Contributing

Found a bug? Have a feature idea? Feel free to:
1. Open an issue on GitHub
2. Create a pull request with improvements
3. Share feedback and suggestions

## 📧 Contact

For questions or suggestions, reach out through GitHub Issues.

---

**Enjoy the challenge! Can you master the Stroop Effect? 🧠**

Made with ❤️ using vanilla HTML, CSS, and JavaScript