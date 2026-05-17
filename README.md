
# D0S-S0S | Advanced File Generator & System Stress Tester

```text
==========================================================
  _____     ____     _____     _____     ____     _____
 |  __ \   / __ \   / ____|   / ____|   / __ \   / ____|
 | |  | | | |  | | | (___    | (___    | |  | | | (___  
 | |  | | | |  | |  \___ \    \___ \   | |  | |  \___ \ 
 | |__| | | |__| |  ____) |   ____) |  | |__| |  ____) |
 |_____/   \____/  |_____/   |_____/    \____/  |_____/ 
                                                          
================== Created by eshka6 =====================
Overview
D0S-S0S is a high-performance console utility built in C++ designed for stress-testing filesystem I/O operations. By utilizing optimized stream buffering, the application bypasses standard execution bottlenecks to rapidly generate massive amounts of structured dummy data directly onto the local storage.

Developed under Neco Corp, this project serves as a practical implementation of infinite loops, high-speed file streams (fstream), and custom ASCII interface mechanics.

Key Features
🚀 Maximum I/O Throughput: File stream pointers are initialized outside the execution loop to ensure uninterrupted hardware write operations.

🛡️ Robust Error Handling: Features complete input verification to prevent stack crashes and invalid runtime executions.

🖥️ Cyberpunk ASCII Interface: Custom-engineered console viewport rendering.

💾 Persistent Logging: Leverages the ios::app flag to securely append data without overriding existing blocks.

Technical Specifications
Language: C++ (ISO C++17 or higher recommended)

Core Libraries: <fstream>, <thread>, <chrono>, <windows.h>

Platform: Windows (utilizes native UTF-8 65001 code pages for console stability)

Installation & Compilation
To compile the source code manually using MinGW / GCC via terminal, execute the following command:

Bash
g++ -O3 main.cpp -o D0S-S0S.exe
(Note: The -O3 flag is highly recommended to enable compiler optimization for maximum file-generation speed).

Usage
Launch the compiled binary D0S-S0S.exe.

Wait for system initialization.

Enter 1 to deploy the stress-test sequence, or 0 to safely terminate the process.

Warning: Monitor your storage capacity during execution. The program will continuously allocate disk blocks until manually aborted (Ctrl + C or closing the terminal window).

Disclaimer
This software is developed strictly for educational and benchmarking purposes. The developer (eshka6 / Neco Corp) is not responsible for any unexpected hardware wear or storage depletion caused by prolonged stress-testing.
