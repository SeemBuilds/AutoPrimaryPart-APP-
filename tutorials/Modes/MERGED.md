How to use the operation `MERGED`:

https://github.com/user-attachments/assets/af984867-7757-451f-8a5f-e1f8afe8ea09

# Steps
1. Select the `MERGED` mode in the APP UI. 
2. Select any model or tool.
3. Click on the `Run` button in APP.

# How it works
- Creates a BoundingBox part as the PrimaryPart for only the first selected model/tool, based on all contained BaseParts of all selected models/tools.
- The BoundingBox is a `fully transparent` part, with `CanCollide`, `CanTouch`, `CanQuery` disabled.
- The BoundingBox is named `PrimaryPart` + GUID.

# Common mistakes
1. *None*
