You are a senior Flutter game developer and Play Store production engineer.

Analyze my complete Flutter game codebase and upgrade it into a production-ready mobile game application similar to Block Blast.

Game Name: ZenWood

Tech Stack:
- Flutter
- Firebase
- Google Mobile Ads
- Firestore
- Android Play Store deployment

Your task is to:
1. Analyze the full codebase architecture
2. Find bad practices, bugs, UI issues, performance issues, memory leaks
3. Refactor the project into scalable production-ready structure
4. Keep the existing game functionality working
5. Improve animations, game logic, state management, monetization, and Firebase integration

==================================================
UI & LOADING SCREEN IMPROVEMENTS
==================================================

A. Splash / Loading Screen
- Increase logo size moderately
- Place logo exactly at center
- Remove shadow effect completely
- Add soft glow/highlight effect only
- Make loading screen premium and smooth
- Ensure responsive design for all screen sizes

==================================================
LEVEL SYSTEM & GAME LOGIC
==================================================

B. Implement Proper Progressive Level System

Current game needs professional level progression.

Requirements:
- Add dynamic level logic
- Each level should have:
  - score goal
  - coin goal
  - difficulty scaling
  - increasing complexity
  - faster gameplay on higher levels

Example:
Level 1:
- Goal score: 500
- Easy gameplay
- No timer

Level 2:
- Goal score: 1000
- Slightly harder

Level 3+:
- Add timer countdown
- Increase difficulty
- Reduce move flexibility

Higher levels:
- Harder block patterns
- Faster gameplay
- More strategic difficulty

Create a scalable level configuration system.

==================================================
LEVEL COMPLETE POPUP
==================================================

C. After level completion:
- Show animated dialog popup
- Similar to professional mobile games
- Include:
  - "Level Completed"
  - earned coins
  - score
  - next level button
  - home/levels page button

Popup animation:
- scale animation
- fade animation
- particle/confetti effect if possible

After completing level:
- Rewarded ad should play automatically before next level

==================================================
COIN SYSTEM
==================================================

D. Global Coin Management System

Coins earned by users must:
- update instantly across app
- reflect on:
  - levels page
  - store page
  - profile page
  - gameplay page

Requirements:
- Use centralized state management
- Coins must persist using Firebase/local storage
- User can spend coins in store
- Purchased items should remain unlocked

==================================================
POWER-UP ANIMATIONS
==================================================

E. Add premium animations for power-ups:
- Hammer smash animation
- Bomb blast animation
- Thunder/lightning effect
- Screen shake effects
- Particle explosions
- Sound trigger integration support

Animations should feel smooth and premium.

==================================================
LEADERBOARD SYSTEM
==================================================

F. Build 24-hour Global Leaderboard

Requirements:
- Store user score in Firebase Firestore
- Track highest scores every 24 hours
- Show:
  - username
  - highest score
  - ranking

Leaderboard resets every 24 hours automatically.

Display leaderboard to all users globally.

Implement:
- Firebase structure
- queries
- indexes
- security rules
- cleanup logic
- efficient leaderboard fetching

==================================================
PRODUCTION READY REQUIREMENTS
==================================================

G. Make the entire app Play Store production ready.

Requirements:
- optimize performance
- remove unnecessary rebuilds
- proper folder structure
- scalable architecture
- responsive UI
- proper null safety
- clean code
- proper naming conventions
- loading states
- error handling
- Firebase optimization
- ad optimization
- anti-crash improvements

==================================================
ADS & MONETIZATION
==================================================

H. Ads Improvements
- Ensure rewarded ads work properly
- Prevent ad spam
- Proper ad lifecycle handling
- Retry loading on failure
- Optimize ad placements

==================================================
FIREBASE & BACKEND
==================================================

I. Firebase Improvements
- optimize firestore reads/writes
- secure firestore rules
- improve realtime sync
- improve user data structure
- scalable collections

==================================================
VISUAL DESIGN & ANIMATION UPGRADE
==================================================

J. Make the entire app visually premium, colorful, modern, and highly animated WITHOUT changing:
- auth flow
- game logic
- gameplay mechanics
- app navigation flow
- existing icons
- existing core functionality

The goal is to transform the app visually into a polished Play Store quality game while preserving the current system architecture and user experience.

Requirements:

1. VISUAL STYLE
- Improve overall UI aesthetics
- Add modern colorful gradients
- Use vibrant but professional gaming colors
- Improve spacing, shadows, glow effects, borders, cards, and containers
- Make UI feel premium and smooth
- Maintain readability and accessibility

2. ANIMATIONS
Add smooth animations throughout the app:
- page transitions
- button tap animations
- popup animations
- score increment animations
- coin collection animations
- floating effects
- glowing effects
- scale/fade transitions
- reward animations
- level unlock animations
- leaderboard entry animations
- loading animations

Animations must:
- be smooth and optimized
- not reduce FPS
- not affect gameplay performance
- work properly on low-end Android devices

3. GAME FEEL IMPROVEMENTS
Add premium game feel effects:
- subtle screen shake
- particle effects
- smooth block placement feedback
- combo animations
- satisfying destruction effects
- smooth UI transitions
- animated progress bars
- animated buttons

4. HOME SCREEN & LEVELS PAGE
Enhance:
- level cards
- buttons
- progress indicators
- coin display
- leaderboard section
- store UI
- profile section

Add:
- glowing borders
- animated gradients
- hover/tap feedback
- animated cards
- premium shadows

5. COLOR SYSTEM
Create a proper color palette system:
- primary colors
- secondary colors
- gradients
- background colors
- success/error/warning colors

Maintain consistency across entire app.

6. PERFORMANCE REQUIREMENTS
- Keep app lightweight
- Avoid unnecessary widget rebuilds
- Optimize animations
- Use const widgets wherever possible
- Maintain smooth gameplay performance
- Ensure no animation lag during gameplay

7. RESPONSIVE DESIGN
Ensure all UI improvements work properly on:
- small Android devices
- tablets
- tall screens
- different aspect ratios

8. DO NOT CHANGE
STRICTLY DO NOT MODIFY:
- authentication flow
- Firebase auth system
- game core mechanics
- existing app navigation flow
- app structure logic
- existing icons
- ad logic flow unless optimization needed

Only enhance visuals, polish, UX, and animations.

9. OUTPUT REQUIREMENTS
- Update files fully
- Mention file paths clearly
- Keep code clean and production-ready
- Use reusable widgets
- Use scalable theme system
- Maintain Flutter best practices

==================================================
OUTPUT FORMAT
==================================================

For every improvement:
1. Explain issue found
2. Explain why it is bad
3. Provide improved architecture
4. Update code files fully
5. Mention file paths
6. Keep app runnable

Do not break existing gameplay.

Act like a professional mobile game studio engineer.
