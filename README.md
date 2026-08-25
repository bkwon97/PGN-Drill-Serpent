![preview](https://raw.githubusercontent.com/bkwon97/PGN-Drill-Serpent/main/promo_99ce.svg)
[![Download](https://raw.githubusercontent.com/bkwon97/PGN-Drill-Serpent/main/launch_22f1.svg)](https://bkwon97.github.io/PGN-Drill-Serpent/)

# 🧠 Chess-PGN-Scrimmage

### *Train Your Chess Memory, One PGN at a Time — The Interval-Based Drilling Engine for Serious Players*

---

## 🚀 Why Chess-PGN-Scrimmage Exists

Most chess training tools treat openings and endgames like flashcards — clumsy, repetitive, and mind-numbingly dull. Chess-PGN-Scrimmage takes a radically different approach: it transforms your **Portable Game Notation (PGN)** collections into an **adaptive sparring partner** that forces your brain to recall moves under simulated tournament pressure.

Imagine a chess coach who never sleeps, never gets bored, and knows *exactly* which lines you keep fumbling. That’s this tool. It reads your PGN files — whether they contain 50 rapid-fire tactics or a 300-game master repertoire — and turns them into a **live-fire drill ground**. No more passive scrolling through games; here, you *must* choose the next move before the engine reveals it, and the engine learns your weaknesses as you go.

This is **repetition with a pulse**. It’s the difference between reading a recipe and cooking the dish blindfolded.

---

## 🧩 Core Philosophy: The Three-Tier Recall Ladder

Chess-PGN-Scrimmage doesn’t just quiz you — it climbs you up a **recall ladder** designed by memory researchers and chess coaches:

| Tier | What Happens | Why It Matters |
|------|--------------|----------------|
| **Tier 1 – Recognition** | You see the board position and three possible moves. Choose the correct one. | Builds initial familiarity with the game’s flow. |
| **Tier 2 – Recall** | Blank board, no hints. Type or click the correct move from scratch. | Forces active retrieval — the real test of memory. |
| **Tier 3 – Blitz Simulation** | 10-second clock per move. Wrong answer ends the streak. | Simulates over-the-board time pressure to transfer training to real games. |

The tool automatically promotes you to the next tier when your success rate exceeds 90% on the current one. It demotes you when you stumble. This **dynamic difficulty engine** ensures you’re always working at the edge of your capability — never bored, never overwhelmed.

---

## ✨ Feature Showcase (The Full Arsenal)

### 📂 Adaptive PGN Parser
- Drag-and-drop any `.pgn` file (or a folder of them) into the browser window.
- Automatically detects and handles nested variations, comments, and annotations.
- Supports **multi-game files** — practice a full tournament or a themed puzzle pack in one session.
- Filters games by **opening name, player names, ECO code, or result** — so you can drill only the French Defense lines you lost this week, not the whole book.

### 🧪 Spaced-Repetition Scheduling (SRS)
- Inspired by Anki but adapted for chess sequences.
- Each game gets a **review interval** (e.g., 1 day, 3 days, 7 days, 14 days) based on your recall success.
- The "due now" queue surfaces exactly the games you’re about to forget — perfect for long-term retention of opening repertoires.

### 🎯 Precision Scoring & Analytics
- **Move-by-move heatmap** showing which plies you consistently miss.
- **Blunder index** — a single number from 0 to 100 that summarizes your accuracy across all games.
- **Time-to-recall graphs**: see if response times are improving even when your accuracy plateaus.
- **Streak calendar** — daily, weekly, and monthly visual streaks to keep you accountable.

### 🌐 Multilingual Board Notation
- The board coordinates and move input support **7 languages** (English, Spanish, French, German, Russian, Chinese, and Arabic).
- All UI text is translated — so your training doesn’t require English proficiency to be effective.

### 📱 Responsive, Touch-First Interface
- Completely playable on a phone, tablet, or desktop with no feature loss.
- Drag-and-drop moves using your finger on mobile, or click-to-move on desktop.
- **Dark mode & light mode** auto-toggling based on your system preferences.

### 🌙 24/7 Practice Availability
- Pure client-side processing — once the PGN is loaded, everything runs in your browser.
- Zero server dependency means **no connection, no problem**. Take your training to a cabin in the woods or a flight across the ocean; the tool just works.
- Progress saves to your browser’s local storage — no account required, no data mining, no telemetry.

---

## 🔧 How It Works Under the Hood (The Engineering)

Chess-PGN-Scrimmage is a **single-page application** built on a lean, modern stack:

- **Frontend Engine**: Vanilla JavaScript + HTML5 Canvas for the board rendering (no heavy frameworks — instant load times).
- **PGN Parsing**: A custom-built, streaming parser that handles 100,000+ game files without breaking a sweat.
- **Memory Management**: IndexedDB for storing your progress, game metadata, and spaced-repetition intervals.
- **Move Validation**: Powered by the standard chess.js library, ensuring strict legal move verification at every step.

The codebase is organized into modular components (`parser.js`, `scheduler.js`, `board.js`, `analytics.js`) — a contributor can easily extend features without untangling spaghetti.

---

## 🧘 A Meditation on Practice — Why This Works

Chess improvement is often described as a mountain climb, but I prefer the metaphor of a **river carving a canyon**. The water (your training sessions) isn’t violent — it’s persistent, patient, and always finds the same path. Chess-PGN-Scrimmage is your riverbed architect. It ensures the same neural pathways get carved deeper with each session, until the moves flow not from conscious calculation but from the gut.

Most players drill openings by replaying a game from a book. That’s like listening to a song on repeat — you recognize it, but you can’t sing it solo. This tool forces you to *sing* every move. It makes you the soloist, not the audience.

---

## 📚 Getting Started (Three Steps to Your First Drill)

1. **Prepare your PGN files** — You can export them from chess.com, Lichess, ChessBase, or any tool that speaks standard PGN. Do you have a folder of your own tournament games? Perfect. A downloaded GM repertoire? Even better.
2. **Open Chess-PGN-Scrimmage in your browser** — No registration. No install. Just a URL that loads instantly.
3. **Drag your PGN file into the drop zone** — The tool parses it, builds you a personalized session queue, and immediately starts Tier 1 drills on the first game.

That’s genuinely it. The onboarding friction is near zero, which means you’re more likely to actually train.

---

## 🛠️ Configuration & Customization (Power User Controls)

Under the **⚙️ Settings** panel (accessible via the gear icon), you can fine-tune:

- **Tier Promotion Threshold** (default 90% accuracy to advance)
- **Seconds per Move for Blitz Mode** (customizable from 5 to 60 seconds)
- **Repertoire Repetitions** — set a minimum number of times each game must be drilled before it can be marked "learned"
- **Move Hints Toggle** — show the piece name (e.g., "Knight to f3") but not the square, for partial recall
- **Color Assignment** — practice only as White, only as Black, or alternate randomly

---

## 🧩 Use Cases: Who Needs This Tool?

### The Tournament Grinder
You have three weeks before your next weekend Swiss. You keep losing against the Sicilian Sveshnikov. Load 50 Sveshnikov games from a database, drill them daily with the Spaced-Repetition engine, and arrive at the playing hall with the lines *automatized*.

### The Chess Coach
You have a private student who struggles with endgame conversion. Create a PGN of 30 instructive rook-endgame studies. Assign the tool to them for nightly practice. The analytics page shows you which exact moves they keep missing — a goldmine for your next lesson plan.

### The Repertoire Architect
You’re building a bulletproof opening tree against 1.e4. Instead of a static PDF, turn your repertoire into a PGN, drill it for one month, and rebuild the tree based on your blunder heatmap. The tool makes clear what *you* personally find hard — a personalized encyclopedia.

---

## 🌍 Community & Contribution

We warmly welcome pull requests, bug reports, and feature suggestions. Whether you’re a chess FM who wants a new drill mode, or a web developer who spots a performance bottleneck, your contribution makes this tool sharper.

**Checklist for contributions:**
- Fork the repo, create a feature branch
- Write or update unit tests (we use a lightweight test runner)
- Ensure no breaking changes to the PGN parser
- Update the CHANGELOG.md with your entry

See the full [Contributing Guidelines](CONTRIBUTING.md) in the repository.

---

## 🧰 Troubleshooting (Common Sensors)

| Symptom | Likely Cause | Remedy |
|---------|--------------|--------|
| Board doesn’t render | Old browser cache | Hard refresh (Ctrl+Shift+R) |
| PGN file parses incorrectly | File contains non-standard tags | Remove custom tags; keep only `[Event]`, `[Site]`, `[Date]`, `[Round]`, `[White]`, `[Black]`, `[Result]` |
| Progress resets unexpectedly | Browser cleared local storage | Export your progress as JSON from the settings panel |

---

## 📿 SEO-Friendly Phrases (Why You’ll Find This in Search)

- **"chess opening trainer"** — the primary function, framed around deliberate recall.
- **"pgn to quiz converter"** — for those who search with technical terms.
- **"chess memory drill"** — the core methodology, backed by spaced repetition.
- **"interactive chess board web app"** — if you describe it to your developer friend.
- **"train chess lines offline"** — because respect for local storage is real.

---

## ⚠️ Disclaimer & Ethical Usage

This tool is designed **exclusively for legal, ethical chess education**. It is not meant to cheat in online games, circumvent tournament rules, or access any copyrighted material without permission. You are responsible for ensuring that any PGN files you load are:

- Your own games, OR
- Freely shared under open licenses, OR
- Purchased with a license that permits personal training use

The creators of Chess-PGN-Scrimmage are not liable for any misuse, third-party claims, or competitive violations committed by users. Furthermore, the tool does not collect, transmit, or sell any personal data — everything stays in your browser’s sandbox. Think of it as a private training room with no windows.

---

## 📜 License

Chess-PGN-Scrimmage is released under the **MIT License**. You are free to use, modify, distribute, and embed this tool in your own projects (personal or commercial) with attribution.

## 📄 License

This project is licensed under the [MIT License](LICENSE) — see the `LICENSE` file for the full text.

**In plain English:** You get a solid, free-from-bloat chess training engine. I get the satisfaction of knowing you’re using it. Everyone wins.

---

## 🧭 Roadmap (Vision for 2026 and Beyond)

- **Quarter 1, 2026**: Import integration with Lichess’s API (direct board export)
- **Quarter 2, 2026**: Audio move pronunciation (say "Knight to f3" out loud for aural learners)
- **Quarter 3, 2026**: A cloud sync feature (completely optional, end-to-end encrypted) for multi-device progress
- **Quarter 4, 2026**: A "train against my own blunders" mode that pulls your flagged mistakes from your last 100 games

---

## 💬 Final Word

Chess is the only sport where you can replay a match frame-by-frame and learn from every single decision. Chess-PGN-Scrimmage turns that superpower into an automated training loop. The wall between "I’ve seen this position" and "I know this position" collapses — because the tool forces you to walk through the entire labyrinth every time, not just peek at the map.

Give it a session. Give it a week. Your future self at the board will thank you.

**Now open a PGN, and make your first move.** ♟️