# introduction
ofxQuantum is part of an ongoing project to investigate Quantum Computing using artistic methods and practices while undertaking my MFA in computational arts at Goldsmiths University London. This piece of a software is the first step in this process and began from the idea of creating theoretical software libraries for hardware that doesn't exist yet.

The aim of this project is to create a bridge between openframeworks which is a tool that is very popular amongst creative coders and new media artists and quantum computing which is a branch of abstract computing which only exists theoretically at this time. In this way I am providing a tool for the future that may possibly be used one day by artists but at the moment is nothing more than an intellectual curiosity.

This project was inspired by my interest in mathematics and computational theory and to develop theoretically and conceptual software. Programming and software design can be very practical and is mostly put to non poetic or practical creative uses so I wanted to make software that is more conceptual and artistic but also may have some practical use at some point even if it can't be used for anything practical at the moment. The reason that I choose quantum computing is that I am fascinated with the way that something as random and seemingly uncontrollable such as quantum mechanics can be put into a mathematical logic that can be used for computation.

# what is quantum computing?

Quantum comping is an area of computing first formulated by several computer theorists the early
1980s (1)(2)(3) which uses the effects of quantum mechanics to perform computational tasks. While
classical computing uses a binary 1/0 bit quantum computing uses a Qubit which holds a superposition
of states between 1 and 0 and works within a world that is filled with probabilities rather than
solid deterministic type variables. This allows a quantum computer to work with bits that hold the probability
of the bit being in a state of 1 or 0 and with some clever algorithm design can compute the results across all posssible solutions to a problem. Another interesting feature of quantum computing is that quantum bits exist in a probability of being in a certain state until the bit is measured. This allows for the use of quantum computing to solve problems that are currently too coputationally heavy to solve on a
classical computer.

# about this addon

This addon implements the dlib library dlib.net which is an open source c++ library by David King to do various abstract computing methods and apply these to real world problems (5) The addon acts as a wrapper to make the implementation of quantum algorithms easier and provides open frameworks programmers with easy access to a quantum computing simulation library. The underlying software library can be seen to be irrelevant to the higher level wrapper ofxQuantum.h which is the main point of entry for the code.

# examples

SimpleHadamardGateExample - Simple example showing the output from a hadamard gate

GroversSearchAlgorithmExample - Shows an implementation of Grovers search algorithm (4)

These must be placed in the myApps openframeworks/apps/myapps (or folder of equal directory depth)

# usage
This addon works with the project generator on OF 8.4 and 9.0 with xcode (osx) and Visual Studio 2015 (windows 8)

The basic usage of the addon is through the ofxQuantum class, the basic usage is:

```c++
ofxQuantum qSim;	 	// Create ofxQuantum object

qSim.init(1);			// Initialise the simulator with 1 bit

qSim.applyGateX(0);		// Apply the Pauli X gate to the first bit

qSim.measureBit(0);		// Measure the first bit

```

# further development
This work is part of an ongoing project into the investigation of quantum computing through artistic methods. The next phase of the project is to develop various hardware components that can be used in a quantum computer. One such component is the 

Quantum State Observation Seed Generation Unit 

which is used to measure states of quantum bits. This will take the form of a device that generates random numbers using quantum phenomena such as the decay of a radioactive isotope. This radioactive decay is a direct manifestation of quantum behaviour of partilces and can be easily measured using a geiger counter.

A further device will be the n-Qbit meausrement gate which will use the Von Neumann Meausurement Unit which is a more advanced device that measures the states of quantum particles.

# references
1. Benioff, Paul (1980). "The computer as a physical system: A microscopic quantum mechanical Hamiltonian model of computers as represented by Turing machines". Journal of statistical physics 22 (5): 563–591.

2. Manin, Yu. I. (1980). Vychislimoe i nevychislimoe [Computable and Noncomputable] (in Russian). Sov.Radio. pp. 13–15. Retrieved 2013-03-04.

3. Feynman, R. P. (1982). "Simulating physics with computers". International Journal of Theoretical Physics 21 (6): 467–488. Bibcode:1982IJTP...21..467F. doi:10.1007/BF02650179.
Developed at Goldsmiths University as part of the MFA Computational Arts Program

4. Grover L.K.: A fast quantum mechanical algorithm for database search, Proceedings, 28th Annual ACM Symposium on the Theory of Computing, (May 1996) p. 212

5. King, D: DLib Introduction, http://dlib.net/intro.html

Jayson Haebich // www.jaysonh.com // mail@jaysonh.com



 

 