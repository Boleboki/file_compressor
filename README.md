# 🗜️ NinjaZIP - File Compression Tool

**NinjaZIP** is a lightweight command-line data compression and archiving utility written in C. It supports compression and extraction using lossless algorithms such as Static Huffman, Dynamic Huffman, and LZW (Lempel-Ziv-Welch).

---

## 📌 Features

* **Lossless Compression**: Implementation of Static Huffman, Dynamic Huffman, and LZW coding.
* **Archiving & Extraction**: Compress files or directories into custom `.nzip` archives and extract them seamlessly.
* **CLI Interface**: Simple and intuitive command-line interface with flag-based execution.
* **Cross-Platform Compatibility**: Built using C with wide-character (`wchar_t`) support for proper file path and encoding handling.

---

## ⚙️ Command-Line Arguments

| Flag | Description |
| :--- | :--- |
| `-h`, `-?` | Displays the help menu with usage examples |
| `-a` | Displays basic information about the tool |
| `-c` | Compresses the specified files/directories |
| `-d` | Decompresses a `.nzip` archive |
| `-e` | Extracts a specific file from an archive |
| `-o <file>` | Specifies the output file or destination directory |
| `-l` | Toggles verbose logging during execution |

---

## 🚀 Installation & Build

### Prerequisites
* C Compiler (`gcc`, `clang`, or MSVC)
* Windows SDK (for `Windows.h` / `CommandLineToArgvW` on Windows systems)

### Compilation
Using `gcc`:
```bash
gcc -Iinclude src/main.c src/parseFiles.c -o NinjaZip.exe
