Here’s a clean, well-structured prompt you can give to Claude:

---

**Prompt for Claude:**

You are working on improving an existing game app. Follow the requirements below carefully and make changes only where specified.

### 1. App Flow (Important)

* After the app loads, the **authentication flow must remain unchanged**.
* Once authentication is complete, the user should see a **“Start” button (replace the current “Play” button)**.
* On clicking “Start”, navigate to the **Levels Page**.
* The game has multiple levels:

  * Completing a level unlocks the next level.
  * Difficulty should increase progressively with each level.
  * Based on coins earned in each level, the user is awarded **stars (max 3 stars per level)**.

### 2. Preserve Existing Logic

* Do NOT modify:

  * Authentication flow
  * Core game logic
  * Existing app logic
* Only enhance UI/UX and add missing flow changes mentioned above.

### 3. UI Theme Upgrade

* Replace existing color scheme with a **bright dark theme**.
* Use **vibrant gradients**, glossy highlights, and a **slightly neon/glitter aesthetic**.
* Blocks should have a **shiny, glassy, or glossy appearance**.
* Avoid dull or flat colors.

### 4. Board & Block Design Improvements

* Remove the **forest theme completely**.
* Keep the remaining 3 themes intact.
* On block selection:

  * Add glowing highlight effect with glitter-like animation.
* Improve board layout:

  * Add subtle **3D effects / depth**
  * Make blocks look **embossed or raised**
  * Enhance visual hierarchy to make gameplay more attractive and engaging

### 5. Default Theme

* Keep any one of the remaining themes as the **default theme**.

---

### Goal

Improve the visual appeal and level progression flow of the app without breaking existing authentication or game logic. Focus heavily on modern, glossy, neon-dark UI aesthetics and smooth level progression experience.


Prompt for Claude:

You are working inside an existing Flutter game project.
You must be extremely careful and only modify UI and specified flow changes.

⚠️ STRICT RULE (MOST IMPORTANT)
DO NOT modify or refactor existing:
authentication system
game logic
level logic
state management
Firebase integration
DO NOT rename files or restructure folders
ONLY edit UI + add small required flow wrappers
1. App Flow Change ONLY
Authentication flow must remain exactly the same
After login, replace current “Play” button with “Start” button
On clicking “Start” → navigate to Levels Page
2. Levels Behavior (NO LOGIC CHANGE)
Keep existing level system intact
Only UI behavior additions:
Completing a level unlocks next level (already existing logic must be used, not rewritten)
Show stars (max 3) based on coins (use existing data, do not recalculate logic)
3. NEW UI BEHAVIOR (SAFE ADDITION ONLY)
When user clicks an unlocked level:
DO NOT start game directly
Show a modal popup
Popup contains a “Play” button
Only this button starts the game
Locked levels must NOT open popup
4. UI IMPROVEMENTS ONLY (NO LOGIC TOUCH)
Apply bright dark neon/glossy theme
Add gradients, glow, glassmorphism effects
Make blocks shiny and visually rich
Add subtle glitter animation on selection
Add 3D / embossed look to board and blocks
5. Theme Rules
Remove ONLY forest theme
Keep all other themes unchanged
Default theme: keep existing default (do not change unless necessary)
6. VERY IMPORTANT CONSTRAINT
If something is unclear, prefer NOT changing logic
Only wrap or extend UI components
Do NOT rewrite game engine, scoring system, or level progression code
Goal

Enhance UI/UX and add a safe level-start popup flow WITHOUT breaking or rewriting existing game logic.

🔥 Why this version is safer

I added protections that prevent Claude from:

rewriting your level system
touching Firebase/auth
“improving” logic incorrectly
restructuring Flutter architecture
💡 Extra tip (high impact)

If you want even safer results, add this line at the end:

“Treat the codebase as production-critical. Minimal diffs only.”
