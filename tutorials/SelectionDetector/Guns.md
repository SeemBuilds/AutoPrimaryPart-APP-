How to set your primary part on weapons(tools or models):

https://github.com/user-attachments/assets/33dbcebe-ab6e-40d8-88fb-a4de787d9ccd

# Steps
1. Select any weapon(guns, swords etc: tools or models)
2. In the APP UI panel, enable `Selection Detector` and enable the `gunEnabled` option.
3. Click on the `Run` button in APP.

# How it works
- Searches for "handle" in all BasePart names of your weapon that are converted to lower case internally, i.e. in APP scripts.
- So even if your BasePart name contains "handle" with a bunch of other letters or "handle" is written with upper and lower case letters., the HANDLE mode sets it as the Primary Part. *Example*: jnnsdhandlennkf or nsnfHhAnDlennskjd

# Common mistakes
1. No BaseParts with “handle” in the name were found in your character.
2. Your handle is spelled incorrectly.
3. `handle` is found in more than 1 name(can lead to undesirable results).
