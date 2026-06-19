# Geometry Dash Copy - Rhythm Platformer Game

A complete, self-contained browser-based rhythm-platformer game engine built with vanilla HTML, CSS, and JavaScript.

## Features

### Gameplay Modes
- 🟦 **Cube**: Classic rectangular platformer
- 🛸 **Ship**: Rotation-based flying mode
- ⚽ **Ball**: Rolling platformer
- 🚀 **UFO**: Gravity-defying exploration
- 〰️ **Wave**: Sinusoidal movement
- 🤖 **Robot**: Jumping mode
- 🕷️ **Spider**: Climbing mechanics

### Level Features
- **8 Original Levels**: Stellar Start → Void Voyage (Easy to Insane)
- **Gravity Flip Portals**: Dynamically reverse gravity mid-level
- **Speed Modifiers**: Temporary speed boost/reduction zones
- **Jump Pads**: Yellow pads for enhanced jumping
- **Orbs**: Collectible spheres for extra boosts
- **Obstacles**: Green blocks and red spikes
- **Progress Tracking**: Real-time percentage display
- **Best Attempt Tracker**: Automatic highest progress storage

### Modes
- **Story Mode**: 8 levels of increasing difficulty
- **Practice Mode**: Unlimited attempts, no death penalty
- **Level Select**: Choose any level to replay

### UI/UX
- Clean menu system
- Real-time progress indicator
- Attempt counter
- Game over/level complete screens
- Pause menu (ESC key)
- Responsive design

## Controls

| Action | Key/Click |
|--------|----------|
| Jump | **SPACE** or **CLICK** |
| Pause | **ESC** |
| Restart Level | **R** |

## Installation

1. **Download all files** to a local directory
2. **Open `index.html`** in a modern web browser
3. Click "Play" to start

### Or Deploy Online

**GitHub Pages**:
1. Push to a GitHub repository
2. Enable Pages in Settings → Pages
3. Select main branch
4. Access at `https://username.github.io/repo-name/`

**Netlify** (recommended):
1. Drag and drop `index.html` onto [netlify.com](https://netlify.com)
2. Get instant public URL

**Vercel**:
1. Upload to [vercel.com](https://vercel.com)
2. Auto-deployed and live

## Game Structure

### Level Format
Levels use a simple tile-based notation:
- `B` = Block (platform)
- `S` = Spike (hazard)
- `J` = Jump Pad (enhanced jump)
- `O` = Orb (collectible)
- `P` = Portal (gravity flip)
- `C` = Checkpoint (respawn point)

Example: `B:B:S:J:O:B` creates a 6-tile level.

### Difficulty Progression
1. **Stellar Start** (Easy) - Introduction
2. **Lunar Landing** (Easy) - Basic platforming
3. **Solar Storm** (Normal) - Jump pad challenges
4. **Cosmic Challenge** (Normal) - Spike avoidance
5. **Nebula Rush** (Hard) - Complex patterns
6. **Pulsar Panic** (Hard) - Rapid sequences
7. **Supernova** (Insane) - Ultimate test
8. **Void Voyage** (Insane) - Final boss level

## Technical Details

### Technologies
- **HTML5**: Canvas API for rendering
- **CSS3**: Flexbox for UI, gradients for styling
- **Vanilla JavaScript**: No dependencies
- **localStorage**: For persistent progress tracking

### Performance
- 60 FPS target
- Efficient collision detection
- Optimized particle effects
- Smooth camera following

### Browser Support
- Chrome/Edge (recommended)
- Firefox
- Safari
- Opera

## Customization

### Add Custom Levels
Edit the `LEVELS` array in the JavaScript:

```javascript
{
    id: 9,
    name: 'Your Level Name',
    difficulty: 'Hard',
    bpm: 200,
    data: 'B:B:S:J:O:B:S:J:O:B'
}
```

### Change Colors
Modify CSS variables in `:root`:

```css
--primary-color: #4CAF50;      /* Green blocks */
--secondary-color: #2196F3;    /* Blue player */
--danger-color: #f44336;       /* Red spikes */
--warning-color: #ff9800;      /* Orange pads */
```

### Adjust Difficulty
Tweak physics constants:

```javascript
const GRAVITY = 0.6;           // Higher = faster falling
const JUMP_POWER = 15;         /* Higher = higher jumps */
const FPS = 60;                // Lower = slower game
```

## Assets & Audio

No external dependencies required. All graphics are drawn procedurally using Canvas API.

For royalty-free background music, embed from:
- [OpenGameArt.org](https://opengameart.org/)
- [Freesound.org](https://freesound.org/)
- [YouTube Audio Library](https://www.youtube.com/audiolibrary/)

## Future Enhancements

- [ ] Sound effects and music integration
- [ ] More gameplay modes (robot, spider)
- [ ] Level editor
- [ ] Multiplayer leaderboards
- [ ] Mobile touch controls
- [ ] Power-ups system
- [ ] Boss battles
- [ ] Campaign story mode

## License

Free to use and modify for personal/educational projects.

## Credits

Inspired by Geometry Dash by RobTop Games.

Built with vanilla web technologies.

---

**Ready to play?** Open `index.html` in your browser and start jumping!
