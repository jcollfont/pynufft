# pynufft: Python non-uniform fast Fourier transform


FFT is the standard method that estimates the frequency components at equispaced locations.

NUFFT can calculate the frequency components at non-equispaced locations.

A minimal "getting start" tutorial is available at http://jyhmiinlin.github.io/pynufft/ .

Please use Python3. PyNUFFT has been tested with Python3.4. However, it should work with Python3.5-3.6. 


### New in version 0.3.3.10

Version 0.3.3.10 is a bug-fixed version. 

Experimental support for Python2. Some tests pass in Python2.7.15 but Python2 is not recommended.

Update for Reikna 0.8.0: async keyword is changed to async_


### Summary

Pynufft implements Fessler's min-max NUFFT, with the following features:

- Written in pure Python.
- Based on numerical libraries, such as Numpy, Scipy (matplotlib for displaying examples).
- Provides the python interface including forward transform, adjoint transform and other routines.
- Provides 1D/2D/3D examples for further developments.
- (Experimental) support of NUFFT on NVIDIA's graphic processing units (GPUs) and multi-core CPU platforms.

### Limitations

The FFTW is not provided in the official Numpy source. But you could include FFTW library in Numpy.

Check out the tutorial (http://jyhmiinlin.github.io/pynufft/misc/fftw.html) or the Anaconda's Python distribution.

### Other nufft implementations in Python:

Python-nufft: Python bindings to Fortran nufft. (https://github.com/dfm/Python-nufft/), MIT license

pynfft: Python bindings around the NFFT C-library, which uses the speed of FFTW, (https://github.com/ghisvail/pyNFFT), GPL v3

nfft: Pure Python implementation of 1D nfft (https://github.com/jakevdp/nfft). 

nufftpy: Pure Python NUFFT of Python-nufft (https://github.com/jakevdp/nufftpy). 

mripy: A Python based MRI package (https://github.com/peng-cao/mripy). combines Numba and NUFFT.

### Acknowledgements

pynufft was funded by the Ministry of Science and Technology, Taiwan, Cambridge Commonwealth, European and International Trust (Cambridge, UK), and Ministry of Education, Taiwan.  

If you find pynufft useful, please cite:

Jyh-Miin Lin and Hsiao-Wen Chung, Pynufft: python non-uniform fast Fourier transform for MRI, Building Bridges in Medical Sciences 2017, St John's College, CB2 1TP Cambridge, UK, 2017

And Fessler and Sutton's min-max NUFFT algorithm:
Fessler JA, Sutton BP. Nonuniform fast Fourier transforms using min-max interpolation. IEEE Trans Signal Process 2003;51(2):560-574.

Please open an issue if you have any question related to pynufft.

### Cite pynufft

@INPROCEEDINGS{lin2017bbmc_pynufft,
	author = {Jyh-Miin Lin and Hsiao-Wen Chung},
	booktitle = {Building Bridges in Medical Sciences 2017, St John's College, CB2 1TP Cambridge, UK},
	title = {{Pynufft: python non-uniform fast Fourier transform for MRI}},
	year = {2017}
}
