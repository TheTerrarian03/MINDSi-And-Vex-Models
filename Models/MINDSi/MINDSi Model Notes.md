# MINDS-I Model Notes

Welcome to the notes for the MINDS-I models! This is an overview of what's in these folders, and notes on how to access, edit, or use them.

## Table of Contents
- [`Folder Contents`](#folder-contents): Outline of what's in the folders and subfolders here
- [`How to use the models`](#how-to-use-the-models): How to use the models for printing
- [`How to edit or tune the models`](#how-to-edit-or-tune-the-models): What to do if you need to adjust the models to fit or work
  - [`Hardware`](#hardware)
  - [`Software`](#software)
  - [`Tuning and Editing`](#tuning-and-editing)

-----

## Folder Contents:

- [`Beams`](./Beams/): A folder of models for the straight Beams
  - [`Original Dimensions`](./Beams/Original%20Dimensions/): pre-made models for beams from original, OEM, dimensions
  - (you may add other folders here with models made custom for your printers)
- [`45-Beams`](./45-Beams/): A folder of models for the diagonal Beams
  - -- tbd --
- [`Project Files`](./Project%20Files/): A folder with save-files for the models. More on these in [`Tuning and Editing`](#tuning-and-editing)

-----

## How to use the models:

So you found a model you want to print, or you're desperate to print one to fix your robot? Great!

In general, 3d printing a model is pretty easy- almost drag-and-drop.
- Requirement 1: Slicing software
  - The slicing software takes the 3d models and turns them into printer-readable code to run.
  - You may need to download software like PrusaSlicer, Cura, or others, depending on printer and what Mr. U recommends.
- Requirement 2: Printer Profile:
  - The printer profile is generally the settings you need to print with, tuned for each printer
  - If you have your own printer and have it tuned, great!
  - Otherwise, you'll need to get Mr. U or someone else to send you a copy of their profile so you can import it and get printing.
- Printing: Once you have those, you can proceed to:
  - Drag-and-Dropping the models you want into the slicing software
  - Adjust settings as needed
  - Slice models, and export to sd card or 3d printer and get them printing.
- Tuning: If your printed parts don't fit..
  - You may wanna tune them and adjust tolerances!
  - in the [`Project Files` folder](./Project%20Files/), you'll find the files to edit the models.
  - More details on this in [`Tuning and Editing`](#tuning-and-editing)


-----

## How to edit or tune the models?

So you need to edit the models in order to fit printer tolerances? You're in the right place:

### Hardware

To edit the files and make changes, you'll want access to either a **Mac** or a **Windows** machine. Sorry chromebook users!

<sub>_(This is the real world now...)_

### Software

First, you'll need some software. I, personally, modeled them in [Ondsel ES (https://ondsel.com/)](https://ondsel.com/), but the project files can also be edited in [FreeCAD (https://www.freecad.org/)](https://www.freecad.org/) if you prefer that.

### Tuning and Editing

Once you download and open the project files (the `.FCStd` files!), you can edit the models. There are a couple different options here, but the sky's the limit:

- Pre-made Parameters: In the tree hierarchy of the project you opened, you should find a spreadsheet names `Vars` or similar, which is a spreadsheet of variables I've made to make my life and your life easier
  - You'll see various columns like `Name` and `Value` and `Desciption/Notes` and some others.
  - Find the row you want to edit that makes sense, take note of the description and notes, and make your edit to the value. Press enter and look back at your model and you should see a change!
  - (It's just a spreadsheet don't over-think it)
  - If you're happy with the change and ready to print it, you should be able to export the object.
    - click on the body of the object
    - press `ctrl + e` (windows) or `cmd + e` (mac)
    - choose where you want to export it to
    - choose file type (like .obj or .stl)
    - adjust export options if needed
    - and export. 
  - Then print!
- Your own custom edits:
  - You could adjust my values, or you could also make your own changes.
  - You're more than welcome to add new features, pads, cuts, bevels, etc!