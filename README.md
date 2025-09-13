***This Documentation is in progress***

# AutoPrimaryPart(APP)
The official AutoPrimaryPart Documentation!

![Version](https://img.shields.io/badge/version-0.1.0--beta-blue)
![Status](https://img.shields.io/badge/status-Public-orange)

## Documentation: 
APP is a Roblox Studio Plugin that lets you automatically set your Model's PrimaryPart after your liking, offering a variety of modes, but also having the ability to detect your Selection and setting the perfect PrimaryPart!

*This Documentation includes the following topics:*

## 📚 Content
- [Installation](#installation)
- [Features](#features)
- [Settings](#Settings)
- [Usage](#usage)
- [Data Usage](#Data_Usage)
- [Contributing](#contributing)
- [Upcoming Updates](#UpcomingUpdates)


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
   
[For Usage, view: Usage]


## Usage
To use APP, you must have installed it!
After that, click on the Plugin Tab, select APP and click the UI button.

In the panel, close every window. This will make it easier to see everything at a glance.

   - **Select Mode Window**
     
        - In this window, you can select a variety of modes, each one having a unique ability to set your PrimaryPart.
        - Just click near the circle to select or change modes:
        - ![SelectingAMode_Tutorial](https://github.com/user-attachments/assets/8f5b5f63-606a-4abd-9821-61d6b998f957)
        - Each Mode's features are listed [here](#features)
          
   - **SelectionDetector**
        - SelectionDetector automatically detects your selection after looking for specific parts and names.
        - *Example:* You have selected a building that contains parts with “Wall” in their names: Your Selection is likely a building(just a rough example)!
        - By opening the `Customize Detection` panel in `Selection Detector`, you can customize what should be detected or not. This may be important if your model includes names or parts, that are also relevant for another Detection.
        -  *Example:* If you have a character selected, but for some reason it includes parts with "Wall" found in their names, SelectionDetector could specify your Selection as a house and not as character!

   - **User Info**
     - DATA COLLECTION IS CURRENTLY DISABLED, AS THIS FEATURE IS NOT FULLY DEVELOPED.
     - USERS WILL BE NOTIFIED BEFORE ANY DATA IS COLLECTED.
     - See: [DATA_USAGE.md](./DATA_USAGE.md)
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
- **Selection Detector**
     - *Enabled:* Whether SelectionDetector should overall be used or not.
          - *Customize Detection(panel):
             - *character:* Whether SelectionDetector should detect characters.
             - *vehicle:* Whether SelectionDetector should detect vehicles.
             - *airplane:* Whether SelectionDetector should detect airplanes.
             - *house:* Whether SelectionDetector should detect house/buildings.
             - *tree:* Whether SelectionDetector should detect trees.
             - *gun:* Whether SelectionDetector should detect guns.
- **User Info**
     - *None*

## Data_Usage
APP collects only minimal technical identifiers and statistics necessary for its functionality.

For details about what data APP stores and how it is used, please read:  
➡️ [DATA_USAGE.md](./DATA_USAGE.md)

- DATA COLLECTION IS CURRENTLY DISABLED, AS THIS FEATURE IS NOT FULLY DEVELOPED.
- USERS WILL BE NOTIFIED BEFORE ANY DATA IS COLLECTED.


## Contributing
Interested in contributing? Great! Please read the guidelines here:  
➡️ [CONTRIBUTION.md](./CONTRIBUTION.md)


## UpcomingUpdates
- Settings for LiveAPP
- Advanced SelectionDetector
- Debugging Panel
- User info Output for Data_Usage(shows certain Data being used)
- APP Output(e.g why certain primary parts were chosen and much more)
