# Dot Art Generator with Turtle Graphics

A simple Python project that creates dot art patterns inspired by extracted colors from an image. Using Python's `turtle` graphics library and a pre-defined list of RGB colors, this script generates a 10x10 grid of colored dots, producing a visually appealing artwork.

## Table of Contents

- [Overview](#overview)
- [Project Structure](#project-structure)
- [Features](#features)
- [Setup Instructions](#setup-instructions)
- [Code Details](#code-details)
- [Requirements](#requirements)

## Overview

The project generates a dot art pattern by positioning dots in a grid, each with a random color from a pre-defined color palette. The color palette is extracted from an image using the `colorgram` library, which provides a list of RGB values used in the artwork. This dot art resembles the style of pointillism, an art technique where small dots create an image.

## Project Structure

- **`color_extraction.py`**: Extracts RGB colors from an image file, using the `colorgram` library to create a color palette.
- **`dot_art.py`**: The main script that generates the dot art pattern using `turtle` graphics.

## Features

- **Color Extraction**: Uses `colorgram` to pull RGB colors from an image to use as a palette.
- **Dot Art Generation**: Utilizes the `turtle` graphics module to create a 10x10 grid of colored dots.
- **Randomized Colors**: Each dot is assigned a random color from the extracted palette.

## Setup Instructions

1. **Install Requirements**:
    ```bash
    pip install colorgram.py
    ```

2. **Run the Color Extraction** (optional):
    - Run the code snippet in `color_extraction.py` to create your own `color_list` by extracting colors from any image (e.g., `image.jpg`).
    - Add the resulting RGB values to the `color_list` in `dot_art.py`.

3. **Run the Dot Art Generator**:
    ```bash
    python dot_art.py
    ```

## Code Details

1. **Color Extraction (`color_extraction.py`)**:
    - This code extracts RGB values from an image, `image.jpg`, creating a list of colors.
2. **Dot Art Creation (`dot_art.py`)**:
    - The turtle's starting position is adjusted for better centering.
    - A 10x10 grid of dots is drawn, each dot being a randomly chosen color from the `color_list`.

## Requirements

- Python 3.6+
- `colorgram.py` library
- `turtle` (comes with Python)

## License

This project is licensed under the MIT License. See the `LICENSE` file for details.
