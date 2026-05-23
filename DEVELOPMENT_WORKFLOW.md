# VideoStreamApp Development Workflow

## Purpose

This repository is for learning SwiftUI and Jetpack Compose by building small video streaming app UI features.

The target domain is long-form and broadcaster-style video services such as TVer, Netflix, and Hulu. The goal is not to copy any specific product, but to practice common UI structures, screen states, and implementation patterns used in streaming apps.

## Collaboration Style

Development should proceed in small, reviewable tasks.

The user reviews and understands each change before the next task starts. This repository should not be developed in large AI-driven batches.

Each task should be close to one Scrum development task, not an entire feature epic.

## Task Granularity

Each task should usually satisfy these constraints:

- One clear goal.
- One reviewable diff.
- Small enough to understand in one sitting.
- Preferably limited to one platform, one screen, or one architectural decision.
- No unrelated refactoring.
- No UI implementation mixed with project scaffolding unless explicitly scoped.

Examples of good task sizes:

- Decide repository directory structure.
- Add SwiftUI app scaffold only.
- Add Compose app scaffold only.
- Define shared sample content model in documentation.
- Build SwiftUI home screen static layout.
- Build Compose home screen static layout.
- Add loading and error states to one screen.
- Add navigation from home to detail on one platform.

Examples of tasks that are too large:

- Build the full app.
- Implement SwiftUI and Compose apps with all screens at once.
- Add API, persistence, navigation, and UI polish in one change.
- Refactor project structure while adding new user-facing behavior.

## Initial Product Direction

Use a fictional video streaming app concept.

Working name: `VideoStreamApp`.

Core UI patterns to practice:

- Home feed with hero content and horizontal content rails.
- Continue watching rail.
- Ranking or trending rail.
- Content detail page.
- Episode list.
- Playback surface and controls.
- Search and category browsing.
- Empty, loading, error, and restricted-content states.

## Suggested Task Sequence

### Task 002: Repository Structure Decision

Goal: Decide how SwiftUI and Compose code will live in this repository.

Expected output:

- A short Markdown decision record.
- Directory plan for iOS and Android or Compose modules.
- No app scaffolding yet.

Review focus:

- Is the structure easy to compare across SwiftUI and Compose?
- Is it simple enough for a learning repository?
- Does it avoid premature abstraction?

### Task 003: SwiftUI Scaffold

Goal: Add the minimal SwiftUI app shell.

Expected output:

- iOS project or Swift package structure.
- A launchable placeholder screen.
- No streaming UI yet.

Review focus:

- Can the project build?
- Is the scaffold minimal?
- Are generated files understandable?

### Task 004: Compose Scaffold

Goal: Add the minimal Compose app shell.

Expected output:

- Android or Compose Multiplatform project structure.
- A launchable placeholder screen.
- No streaming UI yet.

Review focus:

- Can the project build?
- Is the scaffold comparable to the SwiftUI side?
- Are dependencies minimal?

### Task 005: Streaming Home UI Spec

Goal: Define the first screen before implementing it.

Expected output:

- Static home screen requirements.
- Sample content data shape.
- List of UI states to support later.

Review focus:

- Does the spec resemble real streaming app work?
- Is the first implementation small enough?

### Task 006: SwiftUI Home Static Layout

Goal: Implement the first static home screen in SwiftUI.

Expected output:

- Hero area.
- Horizontal content rails.
- Static sample data.
- No networking.

Review focus:

- SwiftUI layout readability.
- State kept minimal.
- UI structure maps clearly to the spec.

### Task 007: Compose Home Static Layout

Goal: Implement the same home screen in Compose.

Expected output:

- Hero area.
- Horizontal content rails.
- Static sample data.
- No networking.

Review focus:

- Compose layout readability.
- Similarity and differences versus SwiftUI.
- Avoidance of unnecessary architecture.

## Review Checklist

For every task, review these points before moving on:

- Does the change match the task scope?
- Are there unrelated edits?
- Is the implementation understandable for learning?
- Is there a simpler solution?
- Are naming and file placement consistent?
- Does the project still build when applicable?
- Are follow-up tasks clearly separated?

## Current Repository State

- GitHub repository: `https://github.com/saga138/VideoStreamApp`
- Visibility: public
- Current branch: `main`
- Existing tracked files: `README.md`, `.gitignore`
- Local task notes under `task/` or `tasks/` are ignored by Git.

