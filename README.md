# Aim:
To use UiPath to automate the process of opening Notepad, typing text, applying basic keyboard shortcuts (Select All, Copy, Paste), and simulating human-like interactions with the desktop application.

# Software Required:
```
1.UiPath Studio (with UiPath.UIAutomation.Activities package).
2.Notepad.
```

# Procedure:
# 1.Start Process to Open Notepad:
   a.Drag Start Process activity into the workflow.
   b.In the FileName property, enter "notepad.exe".
   c.This will open Notepad.
# 2.Type Text Using Type Into:
   a.Drag Type Into activity after the Start Process activity.
   b.Use Indicate on Screen to select the Notepad window.
   c.In the Text property, enter the text to be typed, such as:
         "Hello, this is a keyboard automation made by UiPath studio."
   d.This will type the specified text and simulate the Enter key to create a new line.
# 3.Add a Delay (Optional):
    a.Drag Delay activity to the workflow after the Type Into activity.
    b.Set the Duration property to "00:00:02" (2 seconds).
    c.This will add a short pause to ensure typing is completed before moving to the next action.
# 4.Send Hotkey to Simulate Keyboard Shortcuts:
   a.To Select All text, drag Send Hotkey activity:
       Set Key to "a".
       Set Modifier to "ctrl" (Ctrl + A).
   b.To Copy the selected text, drag another Send Hotkey activity:
       Set Key to "c".
       Set Modifier to "ctrl" (Ctrl + C).
  c.To Paste the copied text, drag another Send Hotkey activity:
       Set Key to "v".
       Set Modifier to "ctrl" (Ctrl + V).

## Workflow:
![Screenshot 2025-05-12 091028](https://github.com/user-attachments/assets/be4f5fbc-10b4-4a29-9d64-0f9e3727ff31)
![Screenshot 2025-05-12 091046](https://github.com/user-attachments/assets/982cd0f0-48e6-4fc6-92f3-762bff284147)
![Screenshot 2025-05-12 091052](https://github.com/user-attachments/assets/7c202503-a3d9-456b-9bbb-900f5a72671d)


# Output:
![Screenshot 2025-05-12 092941](https://github.com/user-attachments/assets/21dffeb9-cbfb-4067-b2cc-ce4487b586b6)

# Result:
Notepad opens automatically, the text is typed and line-breaked, then selected (Ctrl + A), copied (Ctrl + C), and pasted (Ctrl + V) — all automated to simulate human interaction using UiPath.




