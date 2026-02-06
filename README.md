# HashTool – High-Performance Windows File Hash Verification Tool (MD5 / SHA256)

[中文说明](README_CN.md)

HashTool is a high-performance **Windows file hash verification tool** built with **VB.NET and WPF**. 
It supports **MD5 and SHA256** and is designed for **batch and parallel file hash calculation**, 
helping users quickly verify **file integrity** even when processing large numbers of files.

## ✨ Features

- Supports **file hash verification** (no text hashing)
- Supports **MD5** and **SHA256** algorithms
- Supports **drag-and-drop** file input
- Supports **batch file hash calculation**
- Supports **parallel verification of multiple files**, fully utilizing multi-core CPUs to greatly improve performance in large-scale file scenarios
- Automatically matches the number of worker threads based on the system **CPU core count**
- Allows users to **manually adjust thread count** for flexible performance and resource control
- Supports **exporting verification results** for saving and further comparison
- Supports **one-click copying of results** for quick reuse
- Clean and intuitive WPF-based user interface
- Native Windows desktop application experience

## 💡 Use Cases

- Verifying file integrity after large downloads
- Batch hash verification for backup files
- Checking file consistency during file distribution
- High-speed hash calculation for large numbers of files

## 🖼️ Screenshot

![HashTool UI – Parallel File Hash Verification](screenshot.png)

## 🛠️ Tech Stack

- **Language**: VB.NET
- **Framework**: WPF (.NET)
- **UI**: XAML
- **Platform**: Windows

## 📂 Project Structure

```text
├── MainWindow.xaml              # Main window UI
├── MainWindow.xaml.vb           # Main window logic
├── HashToolControl.xaml         # Hash tool control UI
├── HashToolControl.xaml.vb      # Hash tool control logic
├── DwmHelper.vb                 # Windows DWM helper
├── NativeMethods.vb             # Win32 API wrappers
└── README.md / README_CN.md     # Project documentation
```

## 🚀 Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/luoji12/HashTool.git
```

### 2. Open the project in Visual Studio

- Visual Studio 2019 or later is recommended
- Make sure the .NET desktop development workload is installed

### 3. Build and Run

- Build the solution and run the application
- Add files via **file selection** or **drag-and-drop**
- Multiple files can be added at once and will be processed in batch
- All MD5 / SHA256 hashes are calculated **in parallel**
- The application automatically selects an appropriate thread count based on your CPU, with optional manual adjustment
- Verification results can be **exported** or **copied directly** for further use

## 📌 Requirements

- Windows 10 / 11
- .NET Framework or .NET (as defined by the project)
- Visual Studio (for development)

## 📖 Possible Enhancements

You may further extend this project by:

- Adding more hash algorithms (SHA1, SHA512, etc.)
- Customizing result export formats (e.g. JSON, extended CSV)
- Automatic result comparison and highlighting
- Dark mode / theme customization
- Multilingual UI support

## 🤝 Contributing

Contributions are welcome!

- Feel free to open Issues for bug reports or feature requests
- Pull Requests are appreciated

## 📄 License

This project is licensed under the **MIT License**.

---

If you find this project useful, consider giving it a ⭐ on GitHub!


Keywords: file hash, file verification, MD5, SHA256, Windows hash tool, parallel hash
