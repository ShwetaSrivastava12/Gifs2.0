Python GIF and Image Utilities
This repository contains a Python script (gifs2.0.py) that demonstrates several functionalities related to image processing, GIF creation, and animation using Pillow (PIL), imageio, matplotlib, and tkinter.

Features
The script provides the following capabilities:

GIF Creation from Static Images: Combines a list of static image files (JPG, PNG, GIF frames) into a single animated GIF. It also includes functionality to add custom text to each frame, positioned dynamically at the center horizontally and lower vertically.

GIF Creation from Matplotlib Plots: Generates a series of sine wave plots using matplotlib and then compiles them into an animated GIF.

Tkinter Image Switcher: A simple GUI application that allows you to switch between two static images.

Tkinter GIF Viewer: A GUI application that plays an animated GIF.

Setup
Before running the script, you need to install the required Python libraries.

Prerequisites
Python 3.x

Installation
Save the gifs2.0.py file.

Install the necessary Python packages using pip:

pip install pillow imageio matplotlib numpy

(tkinter is usually included with Python installations.)

Usage
The gifs2.0.py script contains several functions and execution blocks. You can run the entire script, or call specific functions as needed.

1. Configure Image Paths and Text
Before running, you must update the image_paths list at the beginning of the script to point to your actual image files.

image_paths = [
    r"C:\Users\minis\OneDrive\Desktop\My_Images\BTS.jpg", # Corrected from .jpg.jpg
    r"C:\Users\minis\OneDrive\Desktop\My_Images\BTS-PNG-Picture.png",
    r"C:\Users\minis\OneDrive\Desktop\My_Images\Bts.gif",
    # Add all your actual image paths here
]

For adding text to GIFs, adjust the following configuration variables:

# --- Configuration for text ---
TEXT_TO_ADD = "Hello Gemini!"
FONT_SIZE = 30
FONT_COLOR = (255, 255, 255) # White color (RGB)

# You can specify a font file path for better control.
# Example: FONT_PATH = r"C:\Windows\Fonts\arial.ttf"
# Make sure the font file exists on your system.
FONT_PATH = r"C:\Windows\Fonts\arial.ttf" # Set to None to use default PIL font

Ensure the FONT_PATH points to a valid .ttf or .otf font file on your system (e.g., C:\Windows\Fonts\arial.ttf for Windows).
