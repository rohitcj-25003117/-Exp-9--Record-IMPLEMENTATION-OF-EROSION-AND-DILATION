# Exp-9--Record-IMPLEMENTATION-OF-EROSION-AND-DILATION
# Implementation of Erosion and Dilation Using OpenCV

## Aim

To write a Python program using OpenCV to perform morphological operations such as **Erosion** and **Dilation** on an image.

The program performs the following operations:

* Image Erosion
* Image Dilation

---

## Software Used

* Anaconda – Python 3.7
* Jupyter Notebook / VS Code
* OpenCV (`cv2`)
* NumPy
* Matplotlib

---

## Algorithm

### Step 1:

Import the required libraries: OpenCV, NumPy, and Matplotlib.

### Step 2:

Load the input image using OpenCV.

### Step 3:

Display the original image.

### Step 4:

Create a structuring element (kernel) of suitable size.

### Step 5: Image Erosion

* Apply the erosion operation using the created kernel.
* Remove pixels from the boundaries of foreground objects.
* Display the eroded image.

### Step 6: Image Dilation

* Apply the dilation operation using the same kernel.
* Add pixels to the boundaries of foreground objects.
* Display the dilated image.

### Step 7:

Compare the original, eroded, and dilated images.

---

## Program

### Original Image

```python
import cv2
import matplotlib.pyplot as plt

img = cv2.imread("JANA JAVA.jpg")

plt.imshow(cv2.cvtColor(img, cv2.COLOR_BGR2RGB))
plt.title("Original Image")
plt.axis("off")
plt.show()
```

### Erosion

```python
kernel = cv2.getStructuringElement(cv2.MORPH_RECT, (5, 5))

erosion = cv2.erode(img, kernel, iterations=1)

plt.imshow(cv2.cvtColor(erosion, cv2.COLOR_BGR2RGB))
plt.title("Image Erosion")
plt.axis("off")
plt.show()
```

### Dilation

```python
kernel = cv2.getStructuringElement(cv2.MORPH_RECT, (5, 5))

dilation = cv2.dilate(img, kernel, iterations=1)

plt.imshow(cv2.cvtColor(dilation, cv2.COLOR_BGR2RGB))
plt.title("Image Dilation")
plt.axis("off")
plt.show()
```

---

## Output

### Original Image
<img width="509" height="409" alt="download" src="https://github.com/user-attachments/assets/4dcdfeca-7088-445d-9b15-5673ce0d9fd8" />


### Erosion

<img width="509" height="409" alt="download" src="https://github.com/user-attachments/assets/2b23c725-bdc2-4ba5-90d0-e3649330d22b" />

### Dilation

<img width="509" height="409" alt="download" src="https://github.com/user-attachments/assets/fbf3f756-447e-482f-9d81-0e12940bc952" />

---

## Result

Thus, the morphological operations **Erosion** and **Dilation** are successfully implemented using OpenCV.

---

## Developed By

**Name:** CJ ROHIT

**Register No:** 212224243005
