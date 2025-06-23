# Grand Strategy Simulator: Total War - Iran vs. Israel

**Author:** [Blindsinner](https://github.com/Blindsinner)

## 1. Introduction

This project is a detailed, turn-based grand strategy wargame simulating a modern conflict between Iran and Israel. It is designed to be a realistic simulation focusing on resource management, strategic military operations, diplomatic maneuvering, and asymmetric warfare. The game is built as a single, self-contained HTML file that runs directly in your browser.

## 2. Core Features

This simulation includes a rich set of features to provide a deep strategic experience:

* **Faction Selection:** Choose to play as **Israel** or **Iran**, each with unique units and strategic options. A **Spectator Mode** is also available to watch the AI battle itself.
* **Turn-Based Gameplay:** The conflict unfolds day-by-day. Each turn, you will manage your budget, produce units, and command your forces on the strategic map.
* **Dynamic Scenario Setup:**
    * **Factual Historical Baseline:** The game loads a 100% factual timeline of real-world events as a starting point.
    * **User-Updated Timeline:** A unique "Latest Intel" system prompts you at the start of each game. You can use an AI to generate events for the time gap between the last known historical fact and the present day, making the start of every campaign unique.
* **Command & Control Center:** A central hub to manage your faction with multiple tabs:
    * **Sit-Rep:** Get a full overview of your budget, national morale, logistics, and a dynamic threat assessment.
    * **Operations:** View a detailed roster of all your military units and their current status.
    * **Production:** Queue up new military units at your various production facilities.
* **Deep Strategic Arsenal:** Go beyond conventional warfare and authorize powerful special operations:
    * **Ballistic Missile Strikes:** Launch powerful conventional missiles at key enemy locations.
    * **SEAD Missions:** Execute "Suppression of Enemy Air Defenses" strikes to disable units like the Iron Dome or S-300 systems.
    * **Nuclear Facility Strikes:** A high-risk, high-reward option to target strategic nuclear sites, causing massive economic damage at a high political cost.
    * **Major Cyber Attacks:** Cripple the enemy's command and control by targeting their capital.
    * **Mass Proxy Mobilization (Iran Only):** Unleash coordinated proxy attacks across multiple border nodes.
* **Research & Development (R&D):**
    * Invest in long-term projects to gain a decisive edge.
    * Develop a **Nuclear Weapons Program** to unlock the ultimate strategic option.
    * Create an **EMP (Electromagnetic Pulse) Weapon** to paralyze enemy electronic systems.
* **Diplomacy & Allied Support:**
    * Open diplomatic channels with your primary superpower ally (**USA** for Israel, **Russia** for Iran).
    * Request emergency financial aid, advanced military hardware (F-22 Raptors or Su-57 Felons), or crucial intelligence to reveal hidden enemy units.
* **Developer Console:**
    * A hidden "cheat" console is accessible via the famous **Konami Code** (`↑ ↑ ↓ ↓ ← → ← → B A`) for testing, debugging, or creative scenarios.

## 3. Setup and Installation

This game is designed for simplicity. No complex setup is required.

1.  Download the `index.html` (or the name you've given the file).
2.  Open the file in a modern web browser like Chrome, Firefox, or Edge. The game will run locally.

### Configuration: Adding Your API Key

The "Intelligence" and "AI Strategic Counsel" features in the Command Center require a **Google Gemini API key** to function.

1.  **Get a Key:** Obtain a free API key from [Google AI Studio](https://aistudio.google.com/apikey).
2.  **Edit the File:** Open the HTML file in a text editor.
3.  **Find the Placeholder:** Scroll down to the `<script>` section and find the following line (around line 1259):
    ```javascript
    // --- Gemini API (For AI advice ONLY) ---
    const API_KEY = "YOUR_API_KEY_HERE"; // IMPORTANT: Replace with your actual Gemini API key
    ```
4.  **Replace the Key:** Replace the text `"YOUR_API_KEY_HERE"` with the actual key you generated from Google. Save the file.

## 4. How to Play

### Starting a Game
1.  When the game loads, you will be presented with the factual history of the conflict.
2.  Next, the **"Update Timeline"** window will appear. You can either:
    * **Skip:** Click "Skip & Start Game" to begin immediately after the last known factual event (October 26, 2024).
    * **Update:** Copy the provided prompt. Paste it into an AI (like Gemini), and then paste the resulting JSON data back into the text box and click "Load Intel". This will add new events to the log and set the start date to the latest event in your data.
3.  Click **"Begin Future Simulation"** to start Turn 1.

### Gameplay
* **Selecting Units/Nodes:** Click on a unit or a map node to see its information in the right-hand panel.
* **Issuing Orders:** When a friendly unit is selected, the bottom-right panel will show available `Move` and `Attack` options.
* **Managing Your Faction:** Use the **Command Center** and **Diplomacy** buttons to access high-level strategic actions.
* **Ending Your Turn:** Once you have completed all your actions, click the **"End Turn"** button to allow the AI opponent to play its turn.

---
*This game was developed by [Blindsinner](https://github.com/Blindsinner).*
