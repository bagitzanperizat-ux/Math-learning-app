# Math Learning App (Ages 4–9)

> **Project Proposal & Interactive Prototype**  
> An adaptive, highly autonomous gamified mobile application designed to improve foundational mathematical skills in young children through an intuitive vertical Quest Map and sub-level task mechanics.

---

##  Executive Summary & Scope

Traditional math learning applications are often overloaded with intrusive ads, complex text-heavy UI, or basic static test banks. This project addresses the challenge of early childhood mathematical education by providing a **child-autonomous, gamified mobile environment** where young learners can navigate and solve problems without requiring adult supervision.

* **Target Audience:** Children aged 4–9 (primary focus on early learners aged 4–5).
* **Core Mascot:** **Leon** (an animated character in a signature green hoodie/zip-up).
* **Key Visual Mechanic (Top-to-Bottom Quest Map):**
  * **Vertical Flow:** The user journey begins at the top position with Leon and progresses downward to the final **Finish Node (`🏁`)**.
  * **Multi-Wall Sub-Level System:** Each node on the map represents a comprehensive level containing 5 internal task "walls" (🧱). Users must solve all 5 tasks sequentially to break the internal walls, mark the level as completed (`✓`), and unlock the downward path to the next node.
  * **Onboarding Age Selection:** Interactive age pre-selection starting from **4 years old**, dynamically adjusting UI complexity and task difficulty.

---

##  Architecture & Technology Stack

The project separates the rapid interactive UX validation phase from the production-ready mobile implementation:

| Layer | Technology | Rationale & Description |
| :--- | :--- | :--- |
| **Production Mobile Stack** | **Flutter** | Cross-platform framework providing native 60fps rendering and declarative UI for iOS and Android. |
| **State Management** | **BLoC (Flutter BLoC)** | Ensures strict separation of business logic, state handling, and UI components for high scalability and testability. |
| **Local Database / Storage** | **Hive** | Fast, lightweight NoSQL key-value database for local offline progress tracking, star metrics, and state persistence. |
| **Prototyping & UX Validation** | **HTML5 & Tailwind CSS** | Standalone interactive web prototype built for immediate visual pre-defense, screenshot capture, and UX flow testing prior to full Flutter compilation. |

---

##  Repository Structure

```text
math-learning-app/
├── prototypes/
│   └── index.html               # Interactive HTML/Tailwind prototype (Quest Map & Wall mechanic)
├── docs/
│   ├── screenshots/             # UI screenshots for presentation and project proposal defense
│   └── architecture.md          # Flutter + BLoC + Hive architectural details
├── mobile/                      # Production Flutter Application
│   ├── lib/
│   │   ├── logic/               # BLoC state management
│   │   ├── models/              # Data models (Hive adaptors)
│   │   └── presentation/        # Flutter UI widgets & screens
│   └── pubspec.yaml
└── README.md                    # Project documentation