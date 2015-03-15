# What is QPasm? #

The PASM Library (LibPASM) provides a simple pseudo-assembler interpreter. This library provides the building blocks for creating a small Integrated Development Environment for small pseudo-assembler programs.

QPasm makes use of the PASM Library to provide a small Integrated Development Environment for small pseudo-assembler programs.

# Why does it exist? #

Both LibPASM and QPasm are being developed by Wesley Stessens.

QPasm implements the same basic pseudo-assembler language as the one being taught in the first year at Hasselt University in the course "Computer systems". The only difference is that the implemented language in QPasm also supports labels to make programming easier.

QPasm is primarily used as a replacement for the older SCASM which was used for the course before.

# Features #

  * Modular UI design: C backend with C++/Qt frontend
  * Pseudo-assembler apps are stored in virtual static memory. Data can be stored in either virtual static or dynamic memory. Memory management is implemented according to Von Neumann architecture meaning instructions can be modified at run-time
  * Code editor with intelligent syntax highlighting, line numbering, visual breakpoints and undo/redo functionality
  * Debugging features: breakpoints, manual step, timed step, pausing
  * On-the-fly editing of data in the register or the memory
  * On-the-fly symbol resolving: labels can be used in assembler apps, and when modifying memory when the program is running the labels are resolved automatically
  * Integrates well with light and dark system themes. Highlighter chooses its color theme based on the darkness of the theme automatically, but colors and fonts can be configured manually as well
  * Layout, font and color settings are stored locally in a portable config.ini file
  * Input format is very flexible: white space may occur before, after and between instructions, instructions are case insensitive, comments are supported anywhere
  * Pseudo-assembler apps which are run using the run-function run in a separate thread which has a system preventing the GUI from freezing by limiting the amount of simultaneous signals to the GUI. Assembler apps which cause an endless loop cannot freeze the GUI

![http://wesley.vidiqatch.org/images/qpasm_1.1_rc1.png](http://wesley.vidiqatch.org/images/qpasm_1.1_rc1.png)