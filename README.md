# Fourier Frequency Filters for Image Processing

Implementation and comparison of frequency-domain image filtering techniques using the 2D Fourier Transform.

## Overview

This project demonstrates how image filtering can be performed in the Fourier domain. The image is transformed from the spatial domain to the frequency domain using the Fast Fourier Transform (FFT), filtered with different frequency masks, and then reconstructed using the inverse FFT.

The project includes:

* Ideal Low-Pass Filter (ILPF)
* Butterworth Low-Pass Filter (BLPF)
* Ideal High-Pass Filter (IHPF)
* Fourier Spectrum Visualization
* Automated Filter Evaluation
* Comparison of Filtering Effects

## Technologies

* Python
* OpenCV
* NumPy
* Matplotlib
* Pandas

## Processing Pipeline

1. Load grayscale image.
2. Compute 2D Fourier Transform.
3. Shift the frequency spectrum to the center.
4. Create frequency-domain filter masks.
5. Apply filters in the frequency domain.
6. Perform inverse Fourier Transform.
7. Normalize and visualize results.
8. Compare filter behavior and image quality.

## Implemented Filters

### Ideal Low-Pass Filter (ILPF)

Allows low-frequency components to pass while removing high-frequency components.

**Effect:**

* Image smoothing
* Noise reduction
* Loss of fine details
* Strong ringing artifacts

### Butterworth Low-Pass Filter (BLPF)

A smoother alternative to the ideal filter with gradual frequency attenuation.

**Effect:**

* Smoother transitions
* Reduced ringing artifacts
* Better visual quality

### Ideal High-Pass Filter (IHPF)

Removes low-frequency components and preserves high-frequency information.

**Effect:**

* Edge enhancement
* Detail sharpening
* Increased emphasis on texture

## Results

The experiments show that:

* Low-pass filters smooth the image and suppress high-frequency details.
* High-pass filters enhance edges and fine structures.
* Butterworth filtering produces more natural-looking results than ideal filtering.
* Ringing artifacts become more noticeable with sharp frequency cutoffs.
* Increasing the Butterworth order makes its behavior closer to the Ideal filter and increases ringing effects.

