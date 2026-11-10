# Digital Images Processing 

# Fill in the Blanks 
1. In morphological image processing, Closing operation is performed by ______ followed by ______.
Answer: B) Dilation, Erosion

2. Opening operation is performed by ______ followed by ______.
Answer: B) Erosion, Dilation

3. The formula for Log Transformation is ______.
Answer: B) \(s = c\log(1+r)\)

4. City-Block Distance (D4) is calculated using ______.
Answer: B) \(|x_1-x_2|+|y_1-y_2|\)

5. The City-Block Distance between (7, −4) and (5, 2) is ______.
Answer: C) 10

6. A High-Pass Filter is mainly used for ______.
Answer: B) Image sharpening

7. The Watershed Algorithm is mainly used for ______.
Answer: B) Image segmentation

8. Image Segmentation divides an image into regions based on ______.
Answer: A) Discontinuity or Similarity

9. The full form of CAT is ______
Answer: A) Computerized Axial Tomography


# Q2) Answer the Following (Attempt Any 6 — 2 Marks Each / Total 12 Marks)

# 1. Differentiate between Sampling and Quantization (2–3 Marks)
# Sampling	                                    
1. Sampling converts continuous coordinates into discrete values.	
2. It determines the number of pixels in an image.	
3. It affects the spatial resolution of an image.	

 # Quantization
1. Quantization converts continuous amplitude (intensity) into discrete values.
2. It determines the number of intensity levels.
3. It affects the intensity resolution of an image.

# 2. What is Histogram Equalization? (2 Marks)
Definition: Histogram Equalization is an image enhancement technique used to improve the overall contrast of an image.
> It spreads the intensity values of pixels over a wider range.
> It makes dark areas clearer and improves image visibility.
Example: It makes a dull or low-contrast image look clearer and brighter.

# 3 Define Opening and Closing Operations (2–3 Marks)
# 1. Opening Operation:
- Opening is a morphological operation performed by erosion followed by dilation.
- It is used to remove small unwanted objects or noise from an image.
Set Formula: A ∘ B = (A ⊖ B) ⊕ B

# 2. Closing Operation:
- Closing is a morphological operation performed by dilation followed by erosion.
- It is used to fill small holes and gaps in an image.
Set Formula: A • B = (A ⊕ B) ⊖ B

# 4. Differentiate between Linear and Non-Linear Operations (2–3 Marks)
# Linear Operations	
> Output changes proportionally with input values.	
> Uses addition and averaging operations.	
> Example: Mean Filter.	

# Non-Linear Operations
> Output does not change proportionally with input values.
> Uses sorting and selecting operations.
> Example: Median Filter.


# 5. Define Image Segmentation and Discontinuity (2–3 Marks)
1. Image Segmentation:
- Image Segmentation is the process of dividing an image into smaller meaningful regions or parts.
- It helps to identify and separate different objects in an image.
2. Discontinuity:
- Discontinuity means a sudden change in pixel intensity or brightness in an image.
- It is used to detect edges and boundaries of objects.
Example: Separating a car from the background is Image Segmentation. Detecting the car's edges is Discontinuity.

# 6. Explain Chain Code and Shape Number with an Example (2–3 Marks)
1. Chain Code:
- Chain Code is a method used to represent the boundary or shape of an object using a sequence of direction numbers.
- It shows the direction of each boundary pixel.
2. Shape Number:
- Shape Number is obtained by taking the first difference of the Chain Code.
- It represents the shape and is independent of the starting point.

# 7. Role of Fourier Transform in Image Processing (2–3 Marks)
- Fourier Transform converts an image from the spatial domain to the frequency domain.
- It helps to separate low-frequency and high-frequency components.
- It is used for image filtering, noise removal and image enhancement.
- It helps in image sharpening and smoothing.

# Define Pattern and Pattern Class (2 Marks)
# 1. Pattern:
- A pattern is an object or item that we want to identify in an image.
- Example: A handwritten letter or a number.
# 2. Pattern Class:
- A Pattern Class is a group of patterns having similar features or characteristics.
- Example: All images of digit 5 belong to the same pattern class.


# Write Expressions for Structuring Element Reflection and Translation (2–3 Marks)
1. Reflection:
- Reflection means flipping the structuring element around the origin.
> Formula (Copy & Paste):
> B̂ = {w | w = -b, for every b ∈ B}

2. Translation:
- Translation means shifting the structuring element from one position to another.
> Formula (Copy & Paste):
> (B)z = {c | c = b + z, for every b ∈ B}


# Q3- Answer the Following ( 4 marks each )
# 1. Explain Dilation and Erosion Operations with 3 × 3 Matrix Examples (4 Marks)
1. Dilation:
> Dilation is a morphological operation used to increase or expand the white (foreground) area of an image.
> It adds pixels to the boundaries of an object.
> It helps to fill small gaps and connect nearby objects.
Example: 
Input Matrix:        |            After Dilation (using a 3 × 3 structuring element):
0 0 0                |           1 1 1
0 1 0                |           1 1 1
0 0 0                |           1 1 1

2. Erosion:
> Erosion is a morphological operation used to decrease or shrink the white (foreground) area of an image.
> It removes pixels from the boundaries of an object.
> It helps to remove small unwanted objects.
Example:
Input Matrix:              After Erosion (using a 3 × 3 structuring element):
1 1 1                |           0 0 0
1 1 1                |           0 1 0
1 1 1                |           0 0 0

# 2. Spatial Filtering Techniques for Smoothing (Means , Median) and Sharpening (sobel, laplician) (4 Marks)
Spatial Filtering: It is a technique used to improve an image by changing pixel values using a small filter mask.

1. Smoothing Filters:
> Mean Filter:
- It replaces the centre pixel with the average value of neighbouring pixels.
- It is used to reduce noise and blur the image.
> Median Filter:
- It replaces the centre pixel with the median value of neighbouring pixels.
- It is useful for removing salt-and-pepper noise.

2. Sharpening Filters:
> Sobel Filter:
- It detects edges by finding changes in pixel intensity.
- It highlights horizontal and vertical edges.
> Laplacian Filter:
- It uses the second-order derivative to detect rapid intensity changes.
- It makes edges and fine details sharper.


# 3. Common Noise Models: Gaussian Noise vs Salt-and-Pepper (Impulse) Noise (4 Marks)
1. Gaussian Noise:
- Gaussian Noise is a type of noise that changes pixel brightness randomly.
- It follows a normal (bell-shaped) distribution.
- It makes the image look grainy.
- It can be reduced using a Mean or Gaussian Filter.
2. Salt-and-Pepper (Impulse) Noise:
- It is a type of noise that appears as random black and white dots in an image.
- It changes some pixels to maximum (white) or minimum (black) values.
- It makes the image look like tiny black and white spots.
- It can be reduced using a Median Filter.


# 4. Distance Measures Between Pixels (4 Marks)
Let two pixels be P(x₁, y₁) and Q(x₂, y₂).
# 1. Euclidean Distance (De):
- It is the straight-line distance between two pixels.
- Formula: De = √[(x1 - x2)² + (y1 - y2)²]

# 2. City-Block Distance (D4):
- It measures distance by moving only horizontally and vertically.
- Formula:D4 = |x1 - x2| + |y1 - y2|

# 3. Chessboard Distance (D8):
- It measures distance by moving horizontally, vertically, or diagonally.
- Formula: D8 = max(|x1 - x2|, |y1 - y2|)


# 5. Basic Gray-Level Transformations (4 Marks)
Gray-level transformations are used to change the brightness and contrast of an image.
# 1. Negative Transformation:
- It changes a bright pixel into a dark pixel and vice versa.
- It is useful for enhancing details in dark areas.
- Formula: s = (L - 1) - r

# 2. Log Transformation:
- It converts dark pixels into brighter values.
- It is useful for improving details in dark areas of an image.
- Formula: s = c × log(1 + r)

# 3. Power-Law (Gamma) Transformation:
- It changes the brightness of an image using a gamma value.
- It is useful for brightness and contrast correction.
- Formula: s = c × r^γ

# 6. Boundary Descriptors vs. Regional Descriptors (4 Marks)
1. Boundary Descriptors:
- They describe the boundary or outline of an object.
- They mainly focus on the shape of the object.
- They are useful for identifying objects based on their outer boundary.
- Examples: Chain Code, Shape Number, and Fourier Descriptors.
2. Regional Descriptors:
- They describe the entire region or area of an object.
- They use properties inside the object, such as area, texture, and intensity.
- They are useful for identifying objects based on their region.
- Examples: Area, centroid, and moments.


# Adaptive Thresholding vs Global Thresholding — 4 Marks
Adaptive Thresholding:
Adaptive thresholding is a segmentation method where the threshold value changes for different regions of an image based on local pixel properties.

Why preferred over Global Thresholding:
1. Global thresholding uses one fixed threshold for the entire image.
2. Adaptive thresholding uses different thresholds for different areas.
3. It works better when the image has uneven or varying illumination.
4. It can detect objects/details even when some parts are dark and other parts are bright.


# Q4 ) Answer the Following (Attempt Any 2 — 6 Marks Each / Total 12 Marks)
# 1. Explain Components of a Digital Image Processing System with a Neat Block Diagram. (6 Marks)
Definition
A Digital Image Processing System is a system used to capture, process, store, display and transfer digital images.
Neat Block Diagram
                         NETWORK
              ─────────────────────────────
              ↕             ↕              ↕
       IMAGE DISPLAY ←→  COMPUTER  ←→ MASS STORAGE
                            ↕
             ↙──────────────┼──────────────↘
            ↙               ↕                ↘
   HARD COPY DEVICE   IMAGE PROCESSING    IMAGE PROCESSING
                         HARDWARE             SOFTWARE
                            ↕
                       IMAGE SENSORS
                            ↑
                      PROBLEM DOMAIN

Components of the System
1. Image Sensors
   - Capture the image from the real-world problem domain.
   - Convert the captured information into digital image data.
2. Image Processing Hardware
   - Performs basic operations required for processing digital images.
   - It works with the computer to process the image.
3. Computer
   - Controls and coordinates the complete image processing system.
   - It executes the required image processing operations.
4. Image Processing Software
   - Contains programs and algorithms used to process images.
   - Examples: enhancement, restoration, segmentation, etc.
5. Mass Storage
   - Stores original and processed images.
   - Provides temporary and permanent storage.
6. Image Display
   - Displays the processed image on a monitor or screen.
7. Hard Copy Device
   - Produces a permanent printed copy of the image.
   - Example: printer.
8. Network
   - Allows images to be transmitted and shared between different systems.


# 2 —Explain Frequency Domain Lowpass Filters: Ideal, Butterworth, and Gaussian with Cut-Off Profiles
(6 Marks — Exam-Oriented, Point-wise)
1. Definition
A Low-Pass Filter (LPF) in the frequency domain allows low-frequency components to pass and reduces high-frequency components.
- Low frequencies → smooth regions
- High frequencies → edges and fine details
- Therefore, LPF is mainly used for smoothing and noise reduction.
2. Ideal Low-Pass Filter (ILPF)
The Ideal LPF passes all frequencies inside the cut-off frequency and completely blocks frequencies outside it.

Formula:
H(u,v) = 1,   if D(u,v) ≤ D₀
         0,   if D(u,v) > D₀

Where:
- D(u,v) = distance from frequency origin
- D₀ = cut-off frequency
Cut-off profile:
H
1 ─────────┐
           │
0          └──────────────→ D
            D₀

👉 Sharp cut-off → may produce ringing effect.
3. Butterworth Low-Pass Filter (BLPF)
Butterworth LPF provides a smooth transition between low and high frequencies.

Formula:
H(u,v) = 1 / [1 + (D(u,v)/D₀)²ⁿ]

Where:
- D₀ = cut-off frequency
- n = order of filter
Cut-off profile:
H
1 ───────────╮
             ╲
              ╲
0              ╰──────────→ D
                 D₀

👉 Increasing n makes the transition sharper.
4. Gaussian Low-Pass Filter (GLPF)
Gaussian LPF gives a very smooth transition and does not have a sharp cut-off.

Formula:
H(u,v) = e^[−D²(u,v) / 2D₀²]

Cut-off profile:
H
1 ─────────╮
           ╲
            ╲
             ╲____
0                  ───────→ D
              D₀

👉 It provides smooth filtering and causes less ringing.