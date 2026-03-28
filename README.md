# 🎬 GIF Generator using Python

## 📌 Overview
This project is a simple Python script that creates an animated GIF from multiple images using the `imageio` library. It reads image files, processes them, and combines them into a single GIF with customizable speed and looping.

---

## ⚙️ How It Works
- Import the `imageio.v3` module
- Define a list of image filenames
- Read each image and store it in a list
- Combine all images into a GIF using `imwrite()`

---

## 💻 Code Example

```python
import imageio.v3 as iio

filenames = ['team-pic1.png', 'team-pic2.png']
images = []

for filename in filenames:
    images.append(iio.imread(filename))

iio.imwrite("image.gif", images, duration=500, loop=0)
