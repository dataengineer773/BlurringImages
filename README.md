We want to smooth out an image, To blur an image, each pixel is transformed to be the average value of its neighbors. This neighbor and
the operation performed are mathematically represented as a kernel (don’t worry if you don’t know
what a kernel is). The size of this kernel determines the amount of blurring, with larger kernels
producing smoother images. Here we blur an image by averaging the values of a 5 × 5 kernel around
each pixel, To highlight the effect of kernel size, here is the same blurring with a 100 × 100 kernel, Kernels are widely used in image processing to do everything from sharpening to edge detection, and
will come up repeatedly in this chapter. The blurring kernel we used looks like this, The center element in the kernel is the pixel being examined, while the remaining elements are its
neighbors. Since all elements have the same value (normalized to add up to 1), each has an equal say in
the resulting value of the pixel of interest. We can manually apply a kernel to an image using filter2D
to produce a similar blurring effect
