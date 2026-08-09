<div align="center">

# ⚡ Competitive Programming Template

_An optimized template and VS Code snippet setup designed to accelerate C++ workflows in competitive programming._

[![C++ Version](https://img.shields.io/badge/C%2B%2B-17%2F20-blue?style=for-the-badge&logo=c%2B%2B)](https://en.cppreference.com/)
[![Editor Support](https://img.shields.io/badge/Editor-VS%20Code-007acc?style=for-the-badge&logo=visual-studio-code)](https://code.visualstudio.com/)
[![License](https://img.shields.io/badge/License-Apache_2.0-orange?style=for-the-badge)](LICENSE)

<p align="center">
  <a href="#-introduction">Introduction</a> •
  <a href="#-quick-start">Quick Start</a> •
  <a href="#-deep-dive-debugger-showcase">Deep Dive</a> •
  <a href="#-license">License</a>
</p>

</div>

---

## 📖 Introduction

This is a personal repository containing optimized template configurations and VS Code snippets for C++ in competitive programming. It is structured to automate common boilerplate code, set up fast input/output configurations, and provide helper debugging macros (`dbg(x)`) for local testing.

While created for personal use, feel free to use, modify, or adapt any parts of this setup for your own competitive programming journey if you find it helpful.

---

## 🛠️ Quick Start

### 1. Integrate VS Code Snippet
1. Copy the contents of [`snippets.json`](snippets.json).
2. Open VS Code and open the Command Palette (`Ctrl + Shift + P` / `Cmd + Shift + P`).
3. Select **Preferences: Configure User Snippets** -> **cpp.json** (or create a new C++ snippet file).
4. Paste the snippet configuration and save.
5. In any `.cpp` file, type `cpp` and press `Tab` to generate the template.

> 💡 **Tip:** If you want to customize the template or create your own custom snippets, you can use this online [Snippet Generator](https://snippet-generator.app/) to easily convert raw code to VS Code JSON format.

### 2. Compilation Commands
* **Local Mode (with debug output)**:
  ```bash
  g++ -O3 solution.cpp -o solution
  ./solution
  ```
* **Judge Mode (disables debug prints)**:
  ```bash
  g++ -DONLINE_JUDGE -O3 solution.cpp -o solution
  ```

---

## 🔍 Deep Dive: Debugger Showcase

The debugger helper (`dbg(x)`) automatically detects types and formats them. Here is a comparison of how outputs are formatted:

| Code Expression | Output format in standard error (`cerr`) |
| :--- | :--- |
| `int x = 42; dbg(x);` | `x = 42` |
| `pair<int, string> p = {1, "code"}; dbg(p);` | `p = {1,code}` |
| `vector<int> v = {1, 2, 3}; dbg(v);` | `v = [ 1 2 3 ]` |
| `map<char, int> mp = {{'a', 1}}; dbg(mp);` | `mp = [ {a,1} ]` |

---

## ⚖️ License

Distributed under the Apache License 2.0. See [`LICENSE`](LICENSE) for more information.