# Research Papers
This repository is a collection of pre-prints of my published research papers.

## Text Compression

### [Multiple-Dictionary Compression using Partial Matching](dcc95.pdf)

Motivated by the desire to find text compressors that compress better than existing dictionary methods, but run faster than PPM implementations, we describe methods for text compression using multiple dictionaries, one for each context of preceeding characters, where the contexts have varying lengths. The context to be used is determined using an escape mechanism similar to that of PPM methods. We describe modifications of three popular dictionary coders along these lines and experiments evaluating their efficacy using the text files in the Calgary corpus. Our results suggest that modifying LZ77 along these lines yields an improvement in compression of about 4%, that modifying LZFG yields a compression improvement of about 8%, and that modifying LZW in this manner yields an average improvement on the order of 12%.

```
@inproceedings{
HLV95b,
author="D. T. Hoang and P. M. Long and J. S. Vitter",
title="Multiple-Dictionary Compression using Partial Matching",
booktitle="Proceedings 1995 Data Compression Conference",
publisher="IEEE Computer Society Press",
month=mar,
year=1995
pages="272--281",
}
```

### [Dictionary Selection using Partial Matching](dpm99.pdf)

Motivated by the desire to find text compressors that compress better than existing dictionary methods, but run faster than PPM implementations, we describe methods for text compression using multiple dictionaries, one for each context of preceding characters, where the contexts have varying lengths. The context to be used is determined using an escape mechanism similar to that of PPM methods. We describe modifications of three popular dictionary coders along these lines and experiments evaluating their efficacy using the text files in the Calgary corpus. Our results suggest that modifying LZ77 along these lines yields an improvement in compression of about 4%, that modifying LZFG yields a compression improvement of about 8%, and that modifying LZW in this manner yields an average improvement on the order of 12%.

```
@article{
HLV99DictionarySelection,
author="D. T. Hoang and P. M. Long and J. S. Vitter",
title="Dictionary Selection using Partial Matching",
journal="Information Sciences",
volume="119",
number="1--2",
year=1999,
pages="57--72",
}
```

## Video Compression

### [Explicit Bit Minimization for Motion-Compensated Video Coding](dcc94.pdf)
We compare methods for choosing motion vectors for motion-compensated video compression. Our primary focus is on videophone and videoconferencing applications, where very low bit rates are necessary, where the motion is usually limited, and where the frames must be coded in the order they are generated. We provide evidence, using established benchmark videos of this type, that choosing motion vectors to minimize codelength subject to (implicit) constraints on quality yields substantially better rate-distortion tradeoffs than minimizing notions of prediction error. We illustrate this point using an algorithm within the $p \times 64$ standard. We show that using quadtrees to code the motion vectors in conjunction with explicit codelength minimization yields further improvement. We describe a dynamic-programming algorithm for choosing a quadtree to minimize the codelength.

```
@inproceedings{
HLV94,
author="D. T. Hoang and P. M. Long and J. S. Vitter",
title="Explicit Bit-Minimization for Motion-Compensated Video Coding",
booktitle="Proceedings 1994 Data Compression Conference",
publisher="IEEE Computer Society Press",
month=mar,
year=1994,
pages="175--184"
}
```

### [Efficient Cost Measures for Motion Compensation at Low Bit Rates](dcc96.pdf)

We present and compare methods for choosing motion vectors for block-based motion-compensated video coding. The primary focus is on videophone and video-conferencing applications, where low bit rates are necessary, where motion is usually limited, and where the amount of computation is also limited. In a typical block-based motion-compensated video coding system, motion vectors are transmitted along with a lossy encoding of the residuals. As the bit rate decreases, the proportion required to transmit the motion vectors increases. We provide experimental evidence that choosing motion vectors explicitly to minimize rate (including motion vector coding), subject to implicit constraints on distortion, yields better rate-distortion tradeoffs than minimizing some measure of prediction error. Minimizing a combination of rate and distortion yields further improvements. Although these explicit-minimization schemes are computationally intensive, they provide invaluable insight which we use to develop practical algorithms. We show that minimizing a simple heuristic function of the prediction error and the motion vector code-length results in rate-distortion performance comparable to explicit-minimization schemes while being computationally feasible. Experimental results are 
provided for coders that operate within the H.261 standard.

```
@inproceedings{
HLV96b,
author="D. T. Hoang and P. M. Long and J. S. Vitter",
title="Efficient Cost Measures for Motion Compensation at Low Bit Rates",
booktitle="Proceedings 1996 Data Compression Conference",
publisher="IEEE Computer Society Press",
pages="102--111",
month=mar,
year=1996
}
```

### [Rate-Distortion Optimizations for Motion Estimation in Low-Bitrate Video Coding](dvm96)

We make a case that taking the number of bits to code each motion vector into account when estimating motion for video compression results in significantly better performance at low bit rates, using simulation studies on established benchmark videos. First, by modifying a "vanilla" implementation of the H.261 standard, we show that choosing motion vectors explicitly to minimize rate (in a greedy manner), subject to implicit constraints on distortion, yields better rate-distortion tradeoffs than minimizing notions of prediction error. Locally minimizing a linear combination of rate and distortion results in further improvements. Using a heuristic function of the prediction error and the motion vector code-length results in compression performance comparable to the more computationally intensive coders while requiring a practically small amount of computation.  We also show that making coding control decisions to minimize rate yields further improvements.

```
@inproceedings{
HLV96a,
author="D. T. Hoang and P. M. Long and J. S. Vitter",
title="Rate-Distortion Optimizations for Motion Estimation in Low-Bit-Rate Video Coding",
booktitle="Proc.\ SPIE 2668, Digital Video Compression: {A}lgorithms and Technologies 1996",
year=1996,
pages="18--27",
doi="10.1117/12.235433",
URL="https://doi.org/10.1117/12.235433",
}
```

### [Efficient Cost Measures for Motion Estimation at Low Bit Rates](itcsvt98.pdf)

We present and compare methods for choosing motion vectors for block-based motion-compensated video coding. The primary focus is on videophone and videoconferencing applications, where low bit rates are necessary, where motion is usually limited, and where the amount of computation is also limited. In a typical block-based motion-compensated video coding system, motion vectors are transmitted along with a lossy encoding of the residuals. As the bit rate decreases, the proportion required to transmit the motion vectors increases. We provide experimental evidence that choosing motion vectors explicitly to minimize rate (including motion vector coding), subject to implicit constraints on distortion, yields better rate-distortion tradeoffs than minimizing some measure of prediction error. Minimizing a combination of rate and distortion yields further improvements. Although these explicit-minimization schemes are computationally intensive, they provide invaluable insight which we use to develop practical algorithms. We show that minimizing a simple heuristic function of the prediction error and the motion vector code-length results in rate-distortion performance comparable to explicit-minimization schemes while being computationally feasible. Experimental results are provided for coders that operate within the H.261 standard.

```
@article{
HLV98EfficientMotionEstimation,
author="D. T. Hoang and P. M. Long and J. S. Vitter",
title="Efficient Cost Measures for Motion Estimation at Low Bit Rates",
journal="IEEE Trans. on Circuit and Systems for Video Technology",
volume="8",
number="4",
year=1998,
pages="488--500",
doi="10.1109/76.709413",
URL="https://doi.org/10.1109/76.709413",
}
```

### [Lexicographic Bit Allocation for MPEG Video](jvcir97.pdf)

We consider the problem of allocating bits among pictures in an MPEG video coder to equalize the visual quality of the coded pictures, while meeting buffer and channel constraints imposed by the MPEG Video Buffering Verifier. We address this problem within a framework that consists of three components: 1) a bit production model for the input pictures, 2) a set of bit-rate constraints imposed by the Video Buffering Verifier, and 3) a novel lexicographic criterion for optimality. Under this framework, we derive simple necessary and sufficient conditions for optimality that lead to efficient algorithms.

```
@article{
HLiV98Lexicographic,
author="D. T. Hoang and E. Linzer and J. S. Vitter",
title="Lexicographic Bit Allocation for MPEG Video",
journal="Journal of Visual Communication and Image Representation",
volume="8",
number="4",
year=1997,
pages="384--404",
URL="https://doi.org/10.1006/jvci.1997.0376",
}
```

## License
The papers included here are licensed under [CC-BY-NC-ND 4.0](https://creativecommons.org/licenses/by-nc-nd/4.0/)
