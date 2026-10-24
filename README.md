# Math Learning App

**Development of a Mobile Application for Improving Mathematical Skills in Children**

## 1. Project Overview

Math Learning App is a proposed story-based educational mobile application designed to help children develop foundational mathematical skills through interactive exercises, visual learning activities, and gamification.

Children will follow a guide character through a learning journey, complete mathematical challenges, and progress through a visual quest map. The project aims to make mathematics more engaging through familiar objects, age-appropriate tasks, immediate feedback, and gradual progression.

The project is planned as a cross-platform mobile application using Flutter and Dart. An interactive HTML prototype is used to explore and demonstrate the proposed user experience.

## 2. Problem Statement

Children develop mathematical skills at different rates. Some children may need additional practice with recognising numbers, counting objects, understanding quantities, and forming written numerals.

Traditional exercises may not always provide interactive practice, immediate feedback, or an engaging learning experience. This project explores how a story-based mobile application can support foundational mathematics learning through short activities, visual guidance, and game-based progression.

The proposed design is informed by preliminary stakeholder discussions, a review of scientific literature, and a comparison of existing educational applications.

## 3. Project Aim and Objectives

### Aim

To design and prototype a mobile application that supports the development of mathematical skills in children aged 4–9 through interactive exercises and game-based learning.

### Objectives

- Investigate children's early mathematics learning needs.
- Review scientific literature on mathematics education and digital learning.
- Compare existing mathematics-learning applications.
- Define functional and non-functional requirements.
- Compare and justify the proposed technical solutions.
- Design the system architecture and user interface.
- Develop an initial prototype focused on children aged 4–5.
- Prepare a verification and evaluation plan for the prototype.

## 4. Target Users

The overall concept is intended for children aged 4–9, divided into three proposed age groups:

- **Ages 4–5:** Number recognition, counting familiar objects, matching quantities to numerals, and guided numeral tracing.
- **Ages 6–7:** Number composition and introductory addition and subtraction.
- **Ages 8–9:** More advanced arithmetic and age-appropriate mathematical problems.

The initial prototype focuses on children aged 4–5.

Parents and educators are secondary stakeholders who may provide feedback on the application's usability and educational relevance.

Kazakh-language support is being considered, but the final language configuration has not yet been confirmed.

## 5. Main Planned Features

The initial prototype is planned to include the following features:

- **Story-based learning:** A guide character accompanies children through the learning journey.
- **Quest map:** A visual map presents learning levels and progression.
- **Number recognition:** Children practise identifying written numerals.
- **Object counting:** Children count small groups of familiar objects.
- **Quantity matching:** Children match quantities of objects to the corresponding numerals.
- **Guided numeral tracing:** Children follow a visual numeral outline using touchscreen input.
- **Immediate feedback:** The application responds to children's answers.
- **Rewards and progression:** Visual indicators and rewards encourage children to continue through learning activities.

The final feature set will be refined during development and evaluation. The initial tracing concept focuses on following a visual guide rather than automatically recognising freely handwritten digits.

## 6. Project Scope

The overall concept covers a story-based mathematics-learning application for children aged 4–9.

The initial project scope includes:

- Research and requirements analysis.
- Literature review and stakeholder feedback.
- Comparison of existing applications and technologies.
- System architecture and design diagrams.
- Interactive interface prototyping.
- A prototype focused on foundational mathematics skills for children aged 4–5.
- Verification and evaluation planning.

The complete implementation of all three age groups, automatic recognition of freely handwritten numerals, and a production-ready educational platform are outside the scope of the initial prototype.

## 7. Technologies

The planned technical approach includes:

| Technology | Purpose |
|---|---|
| Flutter | Cross-platform mobile application development |
| Dart | Main programming language |
| BLoC/Cubit | Proposed state management |
| Hive / Isar | Candidate local storage solutions for learning progress |
| HTML5 and Tailwind CSS | Interactive web prototyping |
| Git and GitHub | Version control, collaboration, and project documentation |

Flutter, Dart, and the proposed BLoC/Cubit architecture are described in the technical design. The final local storage solution will be confirmed by the team.

## 8. Team and Responsibilities

| Team member | Main responsibilities |
|---|---|
| **Bagitzhan Perizat Askhatkyzy** | Research and Documentation |
| **Tyulebayeva Arailym Maratkyzy** | Technical Design and Project Management |

**Supervisor:** Abzal Yermekbayuly Kyzyrkanov

The team collaborates on defining the project scope, reviewing requirements, and preparing the prototype for evaluation.

## 9. Repository Structure

The repository contains project documentation, architecture diagrams, and interactive prototype materials.

```text
Math-learning-app/
├── README.md
├── .gitignore
├── diagrams/
│   ├── system-context.png
│   ├── use-case.png
│   └── component-diagram.png
├── docs/
│   ├── project-proposal.md
│   ├── evidence-of-relevance.md
│   ├── literature-review.md
│   ├── existing-system-comparison.md
│   ├── requirements-specification.md
│   ├── technology-comparison.md
│   ├── architecture-and-diagrams.md
│   ├── verification-plan.md
│   └── supervisor-feedback.md
├── math_learning_app/
│   ├── android/
│   ├── ios/
│   ├── lib/
│   ├── test/
│   ├── pubspec.yaml
│   └── README.md
└── prototypes/
    ├── README.md
    ├── version1.html
    └── version2.html
```
## 10. Project Documentation

- [Project Proposal](docs/project-proposal.md)
- [Evidence of Relevance](docs/evidence-of-relevance.md)
- [Literature Review](docs/literature-review.md)
- [Existing System Comparison](docs/existing-system-comparison.md)
- [Requirements Specification](docs/requirements-specification.md)
- [Technology Comparison](docs/technology-comparison.md)
- [Architecture and Diagrams](docs/architecture-and-diagrams.md)
- [Verification and Evaluation Plan](docs/verification-plan.md)
- [Supervisor Feedback](docs/supervisor-feedback.md)

Architecture diagrams:

- [System Context Diagram](diagrams/system-context.png)
- [Use Case Diagram](diagrams/use-case.png)
- [Component Diagram](diagrams/component-diagram.png)

Interactive prototypes:

- [Prototype Version 1](prototypes/version1.html)
- [Prototype Version 2](prototypes/version2.html)
- [Prototype Documentation](prototypes/README.md)
- **Flutter Application:** [View Flutter Source Code](math_learning_app/)

## 11. Project Management

GitHub Projects is used to organise project tasks and track development progress.

- **Repository:** [Math-learning-app](https://github.com/bagitzanperizat-ux/Math-learning-app)
- **Project Board:** [Math Learning App – Development & Proposal](https://github.com/users/bagitzanperizat-ux/projects/1)

The board uses the following statuses:

- **Todo:** Tasks that have not been started.
- **In Progress:** Tasks currently being worked on.
- **Done:** Completed tasks.

## 12. Current Development Status

The project has progressed from research and documentation to the initial stage of mobile application development.

**Completed:**
- Project proposal and research documentation.
- Literature review and comparison of existing educational applications.
- Functional requirements specification.
- Technology comparison and system architecture diagrams.
- Interactive HTML prototype demonstrating the proposed user experience.
- Initial Flutter project created using Flutter and Dart.
- Flutter project source code uploaded to the GitHub repository.

**In Progress:**
- Development of the Flutter application's user interface.
- Implementation of age-appropriate mathematical activities.
- Integration of interactive exercises, hints, feedback, and progress tracking.

The Flutter application is currently at the initial development stage. The planned educational features have not yet all been implemented or tested.

## 13. Setup, Execution, and Testing

### Current HTML Prototype

The interactive HTML prototype files are located in the `prototypes/` directory.

To inspect a prototype locally:

1. Download or clone the repository.
2. Open the `prototypes/` directory.
3. Open `version1.html` or `version2.html` in a web browser.

If a prototype depends on externally loaded resources, an internet connection may be required.

### Flutter Application

The initial Flutter application project has been created in Android Studio using Flutter and Dart. The project structure has been uploaded to the GitHub repository in the `math_learning_app/` directory.

**Completed setup steps:**
1. Installed and configured the Flutter SDK.
2. Configured the Flutter development environment in Android Studio.
3. Created the initial Flutter project.
4. Generated the default Flutter project structure.
5. Uploaded the Flutter source files to GitHub.

**Development environment:**
- **Framework:** Flutter
- **Programming language:** Dart
- **IDE:** Android Studio
- **Version control:** Git and GitHub

**Next development steps:**
1. Develop the main application screens.
2. Implement interactive mathematics exercises for children aged 4–5.
3. Add answer checking, hints, and feedback.
4. Implement learning progress tracking.
5. Run and test the application on a supported emulator or device.

The Flutter project is currently at the initial development stage. The main educational features have not yet been implemented, and application testing is still to be completed.

## 14. Expected Outcomes

The expected outcomes include:

- A documented project concept and scope.
- Research supported by scientific literature and stakeholder feedback.
- A comparison of existing mathematics-learning applications.
- An initial requirements specification.
- A justified technology selection.
- System architecture diagrams.
- An interactive prototype.
- A verification and evaluation plan.

## 15. Future Development

Potential future improvements include:

- Additional learning journeys for children aged 6–9.
- More mathematical activities and story elements.
- Kazakh-language support.
- Progress summaries for parents and educators.
- Further usability evaluation and assessment of learning-related outcomes.

These possibilities will be considered based on project feedback, available resources, and the results of prototype evaluation.
