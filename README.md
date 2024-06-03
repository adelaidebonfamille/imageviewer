# Image Viewer Application

This repository contains a simple image viewer application built using Python, OpenCV, and Tkinter. The application allows users to load an image, display it in different modes (color, grayscale, original), and view it using OpenCV's image display functions.

## Table of Contents

- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)

## Features

- Load and display images from your file system
- Display images in three modes: color, grayscale, and original
- Use OpenCV to display images in a separate window
- User-friendly interface with Tkinter

## Installation

Ensure you have Python installed on your machine. You will also need to install the required libraries. You can install the necessary libraries using pip:

```bash
pip install opencv-python tkinter pillow
```

## Usage

1. Clone the repository:
   ```bash
   git clone https://github.com/adelaidebonfamille/image-viewer.git
   cd image-viewer
   ```

2. Run the application:
   ```bash
   python image_viewer.py
   ```

3. Use the interface to load and display images:
   - Click "Load Image" to select an image file from your computer.
   - Choose a display mode from the dropdown menu (color, grayscale, original).
   - Click "Show Image" to display the image in the selected mode using OpenCV.



### image_viewer.py

This is the main Python file containing the code for the image viewer application. It includes the following key components:

- `ImageViewer` class: Handles the creation of the Tkinter interface and the image display logic.
  - `__init__(self, master)`: Initializes the main application window and widgets.
  - `create_widgets(self)`: Creates and places widgets in the main window.
  - `load_image(self)`: Opens a file dialog to select an image file and updates the display.
  - `update_display(self)`: Resizes and displays the loaded image in the Tkinter interface.
  - `show_image(self)`: Displays the image using OpenCV in the selected mode (color, grayscale, original).
  - `show_image_cv(self, img_cv)`: Displays the given image using OpenCV.
  - `display_error_message(self, message)`: Displays error messages using Tkinter's messagebox.
