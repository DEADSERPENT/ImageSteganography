# Image Steganography

This program enables you to hide and extract text data within images using Steganography techniques.

## Setup

```python
from tkinter import *
from tkinter import ttk
import tkinter.filedialog
from PIL import ImageTk
from PIL import Image
from tkinter import messagebox
from io import BytesIO
import os
```markdown
# Image Steganography

This program enables you to hide and extract text data within images using Steganography techniques.

## Setup

```python
from tkinter import *
from tkinter import ttk
import tkinter.filedialog
from PIL import ImageTk
from PIL import Image
from tkinter import messagebox
from io import BytesIO
import os
```

## Class Definition: `Stegno`

### Attributes
- `art`: ASCII art for decoration.
- `art2`: Another ASCII art for decoration.
- `output_image_size`: Size of the output image after encoding.

### Methods

#### `main(self, root)`
- Displays the main window of the application.

#### `home(self, frame)`
- Destroys the current frame and goes back to the main window.

#### `frame1_decode(self, f)`
- Displays the decode frame for selecting an image with hidden text.

#### `frame2_decode(self, d_f2)`
- Displays the decode process frame.

#### `decode(self, image)`
- Decodes the hidden text from the provided image.

#### `frame1_encode(self, f)`
- Displays the encode frame for selecting an image to hide text.

#### `frame2_encode(self, f2)`
- Displays the encode process frame.

#### `info(self)`
- Displays information about the original and decoded images.

#### `genData(self, data)`
- Generates binary data from the input text.

#### `modPix(self, pix, data)`
- Modifies the pixels of the image to hide the data.

#### `encode_enc(self, newimg, data)`
- Encodes the data into the image.

#### `enc_fun(self, text_area, myimg)`
- Initiates the encoding process.

#### `page3(self, frame)`
- Goes back to the main window from any frame.

## Usage

```python
root = Tk()

o = Stegno()
o.main(root)

root.mainloop()
```

This script sets up a Tkinter GUI application for image steganography.
```
