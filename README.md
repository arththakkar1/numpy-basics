# Python Numpy Basics and Image Processing

This project demonstrates basic usage of NumPy, saving `.npy` files, and simple image processing to convert a light mode image to dark mode.

## Contents

- **NumPy Basics:**  
   Learn how to create and manipulate arrays using NumPy.

- **Saving `.npy` Files:**  
   Save NumPy arrays to disk for later use.

- **Image Processing:**  
   Convert a light mode image to dark mode using NumPy operations.

## Getting Started

1. **Install Dependencies:**

   ```bash
   pip install numpy pillow
   ```

2. **Run the Code:**
   - Explore the scripts to see examples of NumPy basics.
   - Check how arrays are saved and loaded with `.npy` files.
   - See how an image is inverted to create a dark mode effect.

## Example: Inverting an Image

```python
from PIL import Image
import numpy as np

img = Image.open('light_mode_image.png')
arr = np.array(img)
dark_arr = 255 - arr  # Invert colors
dark_img = Image.fromarray(dark_arr)
dark_img.save('dark_mode_image.png')
```

---

Feel free to explore and modify the code to deepen your understanding of NumPy and basic image processing!
