How to set your primary part on characters(humanoidrootpart):

https://github.com/user-attachments/assets/4c68c8bd-4a4f-4f99-aeed-0d1dc9a97184

# Steps
1. Select any character(r6/r15 or others if hrp is in that char)
2. In the APP UI panel, enable `Selection Detector` and enable the `characterEnabled` option.
3. Click on the `Run` button in APP.

# How it works
- Searches for `hrp` or `humanoidrootpart` in any BasePart name of your character(model).
- So even if your BasePart contains hrp with a bunch of other letters, SelectionDetector chooses it as the Primary Part. *Example:* jnnsd`hrp`nnkf or nsnf`hUmanoIdRootPaRt`nnskjd

# Common mistakes
1. No part with hrp in their name was found in your character.
2. Your hrp is spelled incorrectly.
3. `hrp` or `humanoidrootpart` is found in more than 1 name.
