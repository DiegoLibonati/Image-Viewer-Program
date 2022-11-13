# Image-Viewer-Program

## Getting Started

1. Clone the repository
2. Join to the correct path of the clone
3. Install requirements.txt
4. Use `python image_viewer_program.py` to execute program

## Description

I made a python program that uses tkinter as user interface. This program allows to open images and display them, it works as an image viewer.

## Technologies used

1. Python

## Libraries used

1. Tkinter
2. PIL
3. os

## Galery

![image-viewer-program](https://raw.githubusercontent.com/DiegoLibonati/DiegoLibonatiWeb/main/data/projects/Python/Imagenes/imageviewerpython-0.jpg)

![image-viewer-program](https://raw.githubusercontent.com/DiegoLibonati/DiegoLibonatiWeb/main/data/projects/Python/Imagenes/imageviewerpython-1.jpg)

![image-viewer-program](https://raw.githubusercontent.com/DiegoLibonati/DiegoLibonatiWeb/main/data/projects/Python/Imagenes/imageviewerpython-2.jpg)

![image-viewer-program](https://raw.githubusercontent.com/DiegoLibonati/DiegoLibonatiWeb/main/data/projects/Python/Imagenes/imageviewerpython-3.jpg)

![image-viewer-program](https://raw.githubusercontent.com/DiegoLibonati/DiegoLibonatiWeb/main/data/projects/Python/Imagenes/imageviewerpython-4.jpg)

## Portfolio Link

`https://diegolibonati.github.io/DiegoLibonatiWeb/#/projects?q=Image%20Viewer%20Program`

## Video

https://user-images.githubusercontent.com/99032604/199144046-63b49fa5-be3d-4252-8e69-9b14b21d2e4b.mp4

## Documentation

This function `open_image()` opens the file passed by `filename`. Then we execute the `Image` method called `open` on this `filename`. We resize the image, process the image with the `PhotoImage` method. Then we set the image to display and display it:

```
def open_image():
    filename = filedialog.askopenfilename(initialdir=os.getcwd(), title="Select image file", filetype=(("JPG File", "*.jpg"), ("PNG file", "*.png"),("All file", "name.txt")))
    img = Image.open(filename)
    img = img.resize((1280,720))
    img = ImageTk.PhotoImage(img)
    label_image.configure(image=img)
    label_image.image=img
```
