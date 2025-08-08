# 3D First-Person Shooter Game

A fully-featured browser-based 3D FPS game built with Three.js. Experience intense combat with advanced mechanics including dismemberment physics, combo-based perks, and visceral gore effects.

## Features

### Core Gameplay
- **First-person shooter mechanics** with smooth controls and responsive combat
- **Wave-based survival** with progressively challenging enemy spawns
- **Multiple weapon types** including assault rifle, shotgun, rocket launcher, and melee sword
- **Advanced enemy AI** with pathfinding and combat behaviors

### Combat System

#### Weapons
- **Assault Rifle**: Rapid-fire automatic weapon with 30-round magazines
- **Shotgun**: High-damage close-range weapon with spread pattern
- **Rocket Launcher**: Explosive projectiles with area damage
- **Sword**: Melee weapon with wide swing arc for close combat

#### Special Mechanics
- **Headshot System**: Precision shots deal bonus damage (+50 points) with special effects
- **Dismemberment**: Dynamic gore system with flying limbs and blood effects
- **Blood Trails**: Dismembered parts leave realistic blood trails
- **Screen Shake**: Impact feedback for explosions and heavy hits

### Perk System

#### Adrenaline (Sword Exclusive)
- Triggered by 3 rapid sword kills
- Doubles movement speed for 5 seconds
- Enhanced agility for melee combat

#### Blood Thirst
- Activated after 5-kill streak
- Unlimited ammo for 10 seconds
- Rapid-fire capability for all weapons

#### Hellfire
- Unlocked at 10-kill streak
- Explosive rounds for all weapons
- 25% increased blast damage and radius
- Instakill within blast zone

#### BERSERK
- Requires 15-kill combo
- Multiple weapon enhancements:
  - 3x fire rate increase
  - 5x damage multiplier
  - Unlimited ammo
  - Invulnerability
  - 2x movement speed
- Duration: 10 seconds

#### SLOWMO
- Triggered by 3 rapid headshots
- Time dilation to 25% speed
- Audio pitch modulation
- Player maintains normal speed
- Strategic advantage window

## Controls

### Movement
- **W/A/S/D** - Move forward/left/backward/right
- **Mouse** - Look around
- **Space** - Jump
- **Shift** - Sprint

### Combat
- **Left Click** - Fire weapon
- **R** - Reload
- **1** - Assault Rifle
- **2** - Shotgun
- **3** - Rocket Launcher
- **4** - Sword

### System
- **ESC** - Pause menu
- **F** - Toggle FPS counter
- **G** - Debug mode (collision boxes)

## Technical Details

### Built With
- **Three.js r128** - 3D graphics rendering
- **Vanilla JavaScript** - No framework dependencies
- **Web Audio API** - 3D spatial audio system
- **Pointer Lock API** - FPS mouse control

### Performance Optimizations
- Object pooling for bullets and particles
- Frustum culling for off-screen objects
- LOD system for distant objects
- Efficient collision detection
- Memory leak prevention

### Visual Effects
- Dynamic particle systems
- Muzzle flash and bullet tracers
- Blood spray and gore effects
- Explosion particles
- Screen damage indicators
- Billboard sprites for effects

## Installation

1. Clone or download the repository
2. Open `fps-game.html` in a modern web browser
3. Click to start and enjoy!

No build process or server required - runs completely in the browser.

## Browser Compatibility
- Chrome (recommended)
- Firefox
- Safari
- Edge

Requires WebGL support and modern JavaScript features.

## Game Systems

### Health & Damage
- Player starts with 100 HP
- Health regenerates 5 HP/second after 3 seconds without damage
- Enemies deal contact damage
- Health pickups restore 25 HP

### Scoring
- Standard kill: 100 points
- Headshot bonus: +50 points
- Combo multipliers for streaks
- High score tracking via localStorage

### Enemy Types
- **Standard**: 50 HP, normal speed
- **Heavy**: 75 HP, slower movement
- **Elite**: 100 HP, faster and more aggressive

## Audio Features
- 3D spatial sound for directional awareness
- Dynamic audio pitch during SLOWMO
- Layered sound effects for impacts
- Weapon-specific audio
- Ambient combat sounds
- Perk activation cues

## Known Features

### Gore System
- Realistic dismemberment physics
- Blood particle effects
- Giblet physics with gravity
- Blood trail emitters
- Head removal on fatal headshots
- Explosion dismemberment

### HUD Elements
- Health bar with regeneration indicator
- Ammunition counter (current/reserve)
- Score and wave display
- Kill feed notifications
- Perk activation alerts
- Combo counter
- Crosshair with hit markers

## Development

This is a single-file HTML application containing all code inline. To modify:

1. Open `fps-game.html` in a code editor
2. Make changes to the JavaScript sections
3. Save and refresh browser to test

The game uses ES6 classes for organization:
- `Player` - Player controller and weapon management
- `Enemy` - AI behavior and pathfinding
- `ParticleSystem` - Visual effects management
- `AudioManager` - 3D audio and sound effects
- `GameManager` - Core game loop and state
- `UIManager` - HUD and interface updates

## Performance Tips

For best performance:
- Close other browser tabs
- Ensure hardware acceleration is enabled
- Update graphics drivers
- Use Chrome for optimal WebGL performance
- Adjust browser zoom to 100%

## Credits

Created as a demonstration of modern web game development capabilities using Three.js and vanilla JavaScript. Showcases advanced FPS mechanics typically found in desktop games, running entirely in the browser.

## License

This project is provided as-is for educational and entertainment purposes.