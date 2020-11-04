# Fast — CNN

This repository proposed a new method of convolving the image with kernel. Instead of convolving the images and kernels, I used FFT property. By using the property we are able to reduce much time and prevent edges. We are able to generate similiar results of convolution layers from Fast Fourier Transform.

![](/media/p3.jpg)

## Fast Fourier Transform

The Fourier Transform is one of the deepest insights ever made in mathematics but unfortunately, the meaning is buried deep inside some ridiculous equations. The Fourier transform is a way of splitting something up into a bunch of sine waves. 

![](/media/sine.gif)

As usual, the name comes from some person who lived a long time ago called Fourier. In mathematical terms, The Fourier Transform is a technique that transforms a signal into its constituent components and frequencies. Fourier transform is widely used not only in signal (radio, acoustic, etc.) processing but also in image analysis eg. edge detection, image filtering, image reconstruction, and image compression. One example: Fourier transform of transmission electron microscopy images helps to check the periodicity of the samples. periodicity — means pattern. Fourier transform of your data can expand accessible information about the analyzed sample.

![](/media/fft.gif)

## FFT Property

The property says that by taking fourier transform of both image and kernel and multiply in frequency domain, and then taking inverse fourier transform, we can get the resultant same or very similiar as the resultant of convolution.

## Output after Convolution

![](/media/cnnoutput.png)

## Output after applying FFT property

![](/media/fftoutput.jpg)
