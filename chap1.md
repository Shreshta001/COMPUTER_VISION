# 📸 Digital Image Processing Concepts

## 1. Digital Image Representation

### Concept
- Digital image representation involves converting visual information into a format that computers can process and store. This is essential for tasks in computer vision, image analysis, and more. 🖼️

### How Images Are Stored Digitally
- **🟡 Pixels**: 
  - Images are composed of small units called **pixels** (picture elements).
  - Each pixel represents a specific point in the image.
  
- **🎨 Color Depth**:
  - Pixels store color information, typically in **RGB format** (Red, Green, Blue).
  - Each color channel can have a range of values (e.g., 0-255 for 8-bit depth).

- **🖥️ Bitmaps**:
  - Images can be stored as **bitmap files** where pixel values are arranged in a grid format representing the image's height and width.

### Role of Pixels
- Pixels are the fundamental building blocks of digital images. 🧩
- The arrangement of pixels in a grid creates the visual representation of the image.

### Pixel Intensity
- Refers to the **brightness** or **color value** of a pixel. 💡
- In grayscale images, intensity values range from 0 (black) to 255 (white).
- Higher pixel intensity values correspond to **brighter colors**, contributing to overall image information and quality.

---

## 2. Linear Systems in Image Processing

### Definition
- A **linear system** in image processing is one where the output is directly proportional to the input. 📊

### Properties
1. **Linearity**:
   - The response to combined inputs is the sum of the responses to each input.
   - Mathematically: 
     \[
     f(a \cdot x + b \cdot y) = a \cdot f(x) + b \cdot f(y)
     \]

2. **Shift-Invariance**:
   - The system's response does not depend on the position of the input.
   - Mathematically: 
     \[
     f(x - x_0) = f(x)
     \]

### Usage in Filtering Operations
- Linear systems are commonly used in **filtering operations** where input images are processed to enhance or detect features. 🔍
- Examples include **Gaussian blurring**, **edge detection**, and **image sharpening**.

---

## 3. Convolution and Cross-Correlation

### Convolution
- **Definition**: A mathematical operation that combines two functions to produce a third function. 🤝
- **Formula**:
  \[
  (f * g)(x, y) = \sum_{m=-\infty}^{\infty} \sum_{n=-\infty}^{\infty} f(m, n) \cdot g(x - m, y - n)
  \]
  - Here, \( f \) is the input image and \( g \) is the kernel/filter.

### Cross-Correlation
- **Definition**: A measure of similarity between two signals (or images) as a function of the time-lag applied to one of them. 📈
- **Formula**:
  \[
  (f \star g)(x, y) = \sum_{m=-\infty}^{\infty} \sum_{n=-\infty}^{\infty} f(m, n) \cdot g(m + x, n + y)
  \]
  - The kernel is **not flipped** in this operation.

### Differences
| Aspect               | Convolution                               | Cross-Correlation                          |
|----------------------|------------------------------------------|-------------------------------------------|
| 🔄 **Kernel Handling**      | Kernel is flipped                         | Kernel remains the same                   |
| 🎯 **Purpose**              | Used for filtering                        | Used for similarity measurement            |
| 📐 **Mathematical Focus**   | Focuses on signal modification           | Focuses on comparing signals               |

---

This README provides a structured overview of key concepts in digital image representation, linear systems in image processing, and the differences between convolution and cross-correlation. Use this as a quick reference for your exam! 🎓
