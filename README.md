# SoftwareSecurity

Security Labs & Algorithm Implementations Repository

This repository consolidates several core systems-security labs alongside classical algorithm implementations. The intent is simple: create a single, structured workspace containing reverse-engineering, privilege-escalation exploits, memory-corruption attacks, format-string exploitation, and search-based pathfinding. Each module is standalone, testable, and engineered for reproducibility.

The repo is anchored around practical, hands-on security work. Nothing here is theoretical; every lab interacts directly with the machine—binary manipulation, stack control, process privileges, memory introspection, and exploit payload construction.

⸻

Repository Structure

1. Lab 1 — Reverse Engineering Assembly Code

This module focuses on understanding program behavior by reverse-engineering compiled binaries.
Skills demonstrated:
• Reading and mapping x86/x86-64 instructions
• Structuring control flow from assembly
• Reconstructing source-level intent
• Identifying computation patterns and memory access strategies

The output is a fully documented breakdown of the binary, its logic, and its vulnerabilities.

⸻

2. Lab 2 — Set-User-ID (SUID) Executive Behavior

This lab explores privilege escalation paths through SUID binaries. The work includes:
• Understanding effective vs real UID and privilege propagation
• Investigating secure vs insecure SUID interactions
• Building controlled demonstrations of privilege escalation
• Validating system protection behavior

It clarifies exactly where poor SUID design leaks system control.

⸻

3. Lab 3 — Environment Variable Manipulation

Environment variables are often underestimated attack surfaces. This module shows how they shape program execution:
• Overriding library paths
• Injecting payloads via environment expansion
• Observing how privileged programs ingest and trust environment-level data
• Designing controlled experiments to detect unsafe variable handling

This is foundational for later exploitation labs.

⸻

4. Lab 4 — Buffer Overflow (Stack-Based Exploitation)

Referencing  ￼
This is the core offensive-security module. It includes:
• Analyzing stack frames and return-address overwrite mechanics
• Injecting shellcode to spawn privileged shells
• Defeating ASLR, StackGuard, and non-executable stack settings
• Constructing badfile payloads and tuning NOP sleds
• Iteratively refining offset calculations

The lab demonstrates clean, controlled exploitation to achieve root-level execution.

⸻

5. Lab 5 — Format String Vulnerabilities

Referencing  ￼
This module dives into format-string exploitation, which is significantly more subtle than buffer overflows. It covers:
• Forcing arbitrary memory reads
• Crashing the target process
• Overwriting internal variables, including multi-byte controlled writes
• Injecting shellcode and redirecting execution via return-address manipulation
• Achieving remote code execution over UDP

This lab shows why unsafe printf(msg) patterns remain one of the most expensive real-world mistakes.

⸻
How to Run Each Module

Every folder includes:
• Source code
• Clear execution instructions
• Expected outputs
• Optional extended tasks for deeper experimentation

Where applicable, privileged operations are sandboxed and should only run inside controlled virtual environments.

⸻

Why This Repo Exists

This repository is not coursework. It’s capability signaling. It demonstrates breadth across:
• Low-level system behavior
• Memory manipulation
• Secure coding principles
• Exploitation methodology
• Classical algorithm design
• Reverse engineering

The integrations show a consistent pattern: strong systems intuition and the ability to reason directly about machine-level execution.
