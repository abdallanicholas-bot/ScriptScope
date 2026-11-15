ScriptScope
ScriptScope is an all-in-one, multi-language development environment designed to simplify coding, debugging, analyzing, and optimizing software.

Combining an IDE-style code editor with a visual runtime debugger and static analysis engine, ScriptScope provides developers with a centralized workspace to write code, inspect program execution, identify potential issues, and improve code quality.

With support for JavaScript, Java, C#, Python, C, C++, Rust, and Go, ScriptScope aims to provide a unified development experience across multiple programming languages.

Key Features
Multi-Language Support: Work with JavaScript, Java, C#, Python, C, C++, Rust, and Go.
Integrated Code Editor: Write, edit, and manage code through an IDE-style interface.
Visual Runtime Debugger: Inspect program execution and better understand how your code behaves.
Static Code Analysis: Identify potential errors, problematic patterns, and code quality issues.
Code Optimization: Identify opportunities to improve code efficiency and readability.
JavaScript Runtime Support: Supports both browser-based JavaScript and Node.js development.
Local-First Architecture: Designed around an accessible local development workflow.
Language Support & Requirements
Some languages require additional software to be installed and configured on Windows.

Language	Windows Requirements
JavaScript	Supported runtime environment
Java	Java Development Kit (JDK)
C#	.NET SDK
Python	Python installation
C	MSYS2 GCC and GDB
C++	MSYS2 GCC and GDB
Rust	Rust GNU toolchain
Go	Go installation
Windows Setup for C, C++, and Rust
These languages require additional compiler and debugging tools.

C and C++

Install MSYS2.
Install the GCC compiler toolchain.
Ensure GDB is installed for debugging.
Configure the appropriate executable paths in ScriptScope if required.
Rust

Install the Rust GNU toolchain.
Ensure the GNU compiler and debugging dependencies are configured.
Configure the necessary tool paths in ScriptScope if required.
Important: ScriptScope does not automatically install these external dependencies. Make sure the required tools are installed and accessible before compiling or debugging projects.

Known Limitations
Some programming language features currently have limitations within ScriptScope's runtime debugging and variable inspection systems.

Go
Goroutines: Only the main goroutine is recorded by the debugger. Other goroutines execute normally, but their execution lines are not displayed.
Rust
Moved Values: After a value is moved, its variable may display whatever data remains in its memory location. This does not necessarily represent a valid or accessible Rust value.
These limitations affect debugger visibility and variable inspection rather than necessarily preventing programs from executing.

Download & Installation
Navigate to the GitHub Releases page.
Find the latest ScriptScope release.
Download the portable .exe file.
Open the downloaded executable to launch ScriptScope.
Windows Defender / SmartScreen Warning
Windows may display a warning when launching ScriptScope, such as "Windows protected your PC" or an unknown publisher warning.

This can happen when an executable is unsigned or has not established sufficient download reputation with Microsoft.

If you downloaded ScriptScope from this repository's official Releases page and have verified the file:

Click More info on the Windows SmartScreen warning.
Review the application and publisher information if you want.
Click Run anyway.
Security Note: ScriptScope contains no malware or anything negative that could hurt your system.

Project Vision
ScriptScope aims to bring together the capabilities of traditional code editors, debugging environments, and static analysis tools into one cohesive application.

By supporting multiple programming languages and combining development with visual code inspection, ScriptScope strives to make understanding, debugging, and improving code more accessible and efficient.

The long-term goal is to create a flexible development environment that reduces the need to constantly switch between separate programming tools.
