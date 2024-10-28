# Calculator App

A Flutter-based calculator application providing basic arithmetic operations, designed with a clean, dark-themed UI.

## Features

- **Basic Arithmetic Operations**: Supports addition, subtraction, multiplication, and division.
- **Percentage Conversion**: Calculates percentage of the displayed number.
- **Clear and Delete Functions**: "AC" button to reset all fields, and "DEL" button to remove the last entered character.
- **Responsive Layout**: Buttons adjust dynamically for a consistent user experience across devices.
- **Dark Theme**: Minimalistic dark theme for a smooth, visually appealing interface.

## Screenshots

![Screenshot 2023-08-28 225201](https://github.com/AadityaPanda/calculator/assets/95534176/2fc076a1-bc9c-4fe0-a4eb-435c3a8b6cbb)
![Screenshot 2023-08-28 225305](https://github.com/AadityaPanda/calculator/assets/95534176/91a51260-485c-4c8a-82cd-2e4dde67a7de)

## Getting Started

Follow these instructions to get a local copy of the project up and running.

### Prerequisites

- [Flutter SDK](https://flutter.dev/docs/get-started/install)
- Any IDE supporting Flutter (e.g., VS Code, Android Studio)

### Installation

1. **Clone the repository:**
   ```bash
   git clone https://github.com/AadityaPanda/calculator.git
   cd calculator-app
   ```

2. **Install dependencies:**
   ```bash
   flutter pub get
   ```

3. **Run the app:**
   ```bash
   flutter run
   ```

## Project Structure

- `main.dart`: Initializes the app and sets up the dark theme.
- `calculator_screen.dart`: Contains the main layout of the calculator screen, button actions, and calculator logic.
- `button_values.dart`: Defines the buttons and their labels used in the calculator.

## Code Highlights

### main.dart

```dart
import 'package:flutter/material.dart';
import 'calculator_screen.dart';

void main() {
  runApp(const MyApp());
}

class MyApp extends StatelessWidget {
  const MyApp({super.key});

  @override
  Widget build(BuildContext context) {
    return MaterialApp(
      title: 'Calculator',
      debugShowCheckedModeBanner: false,
      theme: ThemeData.dark(),
      home: const CalculatorScreen(),
    );
  }
}
```

### calculator_screen.dart

Handles button presses, arithmetic logic, and displays results.

### button_values.dart

Defines constants for each button label, which are used throughout the app for consistency and ease of maintenance.
