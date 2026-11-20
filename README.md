# ScriptScope

**ScriptScope** is an all-in-one, multi-language development environment designed to simplify coding, debugging, analyzing, and optimizing software.

Combining an IDE-style code editor with a visual runtime debugger and static analysis engine, ScriptScope provides developers with a centralized workspace to write code, inspect program execution, identify potential issues, and improve code quality.

With support for JavaScript, Java, C#, Python, C, C++, Rust, and Go, ScriptScope aims to provide a unified development experience across multiple programming languages.

---

## Key Features

- **Multi-Language Support:** Work with JavaScript, Java, C#, Python, C, C++, Rust, and Go.
- **Integrated Code Editor:** Write, edit, and manage code through an IDE-style interface.
- **Visual Runtime Debugger:** Inspect program execution through an interactive execution timeline.
- **AST-Based Instrumentation:** Analyze JavaScript code structure and generate execution events while preserving source locations.
- **Source Code Highlighting:** Navigate directly to relevant lines of code when inspecting execution events.
- **Variable Tracking:** Observe variable declarations, assignments, and updates during execution.
- **Function Tracking:** Record function calls, entries, and returns.
- **Branch Tracking:** Inspect conditional decisions and short-circuit evaluations.
- **Static Code Analysis:** Identify potential errors, problematic patterns, and code quality issues.
- **Code Optimization:** Identify opportunities to improve code efficiency and readability.
- **JavaScript Runtime Support:** Designed to support both browser-based JavaScript and Node.js development.
- **Local-First Architecture:** Designed around an accessible local development workflow.

---

## Language Support & Requirements

Some languages require additional software to be installed and configured on Windows.

| Language | Windows Requirements |
|---|---|
| JavaScript | Supported runtime environment |
| Java | Java Development Kit (JDK) |
| C# | .NET SDK |
| Python | Python installation |
| C | MSYS2 GCC and GDB |
| C++ | MSYS2 GCC and GDB |
| Rust | Rust GNU toolchain |
| Go | Go installation |

### Windows Setup for C, C++, and Rust

These languages require additional compiler and debugging tools.

**C and C++**

1. Install MSYS2.
2. Install the GCC compiler toolchain.
3. Ensure GDB is installed for debugging.
4. Configure the appropriate executable paths in ScriptScope if required.

**Rust**

1. Install the Rust GNU toolchain.
2. Ensure the GNU compiler and debugging dependencies are configured.
3. Configure the necessary tool paths in ScriptScope if required.

**Important:** ScriptScope does not automatically install these external dependencies. Make sure the required tools are installed and accessible before compiling or debugging projects.

---

## Visual Debugging & Execution Tracking

ScriptScope's visual debugging system is designed to make program execution easier to understand.

Rather than only displaying program output, the debugger records execution events and presents them through an interactive timeline.

Current JavaScript instrumentation includes:

- Variable declarations and assignments.
- Variable updates, including increment and decrement operations.
- Function calls.
- Function entries and returns.
- Conditional branch decisions.
- Short-circuit evaluations.
- Source-location tracking.

Selecting an execution event allows the corresponding source location to be highlighted in the editor.

The instrumentation engine is still being expanded, and not all JavaScript language constructs are currently supported.

---

## Known Limitations

Some programming language features currently have limitations within ScriptScope's runtime debugging and variable inspection systems.

**Go Goroutines:**
Only the main goroutine is recorded by the debugger. Other goroutines execute normally, but their execution lines are not displayed.

**Rust Moved Values:**
After a value is moved, its variable may display whatever data remains in its memory location. This does not necessarily represent a valid or accessible Rust value.

**JavaScript Instrumentation:**
Some language constructs are not fully instrumented, including destructuring, object-property modifications, certain function invocation patterns, and asynchronous execution.

**JavaScript Execution Safety:**
The browser-based JavaScript execution prototype uses Web Workers to separate execution from the main interface thread. However, a Web Worker is not a security sandbox. Only execute trusted code.

**Node.js Execution:**
Node.js is a planned separate execution target. Direct Node.js code execution is not currently enabled.

These limitations primarily affect debugger visibility, instrumentation, and variable inspection rather than necessarily preventing programs from executing.

---

## Download & Installation

1. Navigate to the GitHub Releases page.
2. Find the latest ScriptScope release.
3. Download the portable `.exe` file.
4. Open the downloaded executable to launch ScriptScope.

No traditional installation process is required for the portable version.

### Windows Defender / SmartScreen Warning

Windows may display a warning when launching ScriptScope, such as "Windows protected your PC" or an unknown publisher warning.

This can happen when an executable is unsigned or has not established sufficient download reputation with Microsoft.

If you downloaded ScriptScope from this repository's official Releases page and have independently verified the file:

1. Click **More info** on the Windows SmartScreen warning.
2. Review the application and publisher information.
3. Click **Run anyway** if you decide to proceed.

**Security Note:** Always verify downloaded executables before running them. An official repository release is the recommended download source.

---

## Project Vision

ScriptScope aims to bring together the capabilities of traditional code editors, debugging environments, and static analysis tools into one cohesive application.

By supporting multiple programming languages and combining development with visual code inspection, ScriptScope strives to make understanding, debugging, and improving code more accessible and efficient.

The long-term goal is to create a flexible development environment that reduces the need to constantly switch between separate programming tools.

Future development will focus on expanding debugging capabilities, improving static analysis, introducing more advanced code optimization, and strengthening support for different programming languages.

---

## Project Status

ScriptScope is actively being developed. Features and language support may have varying levels of completeness, particularly within runtime debugging and execution instrumentation.

Contributions, suggestions, and feedback are welcome.
