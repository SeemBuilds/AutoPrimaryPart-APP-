How to use the operation `MULTIMERGED`:

https://github.com/user-attachments/assets/79de0069-80d5-4338-a619-9fb8b36d656c

# Steps
1. Select the `MULTIMERGED` mode in the APP UI. 
2. Select any model or tool.
3. Click on the `Run` button in APP.

# How it works
- Creates a BoundingBox part as the PrimaryPart for all selected models/tools, based on all contained BaseParts of all selected models/tools.
- The BoundingBox is a `fully transparent` part, with `CanCollide`, `CanTouch`, `CanQuery` disabled.
- The BoundingBox is named `PrimaryPart` + GUID.

# Common mistakes
1. *None*
