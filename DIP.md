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