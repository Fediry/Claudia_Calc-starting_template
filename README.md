# Claudia_Calc-CPP_DevContainer
 Basic starting template including the devcontainer, Dockerfile, spdlog, and claudia_calc example files.

## Based on CPP_DevContainer_Template
 Basic Template to start coding in C++ in VS Code
 
 Credit to Chris Pirz for the original Docker file.
 https://github.com/ChristopherPisz/DevEnvCpp

## Requirements:
 * VS Code
 * Docker (or Docker-Desktop)
 * Docker extension on VS Code
 * Dev Containers extension on VS Code

## Installation:
 * Make a new git repository/ project folder for where you want to keep your work.
 * In a temporary folder (like Downloads or Desktop) clone this repo(or download the .zip file, and extract it).
 * Copy the .vscode, .devcontainer, and src folders into your project folder.
 * Open your project folder in VS Code...
   - VS Code should pop up a reccomendation to run/open the folder as a devcontainer
   - You may need to add the devcontainer and Docker extensions to vscode before hand.
   - Once the devcontainer extension is installed, to open the folder as a contianer manually,
     go to the command pallet (ctr+sht+P) and type dev container. This should list several options.
     Choose "Dev Containers: Open Folder in Container...", which should build the container and
     open a new VS Code screen inside that container. **NOTE:** The first time VS Code builds the
     container it may take a long time. Subsequent builds should be much faster.
 * You should be able to build and run claudia_calc.cpp right away. If the error occurs that
   it cannot find spdlog/spdlog.h, hit abort and wait a minute before trying again. VS Code
   has to load the C++ extensions in the container after it's built, and sometimes this takes
   an extra minute or two.
 
## Warning:
 VS Code's Dev Containers should preserve your work in the container in a volume it sets up automatically,
 however if something goes wrong with the contianer or volume, you may lose any work you've done. So commit
 to github often!
