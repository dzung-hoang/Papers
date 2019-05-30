# Research Papers
This repository is a collection of pre-prints of my published research papers.

## Sequence Alignment / Custom Computing Machines

### [A Systolic Array for the Sequence Alignment Problem](cs92-22.pdf)

This report introduces a new systolic algorithm for the sequence alignment problem. This work builds upon an existing systolic array for computing the edit distance between two sequences. The alignment array is meant to be used as the second phase in a two-phase design with a modified edit distance array serving as the first phase. An implementation on the SPLASH programmable logic array is described. Because of the extensive pipelining in the systolic array, computing an alignment on the array takes that same amount of time as computing just the edit distance. Compared to conventional computers, SPLASH implementation performs several orders of magnitude faster. 

```
@techreport{
    CS92TR22,
    author="D. T. Hoang",
    title="A Systolic Array for the Sequence Alignment Problem",
    institution="Brown University, Dept. of Computer Science",
    number="CS-92-22",
    year=1992
}
```

### [FPGA Implementation of Systolic Sequence Alignment](fpl92.pdf)

This paper describes an implementation of a novel systolic array for sequence alignment on the SPLASH reconfigurable logic array. The systolic array operates in two phases. In the first phase, a sequence comparison array due to Lopresti is used to compute a matrix of distances which is stored in local RAM. In the second phase, the stored distances are used by the alignment array to produce a binary encoding of the sequence alignment. Preliminary benchmarks show that the SPLASH implementation performs several orders of magnitude faster than implementation on supercomputers.

```
@inproceedings{DBLP:conf/fpga/HoangL92,
  author    = {Dzung T. Hoang and
               Daniel P. Lopresti},
  title     = {{FPGA} Implementation of Systolic Sequence Alignment},
  booktitle = {Field-Programmable Gate Arrays: Architectures and Tools for Rapid
               Prototyping, Second International Workshop on Field-Programmable Logic
               and Applications, Vienna, Austria, August 31 - September 2, 1992,
               Selected Papers},
  pages     = {183--191},
  year      = {1992},
  crossref  = {DBLP:conf/fpga/1992},
  url       = {https://doi.org/10.1007/3-540-57091-8\_43},
  doi       = {10.1007/3-540-57091-8\_43},
  timestamp = {Tue, 14 May 2019 10:00:51 +0200},
  biburl    = {https://dblp.org/rec/bib/conf/fpga/HoangL92},
  bibsource = {dblp computer science bibliography, https://dblp.org}
}
```

### The Splash 2 Processor and Applications

**_Pre-print is not available._**

Splash 2 is an attached parallel processor in which the computing eZements are user programmable FPGA devices. The architecture of Splash 2 is designed to accelerate the solution of problems which exhibit at least modest amounts of temporal or data parallelism. Applications are developed by writing descrzplions of algorithms in VHDL, which are then iteratively refined and debugged widhin a simulator. Once an application is determined to be functionally correct in simulation, it is compiled to a gate list and optimized by logic synthesis. The gate list is then mapped onto the FPGA architecture by automatic placement and routing tools-to form a loadable FPGA object module. A C language library and a symbolic debugger comprise the execution environment. The Splash 2 system has been shown to be effective on a variety of applications, including text searching, sequence analysis, and image processing.

```
@inproceedings{DBLP:conf/iccd/ArnoldBHPST93,
  author    = {Jeffrey M. Arnold and
               Duncan A. Buell and
               Dzung T. Hoang and
               Daniel V. Pryor and
               Nabeel Shirazi and
               Mark R. Thistle},
  title     = {The Splash 2 Processor and Applications},
  booktitle = {Proceedings 1993 International Conference on Computer Design: {VLSI}
               in Computers {\&} Processors, {ICCD} '93, Cambridge, MA, USA,
               October 3-6, 1993},
  pages     = {482--485},
  year      = {1993},
  crossref  = {DBLP:conf/iccd/1993},
  url       = {https://doi.org/10.1109/ICCD.1993.393329},
  doi       = {10.1109/ICCD.1993.393329},
  timestamp = {Mon, 11 Feb 2019 17:32:53 +0100},
  biburl    = {https://dblp.org/rec/bib/conf/iccd/ArnoldBHPST93},
  bibsource = {dblp computer science bibliography, https://dblp.org}
}
```

### [Searching Genetic Databases on Splash 2](fccm93.pdf)

**_This paper was recognized as one of the 25 most significant papers from the first 20 years of IEEE International Symposium on Field-Programmable Custom Computing Machines (FCCM)._**
http://www.tcfpga.org/fccm20/fccm20endorsements.pdf

In this paper, we describe two systolic arrays for computing the edit distance between two genetic sequences using a well-known dynamic programming algorithm. The systolic arrays have been implemented for the Splash 2 programmable logic array, and are intended to be used for database searching. Simulations indicate that that the faster Splash 2 implementation can search a database at a rate of 12 million characters per second, several orders of magnitude faster than implementations of the dynamic programming algorithm on conventional computers.

```
@inproceedings{
    FCCM93,
    author="D. T. Hoang",
    title="Searching Genetic Databases on Splash 2",
    booktitle="Proceedings 1993 IEEE Workshop on Field-Programmable Custom Computing Machines",
    publisher="IEEE",
    year=1993,
    pages="185--192",
}
```

## Text Compression

### [Multiple-Dictionary Compression using Partial Matching](dcc95.pdf)

Motivated by the desire to find text compressors that compress better than existing dictionary methods, but run faster than PPM implementations, we describe methods for text compression using multiple dictionaries, one for each context of preceeding characters, where the contexts have varying lengths. The context to be used is determined using an escape mechanism similar to that of PPM methods. We describe modifications of three popular dictionary coders along these lines and experiments evaluating their efficacy using the text files in the Calgary corpus. Our results suggest that modifying LZ77 along these lines yields an improvement in compression of about 4%, that modifying LZFG yields a compression improvement of about 8%, and that modifying LZW in this manner yields an average improvement on the order of 12%.

```
@inproceedings{DBLP:conf/dcc/HoangLV95,
  author    = {Dzung T. Hoang and
               Philip M. Long and
               Jeffrey Scott Vitter},
  title     = {Multiple-Dictionary Coding Using Partial Matching},
  booktitle = {Proceedings of the {IEEE} Data Compression Conference, {DCC} 1995,
               Snowbird, Utah, USA, March 28-30, 1995.},
  pages     = {272--281},
  year      = {1995},
  crossref  = {DBLP:conf/dcc/1995},
  url       = {https://doi.org/10.1109/DCC.1995.515517},
  doi       = {10.1109/DCC.1995.515517},
  timestamp = {Wed, 20 Jun 2018 17:24:54 +0200},
  biburl    = {https://dblp.org/rec/bib/conf/dcc/HoangLV95},
  bibsource = {dblp computer science bibliography, https://dblp.org}
}
```

### [Dictionary Selection using Partial Matching](dpm99.pdf)

Motivated by the desire to find text compressors that compress better than existing dictionary methods, but run faster than PPM implementations, we describe methods for text compression using multiple dictionaries, one for each context of preceding characters, where the contexts have varying lengths. The context to be used is determined using an escape mechanism similar to that of PPM methods. We describe modifications of three popular dictionary coders along these lines and experiments evaluating their efficacy using the text files in the Calgary corpus. Our results suggest that modifying LZ77 along these lines yields an improvement in compression of about 4%, that modifying LZFG yields a compression improvement of about 8%, and that modifying LZW in this manner yields an average improvement on the order of 12%.

```
@article{DBLP:journals/isci/HoangLV99,
  author    = {Dzung T. Hoang and
               Philip M. Long and
               Jeffrey Scott Vitter},
  title     = {Dictionary Selection Using Partial Matching},
  journal   = {Inf. Sci.},
  volume    = {119},
  number    = {1-2},
  pages     = {57--72},
  year      = {1999},
  url       = {https://doi.org/10.1016/S0020-0255(99)00060-2},
  doi       = {10.1016/S0020-0255(99)00060-2},
  timestamp = {Sat, 27 May 2017 14:24:49 +0200},
  biburl    = {https://dblp.org/rec/bib/journals/isci/HoangLV99},
  bibsource = {dblp computer science bibliography, https://dblp.org}
}
```

## Video Compression

### [Explicit Bit Minimization for Motion-Compensated Video Coding](dcc94.pdf)
We compare methods for choosing motion vectors for motion-compensated video compression. Our primary focus is on videophone and videoconferencing applications, where very low bit rates are necessary, where the motion is usually limited, and where the frames must be coded in the order they are generated. We provide evidence, using established benchmark videos of this type, that choosing motion vectors to minimize codelength subject to (implicit) constraints on quality yields substantially better rate-distortion tradeoffs than minimizing notions of prediction error. We illustrate this point using an algorithm within the Px64 standard. We show that using quadtrees to code the motion vectors in conjunction with explicit codelength minimization yields further improvement. We describe a dynamic-programming algorithm for choosing a quadtree to minimize the codelength.

```
@inproceedings{DBLP:conf/dcc/HoangLV94,
  author    = {Dzung T. Hoang and
               Philip M. Long and
               Jeffrey Scott Vitter},
  title     = {Explicit Bit Minimization for Motion-Compensated Video Coding},
  booktitle = {Proceedings of the {IEEE} Data Compression Conference, {DCC} 1994,
               Snowbird, Utah, USA, March 29-31, 1994.},
  pages     = {175--184},
  year      = {1994},
  crossref  = {DBLP:conf/dcc/1994},
  url       = {https://doi.org/10.1109/DCC.1994.305925},
  doi       = {10.1109/DCC.1994.305925},
  timestamp = {Wed, 20 Jun 2018 17:24:41 +0200},
  biburl    = {https://dblp.org/rec/bib/conf/dcc/HoangLV94},
  bibsource = {dblp computer science bibliography, https://dblp.org}
}
```

### [Efficient Cost Measures for Motion Compensation at Low Bit Rates](dcc96.pdf)

We present and compare methods for choosing motion vectors for block-based motion-compensated video coding. The primary focus is on videophone and video-conferencing applications, where low bit rates are necessary, where motion is usually limited, and where the amount of computation is also limited. In a typical block-based motion-compensated video coding system, motion vectors are transmitted along with a lossy encoding of the residuals. As the bit rate decreases, the proportion required to transmit the motion vectors increases. We provide experimental evidence that choosing motion vectors explicitly to minimize rate (including motion vector coding), subject to implicit constraints on distortion, yields better rate-distortion tradeoffs than minimizing some measure of prediction error. Minimizing a combination of rate and distortion yields further improvements. Although these explicit-minimization schemes are computationally intensive, they provide invaluable insight which we use to develop practical algorithms. We show that minimizing a simple heuristic function of the prediction error and the motion vector code-length results in rate-distortion performance comparable to explicit-minimization schemes while being computationally feasible. Experimental results are 
provided for coders that operate within the H.261 standard.

```
@inproceedings{DBLP:conf/dcc/HoangLV96,
  author    = {Dzung T. Hoang and
               Philip M. Long and
               Jeffrey Scott Vitter},
  title     = {Efficient Cost Measures for Motion Compensation at Low Bit Rates (Extended
               Abstract)},
  booktitle = {Proceedings of the 6th Data Compression Conference {(DCC} '96), Snowbird,
               Utah, USA, March 31 - April 3, 1996.},
  pages     = {102--111},
  year      = {1996},
  crossref  = {DBLP:conf/dcc/1996},
  url       = {https://doi.org/10.1109/DCC.1996.488315},
  doi       = {10.1109/DCC.1996.488315},
  timestamp = {Wed, 20 Jun 2018 17:25:13 +0200},
  biburl    = {https://dblp.org/rec/bib/conf/dcc/HoangLV96},
  bibsource = {dblp computer science bibliography, https://dblp.org}
}

```

### [Rate-Distortion Optimizations for Motion Estimation in Low-Bitrate Video Coding](dvc96.pdf)

We make a case that taking the number of bits to code each motion vector into account when estimating motion for video compression results in significantly better performance at low bit rates, using simulation studies on established benchmark videos. First, by modifying a "vanilla" implementation of the H.261 standard, we show that choosing motion vectors explicitly to minimize rate (in a greedy manner), subject to implicit constraints on distortion, yields better rate-distortion tradeoffs than minimizing notions of prediction error. Locally minimizing a linear combination of rate and distortion results in further improvements. Using a heuristic function of the prediction error and the motion vector code-length results in compression performance comparable to the more computationally intensive coders while requiring a practically small amount of computation.  We also show that making coding control decisions to minimize rate yields further improvements.

```
@inproceedings{
    HLV96a,
    author="D. T. Hoang and P. M. Long and J. S. Vitter",
    title="Rate-Distortion Optimizations for Motion Estimation in Low-Bit-Rate Video Coding",
    booktitle="Proc.\ SPIE 2668, Digital Video Compression: {A}lgorithms and Technologies 1996",
    year=1996,
    pages="18--27",
    URL="https://doi.org/10.1117/12.235433",
}
```

### [Efficient Cost Measures for Motion Estimation at Low Bit Rates](itcsvt98.pdf)

We present and compare methods for choosing motion vectors for block-based motion-compensated video coding. The primary focus is on videophone and videoconferencing applications, where low bit rates are necessary, where motion is usually limited, and where the amount of computation is also limited. In a typical block-based motion-compensated video coding system, motion vectors are transmitted along with a lossy encoding of the residuals. As the bit rate decreases, the proportion required to transmit the motion vectors increases. We provide experimental evidence that choosing motion vectors explicitly to minimize rate (including motion vector coding), subject to implicit constraints on distortion, yields better rate-distortion tradeoffs than minimizing some measure of prediction error. Minimizing a combination of rate and distortion yields further improvements. Although these explicit-minimization schemes are computationally intensive, they provide invaluable insight which we use to develop practical algorithms. We show that minimizing a simple heuristic function of the prediction error and the motion vector code-length results in rate-distortion performance comparable to explicit-minimization schemes while being computationally feasible. Experimental results are provided for coders that operate within the H.261 standard.

```
@article{DBLP:journals/tcsv/HoangLV98,
  author    = {Dzung T. Hoang and
               Philip M. Long and
               Jeffrey Scott Vitter},
  title     = {Efficient cost measures for motion estimation at low bit rates},
  journal   = {{IEEE} Trans. Circuits Syst. Video Techn.},
  volume    = {8},
  number    = {4},
  pages     = {488--500},
  year      = {1998},
  url       = {https://doi.org/10.1109/76.709413},
  doi       = {10.1109/76.709413},
  timestamp = {Fri, 26 May 2017 22:51:14 +0200},
  biburl    = {https://dblp.org/rec/bib/journals/tcsv/HoangLV98},
  bibsource = {dblp computer science bibliography, https://dblp.org}
}
```

### [Lexicographic Bit Allocation for MPEG Video (Journal)](jvcir97.pdf)
### [Lexicographic Bit Allocation for MPEG Video Coding (ICIP'97)](icip97a.pdf)
### [A Lexicographic Framework for MPEG Rate Control (DCC'97)](dcc97.pdf)

We consider the problem of allocating bits among pictures in an MPEG video coder to equalize the visual quality of the coded pictures, while meeting buffer and channel constraints imposed by the MPEG Video Buffering Verifier. We address this problem within a framework that consists of three components: 1) a bit production model for the input pictures, 2) a set of bit-rate constraints imposed by the Video Buffering Verifier, and 3) a novel lexicographic criterion for optimality. Under this framework, we derive simple necessary and sufficient conditions for optimality that lead to efficient algorithms.

```
@article{DBLP:journals/jvcir/HoangLV97,
  author    = {Dzung T. Hoang and
               Elliot L. Linzer and
               Jeffrey Scott Vitter},
  title     = {Lexicographic Bit Allocation for {MPEG} Video},
  journal   = {J. Visual Communication and Image Representation},
  volume    = {8},
  number    = {4},
  pages     = {384--404},
  year      = {1997},
  url       = {https://doi.org/10.1006/jvci.1997.0376},
  doi       = {10.1006/jvci.1997.0376},
  timestamp = {Thu, 18 May 2017 09:52:12 +0200},
  biburl    = {https://dblp.org/rec/bib/journals/jvcir/HoangLV97},
  bibsource = {dblp computer science bibliography, https://dblp.org}
}

@inproceedings{DBLP:conf/icip/HoangVL97,
  author    = {Dzung T. Hoang and
               Jeffrey Scott Vitter and
               Elliot L. Linzer},
  title     = {Lexicographic Bit Allocation for {MPEG} Video Coding},
  booktitle = {Proceedings 1997 International Conference on Image Processing, {ICIP}
               '97, Santa Barbara, California, USA, October 26-29, 1997},
  pages     = {322--325},
  year      = {1997},
  crossref  = {DBLP:conf/icip/1997},
  url       = {https://doi.org/10.1109/ICIP.1997.647771},
  doi       = {10.1109/ICIP.1997.647771},
  timestamp = {Thu, 25 May 2017 00:40:36 +0200},
  biburl    = {https://dblp.org/rec/bib/conf/icip/HoangVL97},
  bibsource = {dblp computer science bibliography, https://dblp.org}
}

@inproceedings{DBLP:conf/dcc/HoangLV97,
  author    = {Dzung T. Hoang and
               Elliot L. Linzer and
               Jeffrey Scott Vitter},
  title     = {A Lexicographic Framework for {MPEG} Rate Control},
  booktitle = {Proceedings of the 7th Data Compression Conference {(DCC} '97), Snowbird,
               Utah, USA, March 25-27, 1997.},
  pages     = {101--110},
  year      = {1997},
  crossref  = {DBLP:conf/dcc/1997},
  url       = {https://doi.org/10.1109/DCC.1997.581982},
  doi       = {10.1109/DCC.1997.581982},
  timestamp = {Wed, 20 Jun 2018 17:25:39 +0200},
  biburl    = {https://dblp.org/rec/bib/conf/dcc/HoangLV97},
  bibsource = {dblp computer science bibliography, https://dblp.org}
}
```

### [Multiplexing VBR Video Sequences onto a CBR Channel with Lexicographic Optimization](icip97b.pdf)

We apply a novel lexicographic framework for bit allocation to the multiplexing of multiple VBR video streams onto a single CBR channel. In the lexicographic framework, the maximum distortion is minimized, then the second highest distortion, and so on, resulting in nearly constant quality. With a suitably constructed multiplexing model, we show that the multiplexing problem reduces to a single-stream CBR bit allocation problem, to which we apply the lexicographic framework. This method has applications for video servers, especially for near-video-on-demand.

```
@inproceedings{DBLP:conf/icip/HoangV97,
  author    = {Dzung T. Hoang and
               Jeffrey Scott Vitter},
  title     = {Multiplexing {VBR} Video Sequences onto a {CBR} Channel with Lexicographic
               Optimization},
  booktitle = {Proceedings 1997 International Conference on Image Processing, {ICIP}
               '97, Santa Barbara, California, USA, October 26-29, 1997},
  pages     = {369--372},
  year      = {1997},
  crossref  = {DBLP:conf/icip/1997},
  url       = {https://doi.org/10.1109/ICIP.1997.647783},
  doi       = {10.1109/ICIP.1997.647783},
  timestamp = {Thu, 25 May 2017 00:40:32 +0200},
  biburl    = {https://dblp.org/rec/bib/conf/icip/HoangV97},
  bibsource = {dblp computer science bibliography, https://dblp.org}
}
```

### [Real-Time VBR Rate Control of MPEG Video based upon Lexicographic Bit Allocation (Journal)](rti99.pdf)

The MPEG-2 Video Standard describes in detail a bitstream syntax and a decoder model but leaves many details of the encoding process unspecified, such as encoder bit rate control. The standard defines a hypothetical decoder model, called the Video Buffering Verifier (VBV), that can operate in either constant-bit-rate (CBR) or variable-bit-rate (VBR) modes. In this paper, we present a low-complexity algorithm for VBR rate control suitable for low-delay, real-time applications. The algorithm is motivated by recent results in lexicographic optimal bit allocation. The basic algorithm switches between constant-quality and constant-bit-rate modes based on changes in the fullness of the VBV buffer. We show how the algorithm can be applied either to produce a desired quality level or to meet a global bit budget. Simulation results show that the algorithm compares favorably to the optimal VBR algorithm.

```
@article{DBLP:journals/rti/Hoang99,
  author    = {Dzung T. Hoang},
  title     = {Real-Time {VBR} Rate Control of {MPEG} Video based upon Lexicographic
               Bit Allocation},
  journal   = {Real-Time Imaging},
  volume    = {5},
  number    = {5},
  pages     = {365--375},
  year      = {1999},
  url       = {https://doi.org/10.1006/rtim.1998.0168},
  doi       = {10.1006/rtim.1998.0168},
  timestamp = {Thu, 18 May 2017 09:51:49 +0200},
  biburl    = {https://dblp.org/rec/bib/journals/rti/Hoang99},
  bibsource = {dblp computer science bibliography, https://dblp.org}
}

@inproceedings{DBLP:conf/dcc/Hoang99,
  author    = {Dzung T. Hoang},
  title     = {Real-Time {VBR} Rate Control of {MPEG} Video Based upon Lexicographic
               Bit Allocation},
  booktitle = {Data Compression Conference, {DCC} 1999, Snowbird, Utah, USA, March
               29-31, 1999.},
  pages     = {374--383},
  year      = {1999},
  crossref  = {DBLP:conf/dcc/1999},
  url       = {https://doi.org/10.1109/DCC.1999.755687},
  doi       = {10.1109/DCC.1999.755687},
  timestamp = {Tue, 23 May 2017 01:07:02 +0200},
  biburl    = {https://dblp.org/rec/bib/conf/dcc/Hoang99},
  bibsource = {dblp computer science bibliography, https://dblp.org}
}
```
## Ph.D. Thesis

### [Fast and Efficient Algorithms for Text and Video Compression](thesis97.pdf)

There is a tradeoff between the speed of a data compressor and the level of compression it can achieve. Improving compression generally requires more computation; and improving speed generally sacrifices compression. In this thesis, we examine a range of tradeoffs for text and video. In text compression, we attempt to bridge the gap between statistical techniques, which exhibit a greater amount of compression but are computationally intensive, and dictionary-based techniques, which give less compression but run faster. We combine the context modeling of statistical coding with dynamic dictionaries into a hybrid coding scheme we call Dictionary by Partial Matching. In low-bit-rate video compression, we explore the speed-compression tradeoffs with a range of motion estimation techniques operating within the H.261 video coding standard. We initially consider algorithms that explicitly minimizes bit rate and combination of rate and distortion. With insights gained from the explicit minimization algorithms, we propose a new technique for motion estimation that minimizes an efficiently computed heuristic function. The new technique gives compression efficiency comparable to the explicit-minimization algorithms while running much faster. We also explore bit-minimization in a non-standard quadtree-based video coder that codes motion information hierarchically using variable-sized blocks. For video coding at medium-to-high bit rates, we propose a framework that casts rate control as a resource allocation problem with continuous variables, non-linear constraints, and a novel lexicographic optimality criterion motivated for near-constant-quality video. With this framework, we redefine the concept of efficiency to better reflect the constancy in quality generally desired from a video coder. Rigorous analysis within this framework reveals elegant conditions for optimality, which leads to polynomial-time algorithms. Simulation studies confirm the theoretical analysis and produce encodings that are more constant in quality than that achieved with existing rate control methods. As evidence of the flexibility of the framework, we show how to extend it to allocate bits among multiple variable-bit-rate bitstreams for transmission over a constant-bit-rate channel.

```
@phdthesis{Hoang97,
    title="Fast and Efficient Algorithms for Text and Video Compression",
    school="Brown University",
    author="Dzung T. Hoang",
    year=1997,
}
```

## License
The papers included here are licensed under [CC-BY-NC-ND 4.0](https://creativecommons.org/licenses/by-nc-nd/4.0/)
