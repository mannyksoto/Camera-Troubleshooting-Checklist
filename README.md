# Camera-Troubleshooting-Checklist

CAMERA TROUBLESHOOTING CHECKLIST (GUI) - SETUP & USE
======================================================

WHAT'S IN THIS FOLDER
----------------------
- camera_troubleshooter_gui.py   The app itself. Do not rename or move
                                  it out of this folder.
- run_checklist.bat              Double-click this to launch the app.
- README.txt                     This file.

ONE-TIME SETUP (each laptop, only needs to be done once)
----------------------------------------------------------
This app runs on Python, which is not installed on Windows by default.

1. Go to https://www.python.org/downloads/
2. Click the yellow "Download Python" button.
3. Run the installer.
4. On the FIRST screen of the installer, check the box at the bottom
   that says "Add python.exe to PATH" -- this step matters, don't
   skip it. Leave "tcl/tk and IDLE" checked too (it's on by default)
   -- that's what draws the app's window.
5. Click "Install Now" and let it finish.

That's it. The first time you run the app afterward, the launcher
will automatically install one more small piece it needs (for saving
Word reports) -- that happens on its own, no action needed from you.

RUNNING THE APP
------------------
1. Copy this whole folder (all 3 files together) onto the laptop --
   USB drive, email attachment, shared drive, however's easiest.
2. Double-click "run_checklist.bat".
3. A window opens:
     - Enter the site name and your name, click Start.
     - Add a camera by name/location and IP address, click
       "Run Automated Checks" -- it pings the camera, checks common
       ports, and checks the web UI, live in the window.
     - If it finds issues (or you just want to), run the guided
       manual checklist -- one question at a time, Pass / Fail / Skip,
       with an optional note.
     - Add a resolution note, then either add the next camera or
       finish the session.
     - On the summary screen, export the full report as a plain text
       file and/or a Word (.docx) document -- pick where to save it.
4. Saved text reports also land automatically in a "reports" folder
   that appears inside this same folder.

If double-clicking the .bat file does nothing or closes instantly,
right-click it and choose "Run as administrator", or open a Command
Prompt, cd to this folder, and type: python camera_troubleshooter_gui.py
-- that will show any error message that flashed by too fast to read.

UPDATING THE APP LATER
--------------------------
If the app gets improved (new checks, new checklist items), you'll
just get a new camera_troubleshooter_gui.py to drop into this same
folder, replacing the old one. Nothing else needs to change or be
reinstalled.
