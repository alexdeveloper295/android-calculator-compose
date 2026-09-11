# Modern Android Calculator (Jetpack Compose)

A clean, responsive calculator application built with **Jetpack Compose** following **Modern Android Architecture (MVVM + UDF)** principles. Developed as part of advanced Android development practice.

---

## Tech Stack & Key Concepts

- **Language:** Kotlin
- **UI Framework:** Jetpack Compose (Material Design 3)
- **Architecture Pattern:** MVVM (Model-View-ViewModel) + UDF (Unidirectional Data Flow)
- **State Management:** `StateFlow` & `MutableStateFlow`
- **Type-Safe Events & States:** `sealed interface` for UI States & Commands
- **Expression Evaluation:** MathParser (`mXparser`)
- **Dependency Management:** Gradle Version Catalog (`libs.versions.toml`) & Kotlin DSL

---

## Architecture Overview

- **`CalculatorState`:** Represented via a `sealed interface` (`Initial`, `Input`, `Success`, `Error`) ensuring compile-time exhaustive UI handling.
- **`CalculatorCommand`:** Type-safe user intent passed from Composables to the ViewModel.
- **`CalculatorViewModel`:** Encapsulates expression parsing logic, string formatting, and bracket matching (`getCorrectParenthesis()`).

---

## How to Run

1. Clone the repository:
   ```bash
   git clone [https://github.com/YOUR_USERNAME/android-calculator-compose.git](https://github.com/YOUR_USERNAME/android-calculator-compose.git)
