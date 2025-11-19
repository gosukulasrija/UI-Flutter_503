### Experiment 1: Dart Basics

| File | Concept | Description |
| :--- | :--- | :--- |
| `experiment1a.dart` | **Simple Dart Program** | Introduces basic Dart concepts: `void main()`, `print()` for I/O, variable declaration (`int x`), and **string interpolation** (`${x + y}`). |
| `1b` | **Installation** | Guide for setting up the required Flutter SDK and Dart environment. |

---

### Experiment 2: Widgets & Layouts

| File | Concept | Description |
| :--- | :--- | :--- |
| `experiment2a.dart` | **Basic Widgets** | Demonstrates the fundamental UI components: **`Text`**, **`Image.network`** (external asset loading), and **`Container`** for adding padding, color, and structural properties. |
| `experiment2b.dart` | **Layouts** | Illustrates how widgets are positioned: **`Row`** (horizontal), **`Column`** (vertical), and **`Stack`** (Z-axis overlaying, often used with `Positioned`).  |

---

### Experiment 3: Responsive UI

| File | Concept | Description |
| :--- | :--- | :--- |
| `experiment3a.dart` | **Using `MediaQuery`** | Retrieves **global device information** (e.g., `MediaQuery.of(context).size.width`) to make high-level decisions, such as rendering separate Mobile vs. Desktop views. |
| `experiment3b.dart` | **Using `LayoutBuilder`** | Adapts the UI based on the **local constraints of the parent widget** (`c.maxWidth`), making it ideal for inner components that must fit dynamic spaces.  |

---

### Experiment 4: Navigation

| File | Concept | Description |
| :--- | :--- | :--- |
| `experiment4a.dart` | **Push & Pop** | Standard stack navigation: **`Navigator.push()`** adds a screen to the stack, and **`Navigator.pop()`** removes the top screen, returning to the previous one.  |
| `experiment4b.dart` | **Named Routes** | Defines routes globally in the `MaterialApp` (`/`, `/second`) for cleaner, string-based navigation using **`Navigator.pushNamed()`**. |

---

### Experiment 5: Stateful vs. Stateless

| File | Concept | Description |
| :--- | :--- | :--- |
| `experiment5a.dart` | **Stateless Example** | An immutable **`StatelessWidget`** used for static content that does not change after initial creation. |
| `experiment5b.dart` | **Stateful Counter** | A **`StatefulWidget`** holds mutable data (state). Calling **`setState()`** notifies the framework to re-run the `build` method and update the UI efficiently.  |

---

### Experiment 6: Custom Widgets & Styling

| File | Concept | Description |
| :--- | :--- | :--- |
| `experiment6a.dart` | **Custom Widget** | Creates a reusable `MyBtn` widget, demonstrating the core principle of **composition** (breaking the UI into small, manageable components). |
| `experiment6b.dart` | **Simple Theme** | Uses **`ThemeData`** in the `MaterialApp` to apply a global style (e.g., `primarySwatch: Colors.teal`), ensuring **brand consistency** across all Material widgets. |

---

### Experiment 7: Forms

| File | Concept | Description |
| :--- | :--- | :--- |
| `experiment7a.dart` | **Simple Form** | Basic text input using the **`TextField`** widget and visual hints via `InputDecoration`. |
| `experiment7b.dart` | **Form with Validation** | Uses the **`Form`** widget with a **`GlobalKey`** to manage state. **`TextFormField`** uses a `validator` function to ensure data integrity before submission. |

---

### Experiment 8: Animations

| File | Concept | Description |
| :--- | :--- | :--- |
| `experiment8a.dart` | **Implicit (`AnimatedContainer`)** | **Easiest animation**: The widget automatically handles the smooth transition of properties (size, color) over a set `duration` when its values change. |
| `experiment8b.dart` | **Explicit (`FadeTransition`)** | Requires manual control using an **`AnimationController`** and **`SingleTickerProviderStateMixin`**. This allows for complex control like reversing and repeating. |

---

### Experiment 9: API Integration

| File | Concept | Dependency | Description |
| :--- | :--- | :--- | :--- |
| `experiment9a.dart` | **Fetch Users** | `http` | Uses **`async`/`await`** and the `http` package to fetch JSON data from a REST API. **`jsonDecode`** converts the string response into Dart objects. |
| `experiment9b.dart` | **Display in Cards** | `http` | Enhances UI presentation by displaying the fetched data within **`Card`** widgets, improving visual separation and readability. |

---

### Experiment 10: Testing

| File | Concept | Location | Description |
| :--- | :--- | :--- | :--- |
| `lib/functions.dart` | **Simple Function** | `lib/` | The target Dart function (`add(a, b)`) designed for testing in isolation. |
| `test/unit_test.dart` | **Unit Test** | `test/` | Uses **`flutter_test`** to verify individual code units. **`expect()`** is the key assertion that ensures the function's actual output matches the expected result. |