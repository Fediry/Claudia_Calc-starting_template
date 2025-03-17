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
 * Clone the repo (or download the .zip file, and extract it) to a folder of your choice.
 * Open that folder in VS Code
 * VS Code should pop up a reccomendation to run/open the folder as a devcontainer
   - You may need to add the devcontainer extension to vscode before hand.
   - Once the devcontainer extension is installed, to open the folder as a contianer manually,
     go to the command pallet (ctr+sht+P) and type dev container. This should list several options.
     Choose "Dev Containers: Open Folder in Container...", which should build the container and
     open a new VS Code screen inside that container. **NOTE:** The first time VS Code builds the
     container it may take a long time. Subsequent builds should be much faster.

 * You should be able to build and run claudia_calc.cpp right away. If the error occurs that
   it cannot find spdlog/spdlog.h, hit abort and wait a minute before trying again. VS Code
   has to load the C++ extensions in the container after it's built, and sometimes this takes
   an extra minute or two.
 
