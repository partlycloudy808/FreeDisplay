# Jules AI Agent Configuration: FreeDisplay

## Project Overview
FreeDisplay is a native macOS display manager written in Swift and SwiftUI, designed to run exclusively on Apple Silicon (arm64).

## ⚠️ CRITICAL ENVIRONMENT CONSTRAINTS ⚠️
- **No Compilation:** You are operating within a Linux Cloud VM. You **cannot** compile, build, or test this macOS application. 
- **Do Not Run Build Commands:** Do NOT attempt to execute `xcodebuild`, `swift build`, `make`, `pip`, or `pytest`.
- **Static Analysis Only:** You must rely entirely on static code analysis, your understanding of the Swift language, and your knowledge of macOS APIs to write and refactor code.

## Tech Stack & Architecture
- **Language:** Swift 6.
- **UI Framework:** SwiftUI.
- **Hardware Control:** Native Apple Silicon `IOAVService` bindings.
- **Build System:** The project uses `XcodeGen` (`project.yml`) to generate the `.xcodeproj`. 

## Task Execution Directives
1. When asked to implement a feature (e.g., custom display resolutions via `CoreDisplay` or `CGVirtualDisplay`), write the exact Swift implementation.
2. Place hardware/display logic in the `Services/` directory.
3. Ensure any C-header bridging for private Apple frameworks is correctly mapped.
4. Because you cannot test the code locally, you must output highly defensive, safe, and heavily commented Swift code before opening the Pull Request.
