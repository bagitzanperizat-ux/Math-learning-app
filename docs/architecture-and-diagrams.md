# Architecture and Diagrams Specification

## 1. Overview
This document describes the architectural design of the mobile application for early childhood mathematics learning. The system uses a clean, layered architecture implemented in Flutter.

---

## 2. System Architecture Layers

1. **Presentation Layer (UI & Widgets):**
   * Home Screen & Bottom-to-Top Quest Map.
   * Task Screens (Number Recognition, Object Counting, Quantity Matching, Finger Tracing).
   * Character Guidance & Reward Modals.
2. **Business Logic Layer (BLoC / Cubit):**
   * `QuestBloc`: Manages map state, level locking/unlocking, and progression.
   * `MathTaskBloc`: Handles task generation, user input submission, and answer validation.
   * `TracingCubit`: Tracks finger coordinates during touchscreen numeral tracing.
3. **Data Layer (Repositories & Local Storage):**
   * `ProfileRepository`: Reads and writes user preferences and age settings.
   * `ProgressRepository`: Persists level completion and star ratings in **Hive/Isar** storage.

---

## 3. Required Diagrams

The detailed diagram assets are located in the `/diagrams` folder:

### 3.1. System Context Diagram (`/diagrams/system-context.png`)
* **Purpose:** Defines the boundaries of the application and its environment.
* **Actors & Systems:**
  * **Child User:** Interacts directly with the touch screen.
  * **Parent User:** Configures basic profile settings.
  * **Mobile App (System):** Runs offline on the local device.
  * **Local Storage (Hive DB):** Saves persistent progress locally.

### 3.2. Use Case Diagram (`/diagrams/use-case.png`)
* **Main Use Cases:**
  * Select Age Group / Profile.
  * View Bottom-to-Top Quest Map.
  * Play Level (5 tasks per level).
  * Perform Number Recognition Task.
  * Perform Object Counting Task.
  * Perform Quantity Matching Task.
  * Practice Guided Numeral Tracing.
  * Receive Immediate Character Feedback & Stars.

### 3.3. Component Diagram (Draft) (`/diagrams/component-diagram.png`)
* **Components:**
  * `UI Modules` (Map, Exercise Engine, Tracing Canvas).
  * `State Management` (Quest BLoC, Task BLoC).
  * `Domain Services` (Math Task Generator, Tracing Evaluator).
  * `Data Storage` (Hive Progress Storage, Assets Provider).

---

## 4. Mermaid Code Sources

For editing or regenerating the diagrams, you can use the following Mermaid source codes:

### System Context (Mermaid)
```mermaid
graph TD
    User[Child User 4-5 y.o.] -->|Touch Input / Gestures| App[Math Learning App - Flutter]
    Parent[Parent / Educator] -->|Initial Setup| App
    App -->|Read / Write Progress| DB[(Local Hive NoSQL DB)]
    App -->|Load Visual & Audio Assets| Assets[Local Assets Package]