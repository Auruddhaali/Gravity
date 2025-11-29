# How to Build Gravity IDE

Your custom Gravity IDE source code is ready! However, to build the `.exe`, you need to install some prerequisites on your Windows machine.

## 1. Install Prerequisites

The build fails because you are missing the **C++ Build Tools**. Please install:

1.  **Visual Studio 2022 Build Tools**
    *   Download from: [https://visualstudio.microsoft.com/downloads/](https://visualstudio.microsoft.com/downloads/)
    *   Select **"Desktop development with C++"** workload during installation.
2.  **Python 3.x**
    *   Download from: [https://www.python.org/downloads/](https://www.python.org/downloads/)

## 2. Install Dependencies

Once the tools are installed, open a terminal in this directory (`d:\Auro code\Gravity\Gravity`) and run:

```bash
# This usually takes 10-15 minutes and MUST complete without errors
npm install
```

## 3. Build Gravity IDE

After `npm install` succeeds, you can build the application:

### To Run in Development Mode (Fastest)
```bash
.\scripts\code.bat
```

### To Build the .exe Installer
```bash
npm run gulp vscode-win32-x64
```
The output file will be located at: `.build/win32-x64/Gravity.exe`

## 4. Verify Customizations

When you run the app, check:
-   **Title Bar:** Should say "Gravity IDE"
-   **Icon:** Should be your custom Gravity logo
-   **Theme:** Default colors should be Purple (#4f4479)
-   **About Dialog:** Author should be "Auruddha Rushd Ali"
