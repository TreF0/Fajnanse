# 💰 Fajnanse - Personal Finance Management System

![C++](https://img.shields.io/badge/C%2B%2B-17-blue.svg?style=flat&logo=c%2B%2B)
![CMake](https://img.shields.io/badge/CMake-Build-green.svg?style=flat&logo=cmake)
![Tesseract](https://img.shields.io/badge/OCR-Tesseract-red.svg?style=flat)

**Fajnanse** is a finance management application developed as a university project at the **Poznań University of Technology**. It focuses on automating expense tracking through hardware-software integration.

---

## 🔍 Project Overview
The application automates the process of logging expenses by utilizing the **Tesseract OCR** engine. Users can upload images of receipts, which the system then parses to extract key data such as dates, amounts, and currencies, automatically assigning them to predefined budget categories.

### Key Technologies:
* **Language:** C++17
* **Build System:** CMake
* **OCR Engine:** Tesseract
* **Environment:** GitHub Codespaces & VS Code

---

## 👥 Authors & My Role
This was a collaborative effort where I focused on the core interaction layer and quality assurance:

* **[Łukasz Cieślik](https://github.com/TreF0)** – developer of CLI, testing
* **Mateusz Czarnecki** – backend developer, documentation, testing
* **Olimpia Laube** – GUI developer, documentation, testing

---

## ✨ Features
* **Automated Data Entry:** OCR-based receipt scanning and parsing.
* **Multi-interface Support:** Interaction via both a web-based GUI and a terminal-based CLI.
* **Financial Tracking:** Real-time balance updates and transaction history management.
* **Robust Toolchain:** Built with modern C++ standards and automated CMake configuration.

---

## 🚀 Getting Started
The project is optimized for **GitHub Codespaces** to ensure all dependencies (Tesseract, etc.) are correctly configured.

1. Launch the Codespace.
2. Configure and build the project using the **CMake** extension (GCC 10.2.0+).
3. Run the executable:
   ```bash
   ./bin/Fajnanse