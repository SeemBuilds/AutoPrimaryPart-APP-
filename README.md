# AutoPrimaryPart(APP)
The official AutoPrimaryPart Documentation!

![Version](https://img.shields.io/badge/version-0.1.0--beta-blue)
![Status](https://img.shields.io/badge/status-Public-orange)
![Docs](https://img.shields.io/badge/docs-in%20progress-yellow)

APP(AutoPrimaryPart) is a Roblox Studio Plugin that lets you automatically set your Model's PrimaryPart after your liking, offering a variety of modes, but also having the ability to detect your Selection and setting the perfect PrimaryPart!

*This Documentation includes the following topics:*

## 📚 Content
- [Installation](#installation)
- [Usage](#usage)
- [Features](#features)
- [Settings](#Settings)
- [Versioning](#Versioning)
- [Data Usage](#Data-Usage)
- [Contributing](#contributing)
- [Upcoming Updates](#Upcoming-Updates)


## Installation
[➡️ Install AutoPrimaryPart](https://create.roblox.com/store/asset/122023934560086/AutoPrimaryPart)

 or:
1. Open Roblox Studio
2. In the Topbar, select the view panel
3. Click on toolbox
4. In the toolbox, change from Models to Plugins
5. In the Searchbar, search for *AutoPrimaryPart*
6. Select install!
7. Done✅



## Usage
Click on the Plugin Tab, select APP and click the UI button.

In the panel, close every window. This will make it easier to see everything at a glance.
![ClosingEveryWindow](https://github.com/user-attachments/assets/9140ac1b-fd66-49e9-9b1e-41df61918b7d)


   - **Select Mode Window**
     
        - In this window, you can select a variety of modes, each one having a unique ability to set your PrimaryPart.
        - Just click near the circle to select or change modes:
        - ![SelectingAMode_Tutorial](https://github.com/user-attachments/assets/8f5b5f63-606a-4abd-9821-61d6b998f957)
        - Each Mode's features are listed [here](#features)
          
   - **SelectionDetector**
        - SelectionDetector automatically detects your selection after looking for specific parts and names.
        - *Example:* You have selected a building that contains parts with “Wall” in their names: Your Selection is likely a building(just a rough example)!
        - By opening the `Customize Detection` panel in `Selection Detector`, you can customize what should be detected or not. This may be important if your model includes names or parts, that are also relevant for another Detection.
        -  *Example:* If you have a character selected, but for some reason it contains parts with ‘Wall’ in their names, SelectionDetector might incorrectly identify it as a house.
        -  ***To enable SelectionDetector, simply click on the checkbox:***
        -  ![EnablingSelectionDetector](https://github.com/user-attachments/assets/f1401d56-101f-4a50-9480-048c13dfd2e9)

   - **User Info**
     - DATA COLLECTION IS CURRENTLY DISABLED, AS THIS FEATURE IS NOT FULLY DEVELOPED.
     - USERS WILL BE NOTIFIED BEFORE ANY DATA IS COLLECTED.
     - Read: [DATA_USAGE](./DATA_USAGE.md)
## Features
Each Mode has its own ability to make a PrimaryPart for your model. The features are listed here: 

- **SET**:
This Mode gets the closest part to the middle of your whole model and sets it as the Model's PrimaryPart.

- **ADD**:
Gets the BoundingBox of your model and sets it as the Model's PrimaryPart.

- **BIGGEST**:
Gets the biggest(Volume) part in your model and sets it as the Model's PrimaryPart.

- **SMALLEST**:
Gets the smallest(Volume) part in your model and sets it as the Model's PrimaryPart.

- **HIGHEST**:
Gets the highest part on the Y-Axis(world orientation) in your model and sets it as the PrimaryPart of the model.

- **LOWEST**:
Gets the lowest part on the Y-Axis(world orientation) in your model and sets it as the PrimaryPart of the model.

- **RANDOM**:
Gets a random part in your model and sets it as the Model's PrimaryPart.

- **HANDLE**:
Searches specifically for a part whose name contains a “handle” and sets it as the PrimaryPart of the model.

- **MERGED**:
Creates a BoundingBox part as the PrimaryPart for only the first selected model, based on all contained parts.

- **MULTIMERGED**:
Same purpose as MERGED, but sets the PrimaryPart for all selected models.


## Settings
These are the Settings APP offers in each panel:
- **Select Mode**
     - *LiveAPP:* Automatically sets PrimaryPart for Models inserted in Workspace based on the Settings and Mode you have selected in the APP UI.
- **Selection Detector**(also works with *LiveAPP*)
     - *Enabled:* Whether SelectionDetector should overall be used or not.
          - *Customize Detection(panel):*
             - *character:* Whether SelectionDetector should detect characters.
             - *vehicle:* Whether SelectionDetector should detect vehicles.
             - *airplane:* Whether SelectionDetector should detect airplanes.
             - *house:* Whether SelectionDetector should detect house/buildings.
             - *tree:* Whether SelectionDetector should detect trees.
             - *gun:* Whether SelectionDetector should detect guns.
- **User Info**
     - *None*

 ## Versioning
Sometimes APP updates can result in certain modes and options being changed. Versioning is used to retain the desired options and modes after version requests. In APP there is a Versioning panel, with a Versioning TextBox. There you can enter your desired version. This version will now always be used for you, unless you change it.  Please note that if you enter an incorrect or empty version, the version will be loaded to the latest version.

How to revert to any version:
1. in this Github repo, navigate to releases.
There you will find every version of APP.
2. click on your desired version.
You will see a JSON code.
3. copy the value of “version”.
4. in the APP plugin in Roblox studio, under Versioning, paste the copied value into the TextBox.
5. done!

## Data Usage
APP collects only minimal technical identifiers and statistics necessary for its functionality.

For details about what data APP stores and how it is used, please read:  
➡️ [DATA_USAGE](./DATA_USAGE.md)

- DATA COLLECTION IS CURRENTLY DISABLED, AS THIS FEATURE IS NOT FULLY DEVELOPED.
- USERS WILL BE NOTIFIED BEFORE ANY DATA IS COLLECTED.


## Contributing
Interested in contributing? Great! Please read the guidelines here:  
➡️ [CONTRIBUTION](./CONTRIBUTION.md)


## Upcoming Updates
- Settings for LiveAPP
- Advanced SelectionDetector
- Debugging Panel
- User info Output for Data_Usage(shows certain Data being used)
- APP Output(e.g why certain primary parts were chosen and much more)
- Performance optimization
