# 🥷 Kanji's Adventure

A tribute to Motion Twin's adventure game. In this roguelike dungeon crawler, a brave ninja (Kanji) explores procedurally generated dungeons, fights monsters, and collects treasures. Written entirely in vanilla JavaScript, HTML, and CSS, this game demonstrates how to create an engaging gaming experience using just web technologies.

![image](https://github.com/user-attachments/assets/81aaecad-1d1c-488d-b118-6d6836f56268)


## 🎮 Gameplay

### Core Mechanics
- **Dungeon Exploration**: Navigate through procedurally generated dungeons with interconnected rooms
- **Turn-based Combat**: Strategic fights against various monsters
- **Resource Management**: Balance health and energy while exploring
- **Item Collection**: Find and use various items to aid your adventure

### Controls
- **Arrow Keys**: Move Kanji in four directions
- **Combat**: Move towards monsters to engage in combat
- **Item Collection**: Move over items to collect them
- **Level Navigation**: Use stairs (⬆️/⬇️) to move between dungeon levels

### Monsters
| Monster  | Difficulty | Special Traits |
|----------|------------|----------------|
| Ghost    | Easy       | Basic enemy    |
| Goblin   | Easy       | Drops valuable loot |
| Fire Imp | Medium     | Chases player  |
| Skeleton | Hard       | High damage    |
| Shaman   | Very Hard  | Powerful magic |

### Items
- **Consumables**: 
  - Meat (Restores 100 energy)
  - Apple (Restores 50 energy)
  - Small Potion (Restores 8 HP)
- **Equipment**:
  - Knife (3 damage)
  - Katana (5 damage)
  - Leather Armor (1 defense)
  - Iron Armor (2 defense)
- **Treasures**:
  - Coins (Used for scoring)
  - Emerald (+1000 points)
  - Sapphire (+3000 points)
  - Ruby (+8000 points)

### Scoring System
- Monster defeats
- Collected coins (×20)
- Remaining energy (×5)

## 🔧 Technical Implementation

### Architecture
- **Pure Frontend**: No dependencies, built with vanilla JavaScript
- **Single Page**: Everything contained in one HTML file
- **CSS Grid**: Used for dungeon layout
- **Event-based**: Keyboard input handling for player control

### Key Features
- **Procedural Generation**: Custom algorithm for dungeon creation
- **Rarity System**: Weighted random selection for monsters and items
- **Collision Detection**: Grid-based movement and interaction system
- **Combat System**: Turn-based combat with damage calculations
- **State Management**: Game state handled through JavaScript objects

### Dungeon Generation
```javascript
// Example of room generation parameters
const BOARD_SIZE = 15;
const ROOM_SIZE = 5;
const minRoomSize = 3;
const maxRoomSize = 6;
```

The dungeon is generated using:
1. Room placement with variable sizes
2. Corridor generation between rooms
3. Entity placement (monsters, items, stairs)
4. Validation to ensure all areas are accessible

### Rarity System
```javascript
const RARITY_WEIGHTS = {
    common: 50,
    uncommon: 30,
    rare: 15,
    very_rare: 4,
    legendary: 1
};
```

## 🚀 Getting Started

### Play Now
1. Visit [Game URL will be added soon :)]
2. Use arrow keys to move
3. Explore and survive!

### Local Development
1. Clone the repository
```bash
git clone https://github.com/yourusername/kanjis-adventure.git
```
2. Open `index.html` in a web browser
3. No build process or dependencies required!

## 🛠️ Future Improvements
- [ ] Save/Load system
- [ ] Additional monster types
- [ ] More item varieties
- [ ] Advanced combat mechanics
- [ ] Boss battles
- [ ] Sound effects and music

## 🤝 Contributing
Contributions are welcome! Feel free to:
1. Fork the repository
2. Create a feature branch
3. Submit a pull request

## 🙏 Acknowledgments
- Game design inspired by classic roguelikes
- Emoji assets used for characters and items
- [Any other acknowledgments]

---
Made with ❤️ by [Your Name]
