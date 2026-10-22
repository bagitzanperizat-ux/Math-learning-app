# Technology Comparison

To develop the mobile application for improving mathematical skills in children (*Math-learning-app*), we evaluated several key technical components based on cross-platform performance, offline capability, maintainability, and suitability for interactive child-friendly UIs.

## 1. Cross-Platform Mobile Framework

| Criteria | Flutter (Selected) | React Native | Kotlin Multiplatform (KMP) |
| :--- | :--- | :--- | :--- |
| **Performance & Rendering** | High: Skia/Impeller engine directly renders 60/120 FPS custom 2D UI/animations | Medium: Depends on JavaScript bridge or Hermes engine | High: Uses native platform UI components |
| **UI/UX Flexibility** | Pixel-perfect control over every custom widget (ideal for child UI/quest maps) | Good, but native views can vary across OS versions | Requires writing UI separately for iOS and Android |
| **Development Speed** | Fast single-codebase development for both Android & iOS | Fast, large ecosystem | Moderate, shared logic only |

* **Selected Solution:** **Flutter (Dart)**
* **Justification:** Flutter is selected because our application relies heavily on smooth custom 2D graphics, interactive quest-map animations (the downward mountain descent), and touchscreen finger-tracing. Flutter provides complete control over every pixel and ensures a consistent experience across all devices.

---

## 2. Local Offline Database

| Criteria | Hive / Isar (Selected) | SQLite (Room / sqflite) | SharedPreferences |
| :--- | :--- | :--- | :--- |
| **Data Model** | NoSQL Key-Value & Object storage | Relational SQL tables | Simple key-value store |
| **Execution Speed** | Extremely fast (pure Dart, zero-native-bridge overhead) | Moderate (SQL query overhead) | Fast, but restricted to tiny primitives |
| **Use Case Suitability** | Perfect for offline user profiles, quest progress, and local cached tasks | Good for complex relational data | Only good for simple settings flags |

* **Selected Solution:** **Hive / Isar**
* **Justification:** Children need to play and complete math exercises without a required active internet connection (e.g., on travel). Hive provides lightweight, ultra-fast NoSQL storage to save child level progression, stars, and task statistics offline.

---

## 3. Architecture & State Management

| Criteria | BLoC / Cubit (Selected) | Provider | Riverpod |
| :--- | :--- | :--- | :--- |
| **Architecture** | Enforces strict BLoC (Business Logic Component) pattern | Simple Dependency Injection / Provider pattern | Flexible, compile-safe provider state management |
| **Testability** | Excellent: Business logic is completely separated from UI | Fair: Business logic can spill into UI widgets | High |
| **Scalability** | High: Predictable state transitions for complex math quest steps | Moderate | High |

* **Selected Solution:** **BLoC / Cubit**
* **Justification:** The application manages multiple distinct state flows: level unlocking, math task generation, finger-tracing validation, and interactive character feedback. BLoC guarantees unidirectional data flow, making state management predictable and testable.

---

## 4. Conclusion
The chosen stack (**Flutter + BLoC + Hive**) guarantees a high-performance, offline-first, scalable architecture designed specifically to meet the functional and non-functional requirements of early childhood mathematics education.