## RustDecompress - ZIP File Decompression Tool

### Introduction
This project is a ZIP file decompression tool written in Rust. The program supports reading ZIP files from the command line and extracting their contents, including file and directory structures. It preserves file permissions on Unix systems and provides basic file comment information output. The tool is designed to be simple and efficient, utilizing the `zip` crate for ZIP file handling and the Rust standard library for file operations.
### Features
- Extracts all files and directories from a ZIP file.
- Supports file permission settings on Unix systems.
- Displays file comments if available.
- Automatically creates necessary parent directories.

### Usage
1. Build the project:
   ```bash
   cargo build --release
   ```
2. Run the program:
   ```bash
   ./target/release/rust-decompress <filename.zip>
   ```
   - Replace `<filename.zip>` with the target ZIP file path.
   - Example: `./target/release/rust-decompress example.zip`

### Code Structure
- `main.rs`: Contains the main program logic, using the `zip` crate for ZIP file decompression.
- `.gitignore`: Ignores the `1/` folder and `1.zip` file.

### Dependencies
- `zip`: Used for handling ZIP files.
- Standard library (`std::fs`, `std::io`) for file operations.

### Notes
- Ensure the input ZIP file path is valid.
- The current code uses `unwrap()` for error handling; consider adding robust error handling for production use.
- The `1/` folder and `1.zip` file are ignored to avoid unnecessary commits.

### Contribution
Feel free to submit issues or pull requests to improve the project.

---

## RustDecompress - ZIP 文件解压工具

### 介绍
本项目是一个使用 Rust 语言编写的 ZIP 文件解压工具。程序支持从命令行读取 ZIP 文件并解压其中的内容，包括文件和目录结构。它在 Unix 系统上保留文件权限，并提供基本的文件注释信息输出。该工具设计简单高效，利用 `zip` crate 处理 ZIP 文件，并使用 Rust 标准库进行文件操作。
- 解压 ZIP 文件中的所有文件和目录。
- 支持 Unix 系统下的文件权限设置。
- 显示文件注释（如果存在）。
- 自动创建必要的父目录。

### 使用方法
1. 编译项目：
   ```bash
   cargo build --release
   ```
2. 运行程序：
   ```bash
   ./target/release/rust-decompress <filename.zip>
   ```
   - 将 `<filename.zip>` 替换为目标 ZIP 文件路径。
   - 示例：`./target/release/rust-decompress example.zip`

### 代码结构
- `main.rs`：包含主程序逻辑，使用 `zip` crate 处理 ZIP 文件解压。
- `.gitignore`：忽略 `1/` 文件夹和 `1.zip` 文件。

### 依赖
- `zip`：用于处理 ZIP 文件。
- 标准库 (`std::fs`, `std::io`) 用于文件操作。


