# C++ Text RPG  

Welcome to the repository for my TextRPG, a foundational project in C++ development!  

This project is currently **Windows-only**, as it relies on direct Windows API calls for the console, events, input handling, and more. While I’d love to make it cross-platform, I have some more work to do on other things, so that's on the backburner for now.

While a working prototype, this is an ongoing project, and many features are still in development.
⚠ **Important:** The current layout works on my machine but may crash on smaller resolutions. I avoided hardcoded values but some testing still needs to be done 

## 🔧 Build Instructions  
To build the project:  
1. Clone the repository:  
   ```sh
   git clone https://github.com/VladOsip/TextRPG.git
   ```  
2. Navigate into the repo directory and run:  
   ```sh
   cmake -S . -B build
   ```  
3. Build the project:  
   ```sh
   cmake --build . --config Debug   # or use "Release"
   ```  
   - If using MSVC, you can build from the generated `.sln` file.  
   - MSVC creates `Debug/Release` folders when building. The `assets` folder gets copied to `bin`, so you’ll need to move it manually into the `Debug/Release` folders.  

## ✅ Implemented Features  
The following features have been developed so far:  

- **State Machine**  
  - Manages different game states such as `GameState`, `MenuState`, and `TitleState`.  

- **Typewriter Effect**  
  - A simple class that scrolls text based on parameters. This is designed to work with the upcoming `TextState` system.  

- **Item & Equipment Loaders**  
  - Factory-based system for creating items from predefined parameters. Items can also be loaded from XML files.  

- **XML Parser**  
  - A lightweight XML parser using TinyXML2 for reading and loading game data (e.g., items and equipment).  

## 🚀 Planned Features  
Here are some features I plan to implement:  

- **Battle System**  
  - A turn-based combat system for battling various enemies, including a dedicated `BattleState`.  

- **Shops**  
  - A system where players can buy items, weapons, and armor. This is already in development!  

## 💬 Feedback & Contributions  
I’d love to hear your feedback, ideas, and suggestions! This project is a learning experience for me, and something I will strive to improve. 🚀  

