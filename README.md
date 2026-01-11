# RedPulse Talker

A futuristic, interactive web experience with a sleek neon aesthetic. RedPulse Talker features immersive visual effects, custom interactions, and ambient audio to create an engaging user interface.

## Project Overview

**RedPulse Talker** is a modern web application that combines cutting-edge UI design with interactive JavaScript modules. The project emphasizes visual feedback, smooth animations, and an immersive user experience with a red/crimson neon theme.

**Tagline:** *"It sees. It reacts. It speaks."*

## Features

### 🎨 Visual Design
- **Neon Red Theme** - Bold red (#ff0033) accents with glowing text-shadow effects
- **Responsive Layout** - Adapts to different screen sizes with flexible viewport units
- **Custom Cursor** - Smooth, glowing circular cursor with motion smoothing and click feedback
- **Animated Background** - Dynamic background powered by Unicorn Studio with integrated 3D visual effects

### 🎧 Audio
- **Ambient Background Music** - Looping background audio that fades in smoothly
- **User-Triggered Playback** - Audio starts on first user interaction (click or touch)
- **Volume Control** - Configurable fade-in effect for seamless audio integration

### 🖱️ Interactivity
- **Custom Cursor System** - Replaces default cursor with animated, glowing element
- **Responsive Buttons** - "TALK TO ME" and "EXPLORE INTERFACE" CTAs with hover effects
- **Motion Smoothing** - Fluid cursor tracking with lag effects for visual appeal

### 🎬 Background Animation
- **Unicorn Studio Integration** - Loads dynamic 3D backgrounds from Unicorn Studio CDN
- **Full-Screen Overlay** - Background spans entire viewport behind hero content

## Project Structure

```
IEEE/
├── index.html              # Main HTML file with hero section
├── style.css               # Styling with neon theme and animations
├── assets/
│   ├── hero.gif           # Hero section animated GIF
│   └── audio.mp3          # Background ambient audio
├── modules/
│   ├── CustomCursor.js    # Custom cursor implementation
│   ├── AudioPlayer.js     # Audio playback manager
│   └── UnicornBackground.js # Unicorn Studio background handler
└── ind.html               # Legacy/alternate HTML file
```

## Modules

### CustomCursor.js
Implements a custom cursor with visual effects and smooth motion tracking.

**Features:**
- Configurable size and color (default: 30px red glow)
- Multi-layer shadow effect for enhanced glow
- Smooth motion with configurable lag (speed: 0.2)
- Scale-down effect on click ("pop" feedback)
- Automatic cursor hiding

**Usage:**
```javascript
new CustomCursor({ 
  size: 30, 
  color: 'rgba(255,0,51,0.8)' 
});
```

### AudioPlayer.js
Manages background audio playback with fade-in effects.

**Features:**
- Triggers on first user interaction (click or touch)
- Smooth fade-in volume control (200ms intervals)
- Configurable volume level (default: 0.3)
- Handles autoplay restrictions gracefully

**Usage:**
```javascript
new AudioPlayer("#bg-audio", { volume: 0.3 });
```

### UnicornBackground.js
Loads and initializes dynamic background animations via Unicorn Studio CDN.

**Features:**
- Lazy loads Unicorn Studio library
- Prevents duplicate initialization
- Project-specific background ID support
- Console logging for debugging

**Usage:**
```javascript
new UnicornBackground("xiQy6B0JfgInCheMAGOM");
```

## Styling Highlights

### Typography
- **Font:** Public Sans (Google Fonts) with weights 100-900
- **Hero Title:** 8vw font size, all caps, letter-spaced
- **Accent:** "Talker" text in bright red (#ff0033)

### Color Scheme
- **Primary:** Deep black background
- **Accent:** Red (#ff0033) with glow effects
- **Text:** White with red text-shadow

### Animations
- **Button Hover:** Scale up (1.08x) with enhanced glow
- **Ghost Button:** Red background fade on hover
- **Voice Indicator:** Animated red bars (for audio feedback)

## Getting Started

1. **Open the project** - Open `index.html` in a modern web browser
2. **Interact** - Click anywhere to start the background audio
3. **Explore** - Click the hero buttons to interact with the interface
4. **Customize** - Modify options in `index.html` module initialization

### Browser Requirements
- Modern browser with ES6 module support
- Audio playback capabilities
- WebGL support (for Unicorn Studio background)

## Configuration

### Customize Colors
Edit `CustomCursor` initialization in `index.html`:
```javascript
new CustomCursor({ 
  size: 30, 
  color: 'rgba(255,0,51,0.8)' // Change color here
});
```

### Adjust Audio Volume
Modify the `AudioPlayer` initialization:
```javascript
new AudioPlayer("#bg-audio", { volume: 0.5 }); // Increase to 0.5
```

### Change Background Project
Update the Unicorn Studio project ID:
```javascript
new UnicornBackground("YOUR_PROJECT_ID");
```

## Dependencies

- **Unicorn Studio** - CDN-loaded 3D animation platform
- **Google Fonts** - Public Sans typeface
- No npm/package manager required

## Browser Compatibility

- Chrome/Edge 88+
- Firefox 87+
- Safari 14+
- Mobile browsers with ES6 support

## Notes

- Audio autoplay may be restricted by browser policies; the first user interaction triggers playback
- Custom cursor uses `pointer-events: none` to maintain button click functionality
- Background component z-index (1) is behind hero container (z-index: 10)
- Unicorn Studio script loads asynchronously to prevent blocking

## License

This project appears to be part of an IEEE initiative. Check with project maintainers for license details.

 January 2026
