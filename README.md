R6 Recoil Controller

  
    
  
  
    
  
  
    
  



  R6 Recoil Controller is a powerful and customizable tool designed to enhance your gameplay experience in Rainbow Six Siege by providing precise recoil control and operator-specific preset management. Built with Python and CustomTkinter, it offers an intuitive GUI, real-time overlay, and automatic operator detection to help you dominate the battlefield with ease.



⚠️ Important Notice
R6 Recoil Controller is intended for personal use and testing in non-competitive environments. Ensure compliance with the terms of service of Rainbow Six Siege and Ubisoft's policies. This tool is not intended to provide unfair advantages or violate game rules. Use responsibly and at your own discretion. Always check for the latest updates and compatibility with game patches.

⚙️ Installation
R6 Recoil Controller requires Python 3.8 or higher and specific dependencies to run. Follow these steps to set up the project on your system:

Install Python: Download and install Python from the official Python website. Ensure you add Python to your PATH during installation.

Clone the Repository:
git clone https://github.com/Yarouki/R6-Recoil.git
cd R6-Recoil


Set Up a Virtual Environment (recommended):
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate


Install Dependencies:
pip install -r requirements.txt

Ensure you have the following dependencies installed (listed in requirements.txt):

customtkinter
pillow
pynput
opencv-python
numpy
pytesseract
pywin32
requests
packaging


Install Tesseract OCR:

Download and install Tesseract from GitHub.
Add Tesseract to your system PATH (e.g., C:\Program Files\Tesseract-OCR\tesseract.exe on Windows).
Update the pytesseract configuration in recoil_handler.py if necessary.


Run the Application:
python main.py




⚡️ Quickstart
Get started with R6 Recoil Controller in just a few steps. The following example demonstrates how to launch the application and configure a preset for an operator in Rainbow Six Siege.

Launch the Application:Run python main.py to open the GUI. The main window displays operator presets organized into Attackers, Defenders, and Favorites categories.

Select an Operator:Click on an operator button (e.g., "Ash" or "Jäger") to activate their recoil preset. The status bar will update to show the active preset and scope.

Toggle Recoil Control:Use the configured hotkey (default: caps_lock) to toggle the recoil control system on or off. The overlay will display the current status ("Running" or "Paused").

Customize Presets:Click "Edit Preset" to adjust recoil settings (X/Y strength, rapid fire delay) for the selected operator and scope (1x or 2.5x).

Enable Auto-Detection (optional):In the Settings menu, enable auto-detection and set a hotkey (default: f1). The program will use OCR to detect the active operator in-game and apply the corresponding preset.



🎯 Features

Intuitive GUI: Built with CustomTkinter for a sleek, dark-themed interface that's easy to navigate.
Operator-Specific Presets: Customize recoil settings for each operator, with support for 1x and 2.5x scopes.
Real-Time Overlay: Displays the active preset, scope, and status (Running/Paused) directly on your game window.
Automatic Operator Detection: Uses OCR to detect the active operator in-game and switch presets automatically.
Favorites System: Pin your favorite operators for quick access.
Custom Presets: Create and manage custom presets with adjustable recoil strength and rapid fire settings.
High Sensitivity Mode: Fine-tune mouse movement for high-DPI setups.
Hotkey Support: Toggle recoil control and auto-detection with customizable hotkeys.
Auto-Update System: Checks for updates and downloads the latest version seamlessly.
Cross-Platform Compatibility: Designed for Windows, with potential for future Linux support (Tesseract OCR required).


💡 Philosophy
R6 Recoil Controller was created to empower Rainbow Six Siege players with precise control over weapon recoil, making gameplay more enjoyable and accessible. Whether you're a casual player or a competitive enthusiast, this tool simplifies recoil management with an intuitive interface and powerful automation features. Inspired by the need for customization, it allows players to tailor settings to their playstyle while maintaining a lightweight and efficient design.
We aim to provide a user-friendly, customizable, and reliable tool that integrates seamlessly with your gaming setup. Our goal is to enhance your experience without compromising fairness or game integrity.

⚠️ Limitations

Windows Only: Currently designed for Windows due to dependencies on pywin32 and Windows API for overlay functionality. Linux support may be added in the future.
Game Compatibility: Requires regular updates to maintain compatibility with Rainbow Six Siege patches.
OCR Accuracy: Automatic operator detection relies on Tesseract OCR, which may occasionally misread text in certain lighting or resolution conditions.
Game Rules: Users are responsible for ensuring compliance with Ubisoft's terms of service to avoid potential bans.


👀 Examples
Below are examples of how to use R6 Recoil Controller's core features. For more detailed guides, check our Wiki.
📖 Selecting a Preset

Open the application (python main.py).
In the main window, click an operator (e.g., "Sledge") under the "Attackers" category.
The status bar updates to show "Running | Sledge 1x" (assuming 1x scope is selected).
Press the toggle hotkey (caps_lock) to enable recoil control in-game.

📖 Editing a Preset

Select an operator (e.g., "Jäger").
Click "Edit Preset" to open the preset editor.
Adjust the X/Y recoil strength sliders (e.g., X: -2.0, Y: 10.0) for the 1x scope.
Enable rapid fire and set a delay (e.g., 100ms).
Save changes, and the preset is updated for in-game use.

📖 Adding to Favorites

Right-click an operator (e.g., "Ash") in the "Attackers" category.
Select "Add to Favorites" from the context menu.
Ash appears in the "Favorites Attackers" section for quick access.

📖 Enabling Auto-Detection

Go to Settings and enable "Auto-Detect" with the toggle switch.
Set the auto-detect hotkey (e.g., f1).
In-game, press f1 to trigger OCR detection. The program will switch to the detected operator's preset.

📖 Creating a Custom Preset

Click "New Preset" in the main window.
Enter a preset name (e.g., "Custom Ash") and select a category (e.g., "Attackers").
Optionally, select a custom icon (.png file).
Save the preset, and it appears in the selected category with default settings.


🧬 Dependencies
R6 Recoil Controller relies on the following Python libraries and external tools:



Dependency
Description



customtkinter
Provides the modern, dark-themed GUI for the application.


pillow
Handles image processing for operator icons.


pynput
Captures mouse and keyboard inputs for hotkey and recoil control.


opencv-python
Processes screenshots for operator detection using OCR.


numpy
Supports image processing for OCR functionality.


pytesseract
Performs OCR to detect in-game operator names.


pywin32
Manages Windows API calls for overlay and mouse control.


requests
Handles HTTP requests for checking and downloading updates.


packaging
Compares version numbers for the update system.


Tesseract OCR
External tool required for text recognition in auto-detection.


Install dependencies with:
pip install customtkinter pillow pynput opencv-python numpy pytesseract pywin32 requests packaging


👍 Contribute
We welcome contributions to make R6 Recoil Controller even better! To contribute:

Star the Repository: Show your support by adding a GitHub Star.
Report Issues: Found a bug? Report it on the Issues page.
Submit Pull Requests: Add features, fix bugs, or improve documentation.
Share Feedback: Join our Discord community or tweet about the project on X.
Write Tutorials: Share your experience on Medium, Dev.to, or your blog.
Support the Project: Buy us a cup of coffee to keep development going.

To ensure code quality, run the following commands before submitting a pull request:

Linting: pylint *.py
Formatting: black .
Testing: pytest (if tests are added in the future)


☕ Supporters
R6 Recoil Controller is an open-source project maintained through community support. If you’d like to help keep the project alive, consider buying a cup of coffee.



User
Donation



Your supporters here
☕ x N



💻 Code Contributors
Contributions from the community make R6 Recoil Controller possible. Thank you to all contributors!

Contributors will be listed here as the project grows.

⭐️ Stargazers
Your support means the world to us! Star the repository to show your appreciation and help spread the word.

Stargazer chart will be added as the project gains traction.

🧾 License
Copyright (c) 2025 Yarouki and Contributors. R6 Recoil Controller is free and open-source software licensed under the MIT License.
