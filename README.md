# Android-Fragments-with-Responsive-UI_MAD_EXP3
This project demonstrates the implementation of Android Fragments to build a flexible and responsive user interface using Kotlin. The application contains two Fragments: a List Fragment that displays a list of courses and a Detail Fragment that shows information about the selected course.

# Android Fragments with Debugging – Experiment 3

## Project Title

**Android Fragments with Flexible UI and Debugging using Breakpoints**

---

# Overview

This Android application demonstrates the implementation of **Fragments** to create a flexible and responsive user interface.

The application consists of:

- **List Fragment** – Displays a list of items (Courses).
- **Detail Fragment** – Displays information about the selected item.

The application is designed to work on different screen sizes by using fragments.

Additionally, Android Studio Debugger is used to analyze the application's execution using:

- Normal Breakpoint
- Conditional Breakpoint
- Variable Inspection
- Call Stack Analysis
- Fragment Lifecycle Observation

---

# Objectives

- Learn how to use Fragments in Android.
- Implement communication between Fragments.
- Create a responsive UI.
- Understand Fragment Lifecycle.
- Learn Android Studio Debugging.
- Use Normal and Conditional Breakpoints.
- Inspect Variables and Call Stack.

# Technologies Used

- Kotlin
- Android Studio
- Android SDK
- Fragments
- ConstraintLayout
- RecyclerView/ListView (Optional)
- Android Debugger

---

# Project Structure

```text
app
│
├── java
│   └── com.example.fragmentdemo
│       │
│       ├── MainActivity.kt
│       ├── ListFragment.kt
│       ├── DetailFragment.kt
│       └── Course.kt (optional)
│
├── res
│   ├── layout
│   │      activity_main.xml
│   │      fragment_list.xml
│   │      fragment_detail.xml
│   │
│   ├── values
│   │      strings.xml
│   │
│   └── drawable
│
└── AndroidManifest.xml
```

---

# Sample Course List

```text
Android
Java
Python
Kotlin
Flutter
Machine Learning
Data Science
Cloud Computing
```

---

# Working

### Step 1

Application starts.

↓

### Step 2

ListFragment displays all available courses.

↓

### Step 3

User selects a course.

↓

### Step 4

Selected course name is sent to DetailFragment.

↓

### Step 5

DetailFragment displays the course description.

↓

### Step 6

Debugger can pause execution at Breakpoints.

---

# Fragment Communication

```text
ListFragment

        │

        ▼

Selected Item

        │

        ▼

MainActivity

        │

        ▼

DetailFragment
```

---

# Debugging Implementation

This project demonstrates Android Studio Debugger.

## 1. Normal Breakpoint

A breakpoint is placed inside:

```text
DetailFragment.kt

onCreateView()

or

onViewCreated()
```

Whenever the DetailFragment is opened, execution pauses automatically.

From the Debug Window, you can inspect:

- Variables
- Call Stack
- Fragment Lifecycle
- Threads

---

## 2. Conditional Breakpoint

A conditional breakpoint is placed inside:

```text
ListFragment

Item Click Listener
```

Condition:

```kotlin
selectedItem == "Android"
```

Execution pauses only when the selected item is **Android**.

If any other item is clicked, execution continues normally.


# Debug Window Inspection

During debugging, inspect:

- Variables
- Local Variables
- Watches
- Call Stack
- Threads
- Evaluate Expression
- Fragment Lifecycle

---

# Expected Output

### Home Screen

```text
Courses

Android

Java

Python

Flutter

Machine Learning

Cloud Computing
```

---

### Detail Screen

```text
Course

Android

Android is Google's mobile operating system used for developing mobile applications using Kotlin and Java.
```

---


# How to Run the Project

1. Open Android Studio.
2. Click **File → Open**.
3. Select the project folder.
4. Wait for Gradle Sync.
5. Connect an Android device or start an Emulator.
6. Click **Run ▶** or press **Shift + F10**.

---

# Running in Debug Mode

Instead of Run:

- Click **Debug 🐞**
- Or press **Shift + F9**

The application will launch in Debug Mode.



