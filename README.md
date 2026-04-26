# 🎮 Dood Wala

A fully offline, instantly playable **platformer jump game** for Android built with Kotlin + Jetpack Compose.

## Gameplay

Control your quirky **Dood** character — a little yellow blob with antenna — as it bounces upward through platforms. The higher you go, the bigger your score!

### Controls
| Button | Action |
|--------|--------|
| ◀ Left | Move Dood left |
| ▶ Right | Move Dood right |

### Platform Types
| Color | Type | Effect |
|-------|------|--------|
| 🟢 Green | Normal | Standard bounce |
| 🔵 Blue | Moving | Slides left & right |
| 🔴 Red | Spring | Super-high bounce |

### Features
- 🎮 100% offline — no internet required
- ⭐ Score tracking with local leaderboard (top 10 scores)
- 📖 In-app How to Play guide
- 🌀 Wrap-around edges (walk off screen and appear the other side)
- 🏆 Leaderboard with gold/silver/bronze rankings
- 📱 Smooth 60fps Canvas-drawn game loop
- 🎨 Sky background with clouds, animated Dood character

## Build & Run

1. Open in **Android Studio Hedgehog** or later
2. Sync Gradle
3. Run on device or emulator (API 24+)

```
minSdk  : 24
targetSdk: 34
AGP     : 8.5.2
Kotlin  : 2.0.21
```

## Project Structure

```
app/src/main/java/com/doodwala/app/
├── MainActivity.kt          # Entry point & navigation
├── data/
│   └── ScoreRepository.kt   # SharedPreferences score storage
├── game/
│   ├── GameEngine.kt         # Physics, collision, platform logic
│   └── GameScreen.kt         # Compose UI + Canvas rendering
└── ui/
    ├── HomeScreen.kt          # Main menu
    ├── HowToPlayScreen.kt     # Instructions
    ├── LeaderboardScreen.kt   # Top scores
    └── theme/                 # Material 3 theme
```