# introduction

ofxQuantum is part of an ongoing project to investigate Quantum Computing using artistic methods and practices. This project is being developed during my MFA in computational arts at Goldsmiths University London. This piece of a software is the first step in this process and began from the idea of creating theoretical software libraries for hardware that does not exist yet and working with alternative forms of computing. 

The aim of this openframeworks addon is to create a bridge between openframeworks which is a tool that is very popular amongst creative coders and new media artists and quantum computing which is a branch of abstract computing which only exists theoretically at this time but presents a substantial leap in computational power compared with classical computing techniques used in modern computers, laptops and phones. In this way I am providing a tool for the future that may possibly be used one day by artists but at this time is nothing more than an intellectual curiosity.

This project was inspired by my interest in mathematics and computational theory and to develop theoretically and conceptual software and present it to an audience who would not normally be interested in the field of theoretical computing. Programming and software design can be very practical and is mostly put to non poetic or practical creative uses so I wanted to make software that is more conceptual and artistic but also may have some practical use at some point even if it can't be used for anything practical at the moment. The reason that I choose quantum computing is that I am fascinated with the way that something as random and seemingly uncontrollable such as quantum mechanics can be put into a mathematical logic that can be used for computation.

# what is quantum computing?

Quantum comping is an area of computing first formulated by several computer theorists in the early
1980s (1)(2)(3). Quantum computing which uses the effects of quantum mechanics to perform computational tasks. While
classical computing uses a binary 1/0 bit quantum computing uses a Qubit which holds a superposition
of states between 1 and 0 and works within a world that is filled with probabilities rather than
solid deterministic type variables. This allows a quantum computer to work with bits that hold the probability
of the bit being in a state of 1 or 0 and with some clever algorithm design can compute the results across all posssible solutions to a problem. Another interesting feature of quantum computing is that quantum bits exist in a probability of being in a certain state until the bit is measured. This allows for the use of quantum computing to solve problems that are currently too coputationally heavy to solve on a
classical computer.

In a way quantum computing is a fitting embodiement of Konrad Zuse's concept of the Rechnender Raum which is the idea that the universe itself is a giant computing device (4). This concept is becoming more and more aparent as scientists unravel the mysterious behind dna, quantum physics, and other physical processes all of which are structured around computationally driven processes.

# about this addon

This addon implements the dlib library dlib.net which is an open source c++ library by David King to do various abstract computing methods and apply these to real world problems (5) The addon acts as a wrapper to make the implementation of quantum algorithms easier and provides open frameworks programmers with easy access to a quantum computing simulation library. The underlying software library can be seen to be irrelevant to the higher level wrapper ofxQuantum.h which is the main point of entry for the code.

# examples

SimpleHadamardGateExample - Simple example showing the output from a hadamard gate (6)

GroversSearchAlgorithmExample - Shows an implementation of Grovers search algorithm (7)

These must be placed in the myApps folder openframeworks/apps/myapps (or folder of equal directory depth)

# usage
This addon works with the project generator on OF 8.4 and 9.0 with xcode (osx) and Visual Studio 2015 (windows 8)

The basic usage of the addon is through the ofxQuantum class, the basic usage is:

```c++
ofxQuantum qSim;	 	// Create ofxQuantum object

qSim.init(1);			// Initialise the simulator with 1 bit

qSim.applyGateX(0);		// Apply the Pauli X gate to the first bit

qSim.measureBit(0);		// Measure the first bit

```

# hardware development

This work is part of an ongoing project into the investigation of quantum computing through artistic methods and processes. This project also includes the development of various hardware components that use real world quantum effects components that can be used with this ofxQuantum addon. One of these components is the Quantum State Observation Seed Generation Unit which allows the addon to measure the state of qubits using random numbers seeded from the quantum effects of the decay of a uranium atom. 

# references

1. Benioff, Paul (1980). "The computer as a physical system: A microscopic quantum mechanical Hamiltonian model of computers as represented by Turing machines". Journal of statistical physics 22 (5): 563–591.

2. Manin, Yu. I. (1980). Vychislimoe i nevychislimoe [Computable and Noncomputable] (in Russian). Sov.Radio. pp. 13–15. Retrieved 2013-03-04.

3. Feynman, R. P. (1982). "Simulating physics with computers". International Journal of Theoretical Physics 21 (6): 467–488. Bibcode:1982IJTP...21..467F. doi:10.1007/BF02650179.
Developed at Goldsmiths University as part of the MFA Computational Arts Program

4. Zuse, K., (2013). Rechnender raum. Springer-Verlag.

5. King, D: DLib Introduction, http://dlib.net/intro.html

6. Tipsmark, A., Dong, R., Laghaout, A., Marek, P., Ježek, M. and Andersen, U.L., (2011) Experimental demonstration of a Hadamard gate for coherent state qubits. Physical Review A, 84(5), p.050301.

7. Grover L.K.: A fast quantum mechanical algorithm for database search, Proceedings, 28th Annual ACM Symposium on the Theory of Computing, (May 1996) p. 212


# contact

Jayson Haebich // www.jaysonh.com // mail@jaysonh.com



 

 