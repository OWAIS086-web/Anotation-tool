Visionrd - Label Editor
Overview
Visionrd - Label Editor is a graphical user interface (GUI) application built using PySide6, OpenCV, and PIL. It allows users to load, view, edit, and manage labels for a collection of images. The application provides features like zoom, grayscale mode, search & replace, auto-saving, and label management in an easy-to-use interface.

Features
Image Viewing: Load images and view them within the application.
Label Editing: Edit labels associated with images efficiently.
Zoom In/Out: Easily zoom in or out on images.
Grayscale Mode: Toggle between color and grayscale modes.
Search & Replace: Perform search and replace operations on labels.
Color Picker: Change the application’s background color.
Navigation: Quickly navigate through images using Next, Back, and Go To controls.
Auto-Save: Automatically save labels periodically to prevent data loss.
Undo: Undo the recent label changes.
Prerequisites
Python 3.7 or later
Required Libraries:
PySide6
OpenCV (cv2)
Pillow (PIL)
NumPy (numpy)
You can install all required libraries using:

bash
Copy code
pip install PySide6 opencv-python pillow numpy
Getting Started
Clone or download the repository:
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
Replace label_editor.py with your actual script's filename if different.
Usage
Load Labels:

Click on "Load Labels" and select a label file.
Each line in the label file should have the format: image_path\tlabel (where \t is a tab separator).
Select Output Folder: Click "Select Output Folder" and choose the folder where the updated label file will be saved.

Label Editing:

Use the input field to edit the current label.
Click "Save" or press Enter to save changes and move to the next image.
Image Controls:

Next/Back: Navigate using "Next," "Back," or the arrow keys.
Zoom In/Out: Click + or - to zoom or use Up/Down arrow keys.
Grayscale: Toggle grayscale mode using the "Grayscale" button.
Pick Color: Change the background color using the "Pick Color" button.
Search & Replace:

Use the "Search & Replace" button to open the dialog.
Enter the search and replace terms to update labels.
Undo: Use the "Undo" button or Backspace key to revert changes.

Keyboard Shortcuts
Right Arrow: Save and move to the next image
Left Arrow: Move back to the previous image
Up Arrow: Zoom in
Down Arrow: Zoom out
Delete: Delete the current label
Backspace: Undo the last change
Enter/Return: Save the label and move to the next image
Folder Structure
visionrd_logo.png: Application icon file
label_editor.py: Main script file (replace this with your actual script name)
Handling Image Files
The application supports loading both grayscale and color images and allows resizing and zooming.

Error Handling
If an image cannot be loaded, an error message will be displayed.
Appropriate warnings are shown for invalid actions such as out-of-range indices.
Customization
Modify auto_save_interval in milliseconds to adjust the auto-save frequency.
The zoom factor can be customized via self.zoom_factor.
Saving Labels
Edited labels are saved to annotations_fix.txt in the selected output folder. Ensure both the label file and output folder are selected before starting label editing.

Acknowledgements
PySide6: Provides comprehensive Python bindings for the Qt toolkit.
OpenCV: Enables advanced image processing functionalities.
Pillow (PIL): Offers image manipulation capabilities.
License
This project is licensed under the MIT License - see the LICENSE file for details.

Support
For any issues or suggestions, feel free to open an issue on the GitHub repository or contact the developer.

Enjoy labeling your images with Visionrd - Label Editor!

