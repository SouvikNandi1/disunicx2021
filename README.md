# DisunicX Browser

![DisunicX Banner](https://user-images.githubusercontent.com/8016567/201476123-1d5337e5-1c3b-492c-8822-a39c9f2b845d.png)

**A modern, open-source, privacy-focused web browser built with Python and PySide6 that leverages the Tor network for enhanced anonymity and security.**

---

## 📖 About The Project

DisunicX is a custom-built web browser designed from the ground up with privacy as its core principle. It integrates seamlessly with the Tor network, routing your traffic through Tor's volunteer-run overlay network to conceal your location and browsing activity from surveillance and traffic analysis.

The entire user interface is crafted using PySide6 (Qt for Python), providing a sleek, modern, and responsive dark-themed experience. It's a testament to what can be achieved with Python in the desktop application space.

### Key Features

*   **🔒 Tor Integration**: Automatically connects to and routes traffic through the Tor network. A status indicator in the status bar keeps you informed of the connection.
*   **✨ Modern UI**: A beautiful, dark-themed interface with custom-drawn, frameless window controls for a clean, modern look.
*   **🌐 Tabbed Browsing**: A familiar and intuitive tabbed browsing experience with movable and closable tabs.
*   **🚀 Custom New Tab Page**: An elegant and functional new tab page featuring a search bar and a minimalist design.
*   **⚙️ Comprehensive Settings**: A dedicated settings page (`disunic://settings`) to manage:
    *   **General**: Configure startup behavior and default search engine (Disunic, DuckDuckGo, Google, etc.).
    *   **Privacy & Security**: Control cookie policies, tracking protection, and set security levels (Standard, Safer, Safest) that manage JavaScript, plugins, and other potentially risky features.
    *   **Advanced**: Toggle Tor network usage, manage hardware acceleration, and set a custom User-Agent.
*   **📥 Integrated Download Manager**: A built-in page (`disunic://downloads`) to manage all your downloads, with support for pausing, resuming, and canceling.
*   **📜 Rich History Page**: A full-featured, searchable history page (`disunic://history`) to easily find pages you've visited.
*   **🔄 Automatic Updates**: The browser automatically checks for new releases on GitHub and prompts you to download the latest version.
*   **🛠️ Developer Tools**: Includes essential developer features like "View Page Source" and "Inspect Element" (opens in a new tab).
*   **➕ Extra Features**:
    *   Save pages directly to PDF.
    *   Create a QR code for the current page URL.
    *   Clear all browsing data with a single click.

### Built With

*   Python
*   PySide6 (The official Python bindings for Qt)
*   Qt WebEngine (Based on the Chromium project)
*   Tor

---

## 🚀 Getting Started

To get a local copy up and running, follow these simple steps.

### Prerequisites

*   **Python 3.8+**
*   **Tor Executable**: The browser requires a `disunic.exe` (your packaged Tor executable) to be present in the root directory of the project.
*   Install the required Python packages.

    ```sh
    pip install -r requirements.txt
    ```

### Installation & Running

1.  **Clone the repository:**
    ```sh
    git clone https://github.com/SouvikNandi1/disunicx2021.git
    ```
2.  **Navigate to the project directory:**
    ```sh
    cd disunicx2021
    ```
3.  **Install dependencies:**
    (Create a `requirements.txt` file with the content below)
    ```txt
    PySide6
    packaging
    qrcode[pil]
    ```
    Then run:
    ```sh
    pip install -r requirements.txt
    ```
4.  **Run the application:**
    ```sh
    python main.py
    ```

---

## 📦 Building from Source

You can create a standalone executable using PyInstaller. This command bundles the application, its dependencies, and the Tor executable into a single distributable file.

Make sure PyInstaller is installed:
```sh
pip install pyinstaller
```

Then, run the build command from the project's root directory:

```sh
pyinstaller --noconsole --windowed --name DisunicX --add-data "disunic.exe;." --hidden-import PySide6.QtSvg --hidden-import PySide6.QtNetwork --hidden-import PySide6.QtWebChannel --hidden-import PySide6.QtWebEngineWidgets main.py
```

The final `DisunicX.exe` will be located in the `dist/DisunicX` folder.

---

## ⚠️ Disclaimer

DisunicX is an open-source project created for educational and privacy-awareness purposes. The developer, Souvik Nandi, is not responsible for any illegal, harmful, or unethical activities performed using this browser. You use this software at your own risk.

---

## 📄 License

This project is open source. Please add a license file (e.g., MIT, GPL) to define the terms under which it can be used, modified, and distributed.

---

## 📬 Contact

Souvik Nandi - @SouvikNandi1

Project Link: https://github.com/SouvikNandi1/disunicx2021