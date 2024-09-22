# Visionrd - Label Editor

## Overview

**Visionrd - Label Editor** is a graphical user interface (GUI) application built using PySide6, OpenCV, and PIL. It enables users to load, view, edit, and manage labels for a collection of images. The application offers features like zooming, grayscale mode, search & replace, auto-saving, and label management in a user-friendly interface.

## Features

- **Image Viewing**: Load images and view them within the application.
- **Label Editing**: Edit and update labels associated with images.
- **Zoom In/Out**: Zoom in or out on images.
- **Grayscale Mode**: Toggle between color and grayscale image modes.
- **Search & Replace**: Perform search and replace operations on labels.
- **Color Picker**: Change the application’s background color.
- **Navigation**: Navigate through images using Next, Back, and Go To controls.
- **Auto-Save**: Automatically save labels periodically to prevent data loss.
- **Undo**: Undo recent changes to labels.

## Prerequisites

- Python 3.7 or later
- Required Libraries:
  - PySide6
  - OpenCV (`cv2`)
  - Pillow (`PIL`)
  - NumPy (`numpy`)

Install the required libraries using:
```bash
pip install PySide6 opencv-python pillow numpy

Getting Started
Clone the repository:
bash
Copy code
git clone https://github.com/your-username/visionrd-label-editor.git
Navigate to the project directory:
bash
Copy code
cd visionrd-label-editor
Run the application:
bash
Copy code
python label_editor.py
(Replace label_editor.py with your actual script's filename if different.)
Usage
1. Load Labels
Click on "Load Labels" and select a label file.
The label file should have each line formatted as: image_path\tlabel (where \t represents a tab separator).
2. Select Output Folder
Click "Select Output Folder" and choose the folder where the updated label file will be saved.
3. Label Editing
Use the input field to edit the current label.
Click "Save" or press Enter to save changes and move to the next image.
4. Image Controls
Next/Back: Navigate using Next, Back, or the arrow keys.
Zoom In/Out: Click + or - to zoom in or out, or use the Up/Down arrow keys.
Grayscale: Toggle grayscale mode using the "Grayscale" button.
Pick Color: Change the background color using the "Pick Color" button.
5. Search & Replace
Use the "Search & Replace" button to open the dialog.
Enter the search and replace terms to update labels.
6. Undo
Use the "Undo" button or Backspace key to revert changes.
Keyboard Shortcuts
Key	Action
Right Arrow	Save and move to next image
Left Arrow	Move back to previous image
Up Arrow	Zoom in
Down Arrow	Zoom out
Delete	Delete the current label
Backspace	Undo the last change
Enter/Return	Save the label and move to the next image
Folder Structure
plaintext
Copy code
visionrd-label-editor/
│
├── label_editor.py        # Main application script
├── visionrd_logo.png      # Application icon
├── README.md              # Project documentation
└── requirements.txt       # Required dependencies (optional)
Handling Image Files
The application supports loading both grayscale and color images.
Images are resized and adjusted according to the zoom factor.
Error Handling
An error message will be displayed if an image cannot be loaded.
Warning messages will be shown for invalid actions (e.g., out-of-range indices).
Customization
Adjust auto_save_interval (in milliseconds) to change the auto-save frequency.
Modify the zoom_factor to customize zooming behavior.
Saving Labels
Edited labels are saved to annotations_fix.txt in the selected output folder.
Ensure both the label file and output folder are selected before editing labels.
Acknowledgements
PySide6: Provides comprehensive Python bindings for the Qt toolkit.
OpenCV: Enables advanced image processing functionalities.
Pillow (PIL): Offers image manipulation capabilities.
License
This project is licensed under the MIT License - see the LICENSE file for details.

Support
For any issues or suggestions, feel free to open an issue on the GitHub repository or contact the developer.

Enjoy labeling your images with Visionrd - Label Editor!
