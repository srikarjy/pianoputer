# 🎹 Pianoputer - Modern Web Piano

A beautiful, interactive web-based piano application that transforms your computer keyboard into a fully functional musical instrument. Built with modern web technologies and featuring a stunning glassmorphism design.

![Pianoputer Demo](https://img.shields.io/badge/Status-Live%20Demo-brightgreen)
![License](https://img.shields.io/badge/License-MIT-blue)
![Web Audio API](https://img.shields.io/badge/Web%20Audio%20API-Supported-green)

## ✨ Features

### 🎵 **Core Piano Functionality**
- **13-note piano keyboard** (1 octave + 1 note)
- **Real-time audio synthesis** using Web Audio API
- **Multiple waveforms**: Sine, Square, Sawtooth, Triangle
- **Polyphonic playback** (up to 10 simultaneous notes)
- **Volume and octave controls**
- **Sustain pedal** (Spacebar)

### 🎼 **Advanced Features**
- **Recording & Playback**: Record your performances and play them back
- **Download recordings** as JSON files
- **Chord detection**: Automatically identifies major, minor, diminished, augmented, and 7th chords
- **Metronome**: Built-in rhythm keeper with adjustable BPM (40-240)
- **Audio visualizer**: Real-time animated bars that react to your playing

### 🎹 **Input Methods**
- **Computer keyboard mapping**: A-W-S-E-D-F-T-G-Y-H-U-J-K
- **Mouse/touch support**: Click or tap piano keys
- **Responsive design**: Works on desktop, tablet, and mobile

### 🎨 **Visual Design**
- **Glassmorphism UI**: Modern frosted glass effect
- **Gradient backgrounds**: Beautiful purple/blue theme
- **Smooth animations**: 60fps key press animations
- **Responsive layout**: Adapts to any screen size

## 🚀 Quick Start

### **Option 1: Direct File Opening**
1. Download `index.html`
2. Double-click to open in your browser
3. Click anywhere to enable audio
4. Start playing!

### **Option 2: Local Server (Recommended)**
```bash
# Using Python
python3 -m http.server 8000

# Using Node.js
npx serve .

# Then visit http://localhost:8000
```

## 🎯 How to Play

### **Keyboard Mapping**
| Computer Key | Piano Note | Computer Key | Piano Note |
|-------------|------------|-------------|------------|
| A | C | T | F# |
| W | C# | G | G |
| S | D | Y | G# |
| E | D# | H | A |
| D | E | U | A# |
| F | F | J | B |
| | | K | C (next octave) |

### **Controls**
- **Volume Slider**: Adjust overall volume (0-100%)
- **Octave Selector**: Change pitch range (0-8, default 4)
- **Waveform Selector**: Choose sound character
- **BPM Control**: Set metronome tempo (40-240 BPM)
- **Spacebar**: Sustain pedal (hold to sustain notes)

### **Recording Features**
- **Record Button**: Start/stop recording your performance
- **Play Button**: Replay your recorded performance
- **Download Button**: Save recording as JSON file

## 🛠️ Technical Details

### **Built With**
- **HTML5**: Semantic structure
- **CSS3**: Modern styling with CSS Grid, Flexbox, and custom properties
- **JavaScript ES6+**: Class-based architecture with Web Audio API
- **Web Audio API**: Real-time audio synthesis and processing

### **Browser Support**
- ✅ Chrome 66+
- ✅ Firefox 60+
- ✅ Safari 14+
- ✅ Edge 79+

### **Audio Features**
- **Equal temperament tuning** (A4 = 440Hz)
- **ADSR envelope** for natural sound
- **Polyphony management** (max 10 simultaneous notes)
- **Audio context auto-resume** for better compatibility

## 🎼 Music Theory Features

### **Chord Detection**
The app automatically detects and displays:
- **Major chords** (C, D, E, F, G, A, B)
- **Minor chords** (Cm, Dm, Em, Fm, Gm, Am, Bm)
- **Diminished chords** (Cdim, Ddim, etc.)
- **Augmented chords** (Caug, Daug, etc.)
- **7th chords** (Major 7th, Minor 7th)

### **Metronome**
- **Visual indicator**: Pulsing dot shows beat
- **Audio feedback**: Different tones for strong/weak beats
- **Adjustable tempo**: 40-240 BPM range

## 📱 Mobile Experience

The app is fully responsive and optimized for mobile devices:
- **Touch-friendly controls**: Large buttons and sliders
- **Adaptive layout**: Piano keys scale to screen size
- **Gesture support**: Tap piano keys to play
- **Mobile audio**: Optimized for mobile browsers

## 🔧 Customization

### **Modifying Key Mappings**
Edit the `keyMap` object in the JavaScript to change keyboard mappings:

```javascript
this.keyMap = {
  'a': 0,  // C
  'w': 1,  // C#
  // ... customize as needed
};
```

### **Adding New Waveforms**
Extend the waveform selector with new oscillator types:

```javascript
<option value="custom">Custom Waveform</option>
```

### **Changing Visual Theme**
Modify CSS custom properties in the `:root` selector:

```css
:root {
  --bg-gradient: linear-gradient(135deg, #your-colors 0%, #your-colors 100%);
  --accent: #your-accent-color;
}
```

## 🎵 Use Cases

- **Music Education**: Learn piano basics and music theory
- **Practice Tool**: Use metronome and recording features for practice
- **Composition**: Quick musical idea sketching
- **Entertainment**: Fun musical instrument for casual play
- **Development**: Web Audio API learning and experimentation

## 🤝 Contributing

Contributions are welcome! Here are some ideas:
- Add more instrument sounds
- Implement MIDI support
- Add sheet music display
- Create song library
- Add multiplayer features
- Enhance visual effects

### **Development Setup**
1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Test thoroughly
5. Submit a pull request

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- **Web Audio API** for real-time audio synthesis
- **CSS Glassmorphism** for modern UI design
- **Music theory resources** for chord detection algorithms
- **Open source community** for inspiration and tools

## 📞 Support

If you encounter any issues or have questions:
1. Check the browser console for error messages
2. Ensure your browser supports Web Audio API
3. Try refreshing the page
4. Open an issue on GitHub

---

**Enjoy making music with Pianoputer! 🎹✨**
