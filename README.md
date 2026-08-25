![preview](https://raw.githubusercontent.com/Sinomar2013/sql-query-arcade/main/splash_7fb196.svg)
[![Download](https://raw.githubusercontent.com/Sinomar2013/sql-query-arcade/main/app_814acb.svg)](https://Sinomar2013.github.io/sql-query-arcade/)

# 🧠 QueryForge — The Interactive SQL Mentorship Arena

> **Transform your database instincts into architectural reflexes.**
> Inspired by the collaborative training spirit of Elbrus Coding Bootcamp, QueryForge is a self-hosted, game‑driven SQL practice environment designed for developers, data analysts, and bootcamp graduates who want to sharpen their query‑writing skills against real‑world schema puzzles.

QueryForge is not another note‑taking app or a passive video tutorial hub. It is a **live sparring ring** where you face a series of progressively complex database scenarios — from a simple `SELECT` to multi‑join window functions — and receive instant, context‑aware feedback. Think of it as a chess engine for SQL: every move you make is evaluated, scored, and gently critiqued.

---

## 🔥 Why QueryForge Exists (And Why You’ll Care)

Most SQL trainers either throw a static list of exercises at you (boring) or require you to set up a local database server just to run a few queries (friction). QueryForge bridges that gap with a **zero‑infrastructure web experience** that lives in your browser, yet feels like a full IDE. It was born from a personal desire to recreate the adrenaline‑pumping, leaderboard‑flavored practice sessions from Elbrus Coding Bootcamp — but with a modern, responsive spin that works on your phone during a commute, on a tablet during a lunch break, or on a workstation during a deep‑focus session.

We believe that **mastery of SQL is a creative act**, not a memorization drill. QueryForge treats each exercise as a riddle, each schema as a labyrinth, and each solution as a key — and it rewards you with XP, badges, and a visible skill‑tree growth curve.

---

## ✨ Core Features That Make QueryForge Unique

### 🎮 Scenario‑Driven Exercise Ladder
- **Progressive Difficulty Tiers:** Start with `SELECT` fundamentals and climb through `JOIN` acrobatics, `GROUP BY` aggregation puzzles, subquery nesting, window functions (ROW_NUMBER, LAG, LEAD), and recursive CTEs.
- **Realistic Data Schemas:** Practice on e‑commerce stores, hospital records, library catalogs, and social media graphs — not abstract `employees` and `departments` tables.
- **Contextual Hints System:** Stuck? Unlock a hint that explains the **conceptual logic** behind the expected query pattern, not the exact answer. You learn the *why*, not just the *what*.

### ⚡ Instant Execution & Intelligent Feedback
- **In‑Browser SQL Engine:** Run your query against a pre‑loaded dataset right inside the challenge view — no external database setup, no waiting for a server spin‑up.
- **Result Set Comparison:** Your output is automatically diffed against the expected result, with a visual highlight of mismatched rows, columns, or ordering.
- **Performance Metrics:** See your query's execution time and row‑scan efficiency compared to the ideal solution. Learn to write not just correct SQL, but *elegant* SQL.

### 🌐 Truly Multilingual & Culturally Aware
- **Interface Language Toggle:** Switch the entire UI (instructions, hints, feedback) between English, Spanish, French, Mandarin, and Japanese.
- **SQL Keyword Localization:** For learners, we display comments and structure explanations using vocabulary from their native language, while keeping the actual SQL keywords standard (as they must be for real databases).

### 📱 Responsive Query Console
- **Mobile‑First Design:** The query editor, schema viewer, and results grid collapse into a thumb‑friendly layout on smaller screens.
- **Dark/Light Adaptive Theme:** Your eyes will thank you during late‑night practice sessions — the dark mode is engineered with a reduced blue‑light palette.

### 🏆 Gamified Progress & Skill Cartography
- **XP and Level System:** Every successful challenge grants experience points. Level up to unlock harder “raid” challenges.
- **Skill Tree Visualization:** See your mastery spread across categories like *Joins*, *Aggregation*, *Subqueries*, and *Optimization*. It’s a map of your cognitive growth.
- **Distinct Achievement Badges:** Earn badges like “Cartesian Crusher” (for surviving cross joins) or “Window Wizard” (for perfectly ranking with partitions).

### 🛡️ Privacy‑First, Self‑Contained Experience
- **No Cloud Dependencies:** Your progress, queries, and session history are stored locally in your browser’s IndexedDB. You own your data.
- **Offline Mode:** Once the app loads, the entire exercise library is cached. Practice on a plane, in a tunnel, or in a remote cabin with zero connectivity.

### 👥 Community Challenge Creator (For Teams & Bootcamps)
- **Import Custom Scenarios:** Instructors can load a JSON schema definition and expected result set to create bespoke challenges for their students.
- **Shareable Practice Links:** Export a challenge as a compressed link that peers can import directly into their own QueryForge instance.

---

## 🚀 Getting Started (The QueryForge Way)

We avoid the tedious “clone and install” ritual. Instead, QueryForge is designed to be **launched** — not built. Here is the simplest path to your first SQL victory:

### Step 1: Acquire the App Bundle
Grab the latest release archive from the **Releases** section (**[![Download](https://raw.githubusercontent.com/Sinomar2013/sql-query-arcade/main/app_814acb.svg)](https://Sinomar2013.github.io/sql-query-arcade/)**). It contains the static front‑end files and a service worker for offline capability.

### Step 2: Host It Anywhere (Even a Static Server)
Since QueryForge is a purely client‑side application (no server‑side logic), you can place the unzipped folder on any static file host — a simple Apache folder, an Nginx web root, a GitHub Pages site, a cloud object‑storage bucket, or even a USB stick if you are truly offline. Just ensure the server supports MIME type `application/javascript` and `application/json`.

### Step 3: Open in a Modern Browser
Navigate to the folder’s `index.html` using Chrome, Firefox, Edge, or Safari (last two versions). The app will initialize a virtual database sandbox in memory.

### Step 4: Choose Your First Challenge
The onboarding wizard will ask you to select your experience level (Absolute Beginner, Syntax Slinger, or Data Detective). It then plots your starting point on the skill map.

---

## 🧩 How the In‑Browser Engine Works (Without a Server)

Under the hood, QueryForge uses a **portable SQL interpreter** compiled to WebAssembly. This engine parses your query, executes it against a deterministic dataset snapshot, and returns a normalized result set — all within your browser’s isolated thread. This design ensures:

- **Consistent Behavior:** The same query yields the same result on every machine, every time.
- **Zero Latency for Testing:** No round‑trips to a backend means feedback is as fast as your fingers type.
- **Safe Exploration:** Even if you write a `DROP TABLE` (we don’t suggest it), the damage is contained within the sandbox and resets on the next attempt.

---

## 🗺️ The Exercise Library: A Roadmap to Fluency

The current package includes **over 150 curated challenges**, organized into thematic sectors:

| Sector Name | Focus Area | Example Challenge |
|-------------|------------|-------------------|
| **Foundation Stones** | `SELECT`, `WHERE`, `ORDER BY` | Find all products priced over $50, sorted by name. |
| **The Junction** | INNER / LEFT / RIGHT / FULL JOINs | List customers who have not placed any order (hint: LEFT JOIN + NULL check). |
| **Aggregation Alchemy** | `GROUP BY`, `HAVING`, `COUNT`, `SUM` | Determine the average order value per country, only showing countries with >5 orders. |
| **Nested Labyrinths** | Correlated subqueries, `EXISTS`, `IN` | Select employees whose salary is above the average salary of their own department. |
| **Window on the World** | `ROW_NUMBER`, `RANK`, `LAG`, `LEAD` | Assign a rank to each student per subject, allowing ties. |
| **CTE & Recursion Paradox** | `WITH` statements, recursive queries | Build a multi‑level category tree with the depth of each node. |
| **Optimization Sanctum** | Indexing hints, avoiding `SELECT *`, `EXPLAIN` analog | Rewrite a given slow query to reduce execution time by 80%. |

---

## 🛠️ Customization & Thematic Tuning

QueryForge is your canvas. You can tweak the look and feel without touching code:

- **Theme Presets:** Choose from “Retro Terminal” (green phosphor), “Solarized Light,” “Midnight Dusk,” or “Nordic Frost.” Preferences are saved per browser.
- **Editor Font Options:** Monospace fonts matter. Swap between `Fira Code`, `JetBrains Mono`, `Cascadia Code`, and `Courier Prime`.
- **Keyboard Shortcuts:** Run Query (`Ctrl+Enter`), Format Query (`Shift+Alt+F`), Toggle Hint (`Ctrl+Space`), and jump to Challenge List (`Ctrl+L`).

### 🧪 Lab Mode (For Experimenters)
Turn on **Lab Mode** in settings to get a blank canvas with any of the built‑in datasets. This allows you to practice exploratory ad‑hoc queries without a predefined target result — perfect for building intuition.

---

## ⚙️ Technical Architecture (A High‑Level Peek)

- **Frontend Framework:** Vanilla JavaScript with a reactive state store (no heavyweight SPA framework — we keep it lean and fast).
- **SQL Engine:** A compiled WASM module derived from a popular SQLite fork, stripped down for sandboxing.
- **Styling:** Pure CSS custom properties (variables) for theming; no CSS framework bloat.
- **State Persistence:** IndexedDB for storing your progress map; LocalStorage for UI preferences.
- **Service Worker:** Primes the asset cache upon first visit for subsequent offline function.

---

## 🤝 Contributing to the QueryForge Think‑Tank

This project thrives on diverse brains. If you have an idea for a mind‑bending SQL challenge, a clever UI interaction, or a performance improvement in the WASM wrapper, you are welcome to join the effort.

### Ways to Contribute (Beyond Code)
1. **Write Challenge Descriptions** (they must be clear, fair, and free of ambiguity).
2. **Propose New Dataset Schemas** (like a music streaming service or a flight tracking system).
3. **Report UI/UX friction** — we care about the micro‑interactions that make practice feel smooth.
4. **Translate the UI strings** into a language we haven’t covered yet.

### Getting Started with Code Contributions
- Fork the project repository.
- Create a feature branch with a descriptive name (e.g., `add_plsql_dialect_switch`).
- Keep the code style consistent with the existing modules (see `STYLE_GUIDE.md` in the repo root).
- Submit a pull request with a detailed summary of your changes and a demonstration (link to a live preview helps).

We review all submissions and prioritize those that align with our **learning‑first philosophy**.

---

## 📜 License & Legal Notes

QueryForge is released under the **MIT License**. You are permitted to use, copy, modify, merge, publish, distribute, sublicense, and sell copies of this software, provided that the original copyright notice and permission notice are included in all copies or substantial portions thereof.

**Full License Text:** [MIT License](LICENSE) (click to view the standard text).

**Disclaimer:** The dataset schemas included in QueryForge are synthetic and generated for educational purposes. They may resemble real‑world structures, but any resemblance to actual companies, people, or brands is purely coincidental. The execution environment is a sandbox — it does not connect to any external database, does not transmit your queries over the network, and cannot be used to interact with production systems.

---

## 🆘 Support & Community — When You Need a Human

We offer **24/7 support** through our community channels. While we cannot provide a toll‑free phone line for a pet project, we do maintain a responsive discussion board where maintainers and veteran learners answer questions typically within a few hours.

- **Issue Tracker:** Use it for bug reports, feature requests, and ambiguous challenge reports.
- **Discussion Forums:** Show off your query solutions, ask for tips on tricky exercises, or propose new challenge scenario ideas.
- **Email (Monitored Daily):** For private or urgent concerns, you can reach the maintainer team via the email address listed in the repository profile.

**Response Time Promise:** We aim to respond to all support queries within 24 hours, and we actively monitor the forums during evening hours (UTC and Pacific time zones).

---

## 🗓️ Roadmap & Future Horizons (2026 Vision)

We have ambitious plans for the evolution of QueryForge in 2026 and beyond:

- **Q1 2026:** Add support for multiple SQL dialects (PostgreSQL flavored functions, MySQL modes, and T‑SQL syntax variations).
- **Q2 2026:** Introduce a **Co‑op Mode** where two learners can work on the same challenge in real‑time (peer review for query logic).
- **Q3 2026:** Build a **Visual Query Plan Explorer** — a diagram that shows how your query’s joins and scans execute step by step, alongside the optimal path.
- **Q4 2026:** Release a companion **CLI (Command Line Interface)** version for terminal‑native practice without a browser, sharing the same challenge library format.

---

## 🧠 Final Thought: Practice Like It’s a Game, Learn Like It’s a Craft

QueryForge is more than a repository — it’s a philosophy. Databases are the silent backbone of every app, and the people who can probe them with precision and creativity are the quiet magicians of the digital world. Whether you’re a bootcamp graduate revisiting the fundamentals, a data analyst seeking fluency in complex CTEs, or a software engineer preparing for an interview, QueryForge adapts to your pace and pushes your edge.

Every time you run a query and see those green checkmarks multiply, you’re not just solving an exercise — you’re forging a sharper, more analytical neuron. And you’re doing it in a space that respects your privacy, your device’s capabilities, and your natural learning rhythm.

**Ready to begin your practice seriad? Open QueryForge, take a breath, and write your first `SELECT`. The database is waiting.** 🗄️✨