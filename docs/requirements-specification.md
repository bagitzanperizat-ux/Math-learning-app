# Requirements Specification
## Mobile Application for Improving Mathematical Skills in Children

### 1. Purpose

This document defines the initial functional and non-functional requirements for the proposed mobile application. It describes the expected behaviour of the application, the priority of each requirement, and the criteria used to verify its implementation.

The requirements are preliminary and may be updated during technical design, prototype development, and evaluation.

### 2. Project Scope

The initial prototype will focus on foundational mathematics activities for children aged 4–5. The application will combine interactive exercises with a story-based learning journey.

The proposed concept includes a friendly character, a visual learning map with levels arranged from bottom to top, sequential progression, and rewards for completing activities.

The initial prototype will prioritise four mathematical skills:

- Number recognition.
- Counting familiar objects.
- Matching quantities to numerals.
- Guided numeral tracing.

The application is planned using Flutter and Dart, subject to confirmation during technical design.

### 3. Functional Requirements

Priority definitions:

- **Must have:** Essential for the initial prototype.
- **Should have:** Important, but may be simplified if necessary.
- **Could have:** Optional for the initial prototype or suitable for future development.

#### FR-01. Learning Home Screen

**Priority:** Must have

**Description:** The application shall provide a home screen from which the child can start or continue the learning journey.

The interface should use simple navigation, clear visual elements, and age-appropriate illustrations.

**Acceptance criteria:**
- The home screen is displayed when the application launches.
- The child can identify the main action for starting or continuing learning.
- The learning map can be opened from the home screen.

**Verification:** Manual functional testing.

#### FR-02. Story-Based Learning Journey

**Priority:** Must have

**Description:** The application shall connect mathematical activities through a continuous story. A friendly character will accompany the child, introduce challenges, and react to progress.

The character, storyline, and visual design will be finalised during the design phase.

**Acceptance criteria:**
- Activities are presented as part of a connected learning journey.
- The character appears in relevant parts of the learning experience.
- Completing required activities allows the child to continue the journey.
- Story elements do not prevent access to mathematical exercises.

**Verification:** Scenario-based testing and interface review.

#### FR-03. Bottom-to-Top Learning Map

**Priority:** Must have

**Description:** The application shall display a visual learning map with levels arranged from bottom to top. The map will help children understand their position in the learning journey.

**Acceptance criteria:**
- Levels are displayed in a bottom-to-top arrangement.
- The current level is visually identifiable.
- Completed and locked levels have distinguishable visual states.
- The child can select an available level.
- Locked levels cannot be opened through normal navigation.

**Verification:** Manual navigation testing.

#### FR-04. Sequential Level Unlocking

**Priority:** Must have

**Description:** The application shall unlock levels according to a predefined sequence. The child must complete the required activities of the current level before accessing the next level.

**Acceptance criteria:**
- The first level is available at the beginning.
- The next level remains locked until the required activities are completed.
- Successful completion unlocks the next level.
- The displayed level status updates correctly.
- The child cannot skip locked levels through the standard interface.

**Verification:** Functional testing of level progression.

#### FR-05. Number Recognition

**Priority:** Must have

**Description:** The application shall provide interactive activities that help children recognise and distinguish written numerals.

For example, the child may see a numeral and select the matching answer from several options. Numerals will be introduced gradually.

**Acceptance criteria:**
- A numeral is clearly displayed.
- The activity provides selectable answer options.
- The application checks the selected answer.
- The child receives feedback after answering.
- The activity can be repeated for additional practice.

**Verification:** Testing with correct and incorrect answers.

#### FR-06. Counting Familiar Objects

**Priority:** Must have

**Description:** The application shall provide counting exercises using familiar visual objects, such as fruits, stars, toys, or animals.

The child will count the objects and select the corresponding quantity. The number of objects and task complexity will increase gradually.

**Acceptance criteria:**
- The activity displays a clearly distinguishable group of objects.
- The child can select an answer representing the quantity.
- The correct answer corresponds to the number of displayed objects.
- The application checks the selected answer and provides feedback.
- Different object groups can be used across activities.

**Verification:** Functional testing with predefined object groups.

#### FR-07. Matching Quantities to Numerals

**Priority:** Must have

**Description:** The application shall provide activities in which children match a written numeral to a group containing the corresponding number of objects.

For example, the child may be asked to select four stars when shown the numeral 4.

**Acceptance criteria:**
- The activity displays a numeral and visual groups of objects.
- Each group contains a distinguishable quantity.
- The child can select a group.
- The application checks whether the selected quantity matches the numeral.
- The child receives appropriate feedback.

**Verification:** Testing with multiple numeral and quantity combinations.

#### FR-08. Guided Numeral Tracing

**Priority:** Must have

**Description:** The application shall allow children to practise tracing numerals using a finger on a supported touchscreen. A visual outline will guide the child along the intended path.

The activity is intended to familiarise children with numeral shapes and provide basic writing practice.

**Acceptance criteria:**
- A numeral outline is clearly visible.
- The child can interact with the outline using a finger.
- The intended tracing path is visually indicated.
- The application provides feedback after the attempt.
- The tracing activity can be tested on the selected device.

**Verification:** Manual touchscreen testing.

#### FR-09. Immediate Feedback

**Priority:** Must have

**Description:** The application shall provide immediate, age-appropriate feedback after a child submits an answer.

Correct answers may trigger encouraging messages, animations, or character reactions. Incorrect answers should lead to supportive guidance or another attempt.

**Acceptance criteria:**
- Feedback appears after an answer is submitted.
- Correct answers receive positive feedback.
- Incorrect answers receive supportive guidance or an opportunity to retry.
- Feedback corresponds to the actual answer.
- The child can continue the activity after receiving feedback.

**Verification:** Functional testing with correct and incorrect responses.

#### FR-10. Rewards and Achievements

**Priority:** Should have

**Description:** The application should provide virtual rewards, such as stars or achievement indicators, for completing activities and levels.

Rewards should encourage participation without distracting from the educational purpose.

**Acceptance criteria:**
- A reward or completion indicator appears after a qualifying activity.
- The reward corresponds to the completed activity or level.
- Rewards are displayed consistently.
- The prototype does not require real-money purchases to obtain rewards.

**Verification:** Testing of activity completion and reward display.

#### FR-11. Gradual Difficulty Progression

**Priority:** Must have

**Description:** The application shall organise activities from simpler to more challenging tasks.

For example, the learning sequence may begin with number recognition, continue with counting and quantity matching, and then introduce numeral tracing. The exact sequence will be finalised during educational content design.

**Acceptance criteria:**
- The learning sequence is documented.
- Activities follow the defined sequence.
- Later tasks may introduce greater difficulty through larger quantities or additional answer options.
- Activities remain appropriate for the target age group.

**Verification:** Review of the learning sequence and scenario-based testing.

#### FR-12. Activity Retry and Replay

**Priority:** Should have

**Description:** The application should allow children to retry incorrect answers and repeat completed activities without restarting the entire learning journey.

**Acceptance criteria:**
- The child can retry an incorrect answer where the activity supports retries.
- Completed activities can be repeated through the available interface.
- Repeating an activity does not incorrectly reset the overall level status.

**Verification:** Functional testing of retry and replay scenarios.

#### FR-13. Visual Progress Indicators

**Priority:** Should have

**Description:** The application should indicate completed activities and levels through visual markers on the learning map.

Detailed statistics and a separate parent dashboard are not required for the initial prototype.

**Acceptance criteria:**
- Completed levels have a visible completion indicator.
- The current learning position can be identified.
- The displayed progress corresponds to the actual completion state.

**Verification:** Testing of progress indicators and level status.

#### FR-14. Application Language

**Priority:** Could have — pending team decision

**Description:** The team is considering Kazakh as the primary language of the application. This direction may help make the learning experience more accessible to children who are more comfortable learning in Kazakh.

The final language decision has not yet been confirmed.

**Acceptance criteria:**
- The initial prototype language is selected and documented before finalising the content.
- Instructions and feedback use consistent terminology.
- Text is reviewed for linguistic accuracy and suitability for young children.

**Verification:** Interface review and linguistic review.

### 4. Non-Functional Requirements

#### NFR-01. Usability

**Priority:** Must have

The interface shall be simple and understandable for children aged 4–5. Activities should rely on clear visuals and simple interactions rather than long written instructions.

**Acceptance criteria:**
- The main action on each learning screen is visually identifiable.
- Core activities can be completed using the intended touch interactions.
- Navigation is reviewed for age appropriateness.

**Verification:** Usability review.

#### NFR-02. Visual Clarity

**Priority:** Must have

Numerals, objects, buttons, and instructions shall be distinguishable from their backgrounds. Interactive elements should be sufficiently large and spaced to reduce accidental selections.

**Acceptance criteria:**
- Numerals and counting objects are clearly visible.
- Buttons and selectable answers are visually distinguishable.
- Text and visual instructions remain readable on the selected device.

**Verification:** Interface inspection.

#### NFR-03. Performance

**Priority:** Should have

The application should respond promptly to user interactions and display learning activities without disruptive delays on the selected test device.

**Acceptance criteria:**
- Selecting an answer produces a visible response without unnecessary delay.
- Navigation between screens works without repeated freezing.
- Performance is checked on the target device or emulator.

**Verification:** Manual performance testing.

#### NFR-04. Reliability

**Priority:** Must have

The application shall behave consistently during normal use and avoid critical failures during basic learning activities.

**Acceptance criteria:**
- Core activities can be completed without crashes during testing.
- Correct and incorrect answers produce the expected responses.
- Level completion states remain consistent during the tested session.

**Verification:** Repeated functional and stability testing.

#### NFR-05. Privacy and Child Safety

**Priority:** Must have

The initial prototype shall minimise the collection of personal information. Personal accounts, social interaction, and external communication are not required for the initial version.

**Acceptance criteria:**
- Core activities can be tested without creating a child's personal account.
- The prototype does not request unnecessary personal information.
- Any introduced data collection is documented and reviewed.

**Verification:** Review of application features and data handling.

#### NFR-06. Maintainability

**Priority:** Should have

The application should have an understandable structure that allows the team to modify learning activities, level content, and visual elements without redesigning the entire application.

**Acceptance criteria:**
- The source code has a documented structure.
- Related functionality is organised into understandable components or modules.
- The team can identify where to update activity content and level definitions.

**Verification:** Code review.

#### NFR-07. Platform Compatibility

**Priority:** Must have

The application is planned to use Flutter and Dart, subject to confirmation during technical design. The prototype must run on the platform selected for evaluation.

**Acceptance criteria:**
- The development environment and target platform are documented.
- The prototype launches on the selected device or supported emulator.
- Core learning activities can be tested in that environment.

**Verification:** Build and execution testing.

### 5. MVP Acceptance Criteria

The initial prototype will be ready for internal evaluation when:

1. The child can open the application and access the learning map.
2. Levels are arranged from bottom to top.
3. The first level provides access to the core mathematical activities.
4. Number recognition works as intended.
5. Counting activities display correct object quantities.
6. Quantity-to-numeral matching works as intended.
7. Guided numeral tracing can be attempted on a supported touchscreen.
8. Correct and incorrect answers trigger appropriate feedback.
9. Completing required activities updates the level status and unlocks the next level, once the progression mechanism is implemented.
10. The prototype runs on the selected platform without critical failures during basic testing.

These criteria describe the expected behaviour of the prototype and do not indicate that the features have already been implemented.

### 6. Requirement Priorities

| Priority | Requirements | Rationale |
|---|---|---|
| Must have | FR-01 to FR-09, FR-11, NFR-01, NFR-02, NFR-04, NFR-05, NFR-07 | Establish the core learning experience, mathematical activities, progression, and minimum quality requirements. |
| Should have | FR-10, FR-12, FR-13, NFR-03, NFR-06 | Improve motivation, practice opportunities, progress visibility, and maintainability. |
| Could have / pending decision | FR-14 and future extensions | Depends on the final language decision and project resources. |

Priorities are preliminary and should be reviewed by both team members before implementation.

### 7. Open Decisions and Assumptions

The following decisions remain open:

- **Application language:** Kazakh is under consideration but has not been confirmed.
- **Character and storyline:** The concept of a friendly character and connected story is proposed; the details remain undecided.
- **Numeral range:** The exact numbers included in the initial prototype will be selected during content design.
- **Level structure:** The bottom-to-top map is proposed, but the number of levels and activities per level remain to be determined.
- **Progress storage:** The team must decide whether progress is retained between sessions.
- **Target platform:** The device and platform for evaluation must be confirmed.
- **Future age groups:** Content for children aged 6–9 may be considered in later development but is outside the initial prototype scope.

### 8. Future Development

Possible future extensions include additional mathematical topics, learning worlds for older children, multilingual support, a parent dashboard, and more detailed learning progress analysis.

These features will be considered after the initial prototype has been developed and evaluated. They are not commitments for the first version.

### 9. Review and Validation

Both team members shall review the requirements to ensure that they are understandable, feasible, and consistent with the project scope.

Each mandatory requirement must have a defined acceptance criterion and a suitable verification method. Requirements may be updated following team discussions, technical design, and prototype evaluation. Changes should be documented in the project repository.

### 10. Conclusion

This specification defines the initial requirements for a story-based mobile mathematics application for children aged 4–5. The proposed learning experience combines a bottom-to-top progression map, a friendly character, sequential levels, mathematical activities, immediate feedback, and gradual difficulty progression.

The initial prototype focuses on number recognition, counting familiar objects, matching quantities to numerals, and guided numeral tracing. The application language and detailed storyline remain subject to team review.

The specification provides a basis for technical design, prototype development, and evaluation.
