🤖 NEOMATIC AI: AI Browser Automation Tool

NEOMATIC AI is a proprietary, powerful desktop application that runs a web server (Gradio) to combine live browser automation (Selenium) with advanced Large Language Model (LLM) planning. It allows users to execute complex, multi-step web tasks using simple, natural language commands.

It is packaged as a single, portable executable for Windows users.

⚠️ Important Download Notice

The full application executable (NEOMATIC AI.exe) is too large for GitHub. The application must be downloaded and run locally.

⬇️ Download the Latest Release

[INSERT YOUR GOOGLE DRIVE / DROPBOX DOWNLOAD LINK HERE]

Requires Windows 10/11 and the Chrome browser installed.

✨ Key Features

Feature

Description

🧠 LLM Planning

Converts natural language commands (e.g., "search headphones and show cheapest") into a precise, executable sequence of Selenium actions.

🎥 Live Visual Feedback

Provides a real-time stream of the automated browser instance (Chrome) within the Gradio interface.

🖱️ Direct Interaction

Users can click anywhere on the live video feed to execute an instant, direct click on the browser element at those coordinates.

⏯️ Media Control

Dedicated ⏯️ Media Play/Pause button to toggle playback of video or audio elements on sites like YouTube or Spotify.

🔗 Smart Navigation

Uses precise methods to locate and click specific links, including video thumbnails, based on the text title provided by the user.

📊 Universal Search

Locates and uses search bars on any website (Google, Amazon, YouTube, etc.) to perform queries.

⚙️ Single File Executable

Built with PyInstaller (--onefile) for easy distribution—no Python installation or setup required for the end user.

🚀 How to Use

The application runs as a local web server (using the Gradio framework) accessible via your default browser.

Prerequisites

Operating System: Windows 10/11 (The .exe is platform-specific).

Web Browser: Google Chrome must be installed on your machine.

Launching the Application

Download and unzip the compressed file containing NEOMATIC AI.exe.

Double-click NEOMATIC AI.exe.

Wait a few seconds for the application to unpack and launch the browser interface.

In the opened browser window, click the 🚀 Start button to launch the automated Chrome instance.

Command Examples

Goal

Command to Enter

Video Playback

open youtube, search royal oak by lithe and click on royal oak

Form Entry

go to gmail and enter test@example.com

E-commerce Filter

search headphones on Amazon and show cheapest

Hyperlink Click

click link titled Documentation

Interface Control

scroll down or click the ⏯️ Media Play/Pause button.

🏗️ Development & Rebuilding

This section is for developers interested in contributing or modifying the source code.

Dependencies

This project relies on the following libraries (you should create a requirements.txt listing these):

gradio

selenium

requests

Pillow (PIL)

webdriver-manager

Rebuilding the Executable

To rebuild the single-file Windows executable after making changes, ensure you are in the project root directory and run:

# 1. Clean previous build files
git rm -r --cached dist build
git clean -fd

# 2. Run the build command
pyinstaller --onefile --name "NEOMATIC AI" --icon="iconimg.ico" --collect-all gradio --collect-all gradio_client --collect-all safehttpx --collect-all groovy --hidden-import=selenium AI_BROWSER_AUTOMATION.py


⚖️ License and Copyright

Copyright (c) 2025 CHAITANYA PATEL. All rights reserved.

This project is licensed under the GNU Affero General Public License Version 3 (AGPLv3).

The AGPLv3 is a strong copyleft license. It means:

You are free to view, modify, and distribute the source code.

If you deploy this software over a network (i.e., run it on a server for others to access, as in the server-client model), you MUST provide the modified source code under the same AGPLv3 terms.

The primary intention is to prevent proprietary, closed-source usage of modified versions.

Please see the accompanying LICENSE file for full details.
