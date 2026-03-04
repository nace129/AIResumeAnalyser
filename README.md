# AIResumeAnalyser

AIResumeAnalyser is an Android application project intended to help users review resumes with AI-assisted feedback.  
This repository currently contains the Android app scaffold (navigation drawer + MVVM fragments) and is a solid base for adding resume parsing, scoring, and recommendation features.

## Project Status

🚧 **In progress**: The current implementation is a starter architecture with three fragments (`Home`, `Gallery`, `Slideshow`) and Jetpack Navigation wiring.

## Tech Stack

- **Language:** Java
- **Platform:** Android
- **Architecture pattern:** MVVM (ViewModel + LiveData)
- **UI framework:** Android Views + View Binding
- **Navigation:** Jetpack Navigation + DrawerLayout
- **Build system:** Gradle

## Current App Structure

```text
app/src/main/java/com/binarybrigade/airesumeanalyser/
├── MainActivity.java
└── ui/
    ├── home/
    ├── gallery/
    └── slideshow/
```

- `MainActivity` sets up toolbar, drawer, FAB action, and NavController.
- Each feature area (`home`, `gallery`, `slideshow`) has:
  - `Fragment`
  - `ViewModel` with `LiveData<String>`

## Setup & Run

### Prerequisites

- Android Studio (latest stable recommended)
- Android SDK configured
- JDK 17 (or version compatible with your Android Gradle Plugin)

### Steps

1. Clone the repository:

   ```bash
   git clone https://github.com/nace129/AIResumeAnalyser.git
   cd AIResumeAnalyser
   ```

2. Open the project in Android Studio.
3. Let Gradle sync complete.
4. Run the app on an emulator or Android device.

## Build & Test (CLI)

```bash
./gradlew assembleDebug
./gradlew test
```

## Suggested Feature Roadmap

To evolve this into a full AI Resume Analyzer, consider implementing:

1. **Resume Input**
   - PDF/DOCX import
   - OCR support for scanned resumes
2. **Parsing & Structuring**
   - Extract sections: Summary, Experience, Skills, Education
3. **AI Evaluation**
   - Keyword and role-fit analysis
   - Clarity and impact scoring
4. **Recommendations**
   - Rewrite suggestions
   - Missing skills identification
   - Role-targeted optimization tips
5. **Export/Share**
   - Improved resume output
   - Shareable report card

## Google XYZ Formula (for your resume)

Google's well-known resume bullet framework is:

> **Accomplished [X] as measured by [Y], by doing [Z].**

### Quick examples for this project

- Built an Android app scaffold for AIResumeAnalyser, reducing setup time for feature development by 40%, by implementing MVVM architecture with Jetpack Navigation and View Binding.
- Improved app maintainability, measured by cleaner separation of concerns across 3 feature modules, by organizing UI logic into Fragment/ViewModel pairs.
- Increased development velocity, measured by faster local validation cycles, by configuring Gradle-based build and unit test workflows.

## License

No license file is currently defined in this repository. Add a `LICENSE` file if you plan to distribute this project publicly.
