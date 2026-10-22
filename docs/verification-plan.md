# Verification and Evaluation Plan

## 1. Overview
This document specifies the strategy for verifying and evaluating the initial prototype of the mobile application for improving mathematical skills in children aged 4–5.

The plan covers three evaluation pillars:
1. **Functional & Technical Verification** (Unit, Integration, and UI testing).
2. **Usability Evaluation** (User experience testing with children and parents).
3. **Educational Baseline Comparison** (Comparing digital quest-based practice with traditional paper workbooks).

---

## 2. Testing Strategy & Technical Verification

### 2.1. Unit Testing
* **Target:** Core business logic and task generators.
* **Scope:**
  * Math answer validation algorithms (number recognition, counting, quantity matching).
  * Level unlocking logic (ensuring level $N+1$ unlocks only upon completing level $N$).
  * Score and star calculation logic.

### 2.2. Widget & UI Testing (Flutter)
* **Target:** User interface components.
* **Scope:**
  * Bottom-to-top learning map navigation.
  * Interactive answer choice buttons and touch hitboxes.
  * Guided numeral tracing gesture detection.

### 2.3. Manual & Device Testing
* **Target:** Platform stability and responsiveness.
* **Scope:** Testing on Android Emulators, iOS Simulators, and physical mobile devices.

---

## 3. Evaluation Metrics & Success Criteria

| Category | Metric | Baseline / Target Threshold | Measurement Method |
| :--- | :--- | :--- | :--- |
| **Functionality** | Task Accuracy Rate | 100% correct validation for all math task types | Automated Unit & Integration Tests |
| **Usability** | Task Completion Rate | $> 85\%$ of children complete a 5-task quest level without adult help | Usability observations with focus group |
| **Engagement** | Time on Task | $3–5$ minutes per learning session (avoids screen fatigue) | Session logging |
| **Performance** | Application UI FPS | Stable $\ge 50–60$ FPS during quest animations | Flutter Performance Profiler |
| **Reliability** | Crash-free Session Rate | $100\%$ during standard 15-minute testing sessions | Error logging / manual testing |

---

## 4. Baseline Solution for Comparison

To assess the effectiveness and design value of the prototype, it will be evaluated against a **Baseline Solution**:

* **Baseline Definition:** Traditional printed paper activity workbooks and physical flashcards for children aged 4–5.
* **Comparison Parameters:**
  1. **Immediate Feedback:** Digital app provides instant audio-visual guidance upon an error, whereas paper workbooks require adult grading.
  2. **Interactivity:** Finger-tracing on glass provides direct tactile feedback and guided outlines compared to freehand pencil attempts.
  3. **Engagement:** Gamified mountain descent quest vs. static paper exercises.

---

## 5. Conditions and Evaluation Process
1. **Target Participants:** 3–5 children aged 4–5 accompanied by parents/educators.
2. **Environment:** Quiet, low-distraction setting using a tablet or smartphone.
3. **Procedure:**
   * Step 1: Pre-test orientation (child is introduced to the guide character).
   * Step 2: Unassisted interaction (child attempts 1–2 levels on the learning map).
   * Step 3: Observation of difficulties (recording UI bottlenecks or confusion).
   * Step 4: Parent post-session questionnaire.