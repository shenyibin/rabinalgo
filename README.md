$Id$

Sliding Window Based Rabin Fingerprint Computation Library

o Function
  Given a stream of input, compute the rabin-fingerprint of a N-byte-long 
  sliding window, reading the bytes of the stream one by one

o Usage
  - rabinpoly library provides a very simple interface that 
	1) defines the sliding window size, 
	2) reads bytes one by one and returns the rabin-fingerprint of 
	   the current sliding window, and 
	3) resets the sliding window.

  - Look at the example in the example/ directory. The example code 
    reader.cc takes a file and reports the rabin-fingerprints of overlapping 
    64Byte-long sliding windows reading the bytes one by one. To compile the
    example program, read README under the directory.

  - You can find the detail of Rabin Fingerprint in
   "Rabin, M. O. Fingerprinting by Random Polynomials. Tech. Rep. TR-15-81. 
    Center for Research in Computing Technology. Harvard University, 1981."

o History
  - Taken from David Mazieres's LBFS implementation and modified as a 
    stand-alone version by Niraj Tolia et al. (For Content Addressable Storage) 
  - Modified to support a configurable sliding window size and packaged by 
    Hyang-Ah Kim
  - 2005.12.2 version 1.0a 
    Added an example file which was missing in the initial distribution

