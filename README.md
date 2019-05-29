# Research Papers
This repository is a collection of pre-prints of my published research papers.

## [Explicit Bit Minimization for Motion-Compensated Video Coding](dcc94.pdf)
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

## [Multiple-Dictionary Compression using Partial Matching](dcc95.pdf)

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

## [Efficient Cost Measures for Motion Compensation at Low Bit Rates](dcc96.pdf)

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

## [Dictionary Selection using Partial Matching](dpm99.pdf)

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

## Rate-Distortion Optimizations for Motion Estimation in Low-Bitrate Video Coding
D. T. Hoang, P. M. Long, and J. S. Vitter. "Rate-Distortion Optimizations for Motion Estimation in Low-Bitrate Video Coding," IEEE Transactions on Circuits and Systems for Video Technology, 8(4), August 1998, 488-500. A shorter version appears in Proceedings of the Digital Video Compression Conference, IS&T/SPIE 1996 Symposium on Electronic Imaging: Science & Technology, 2668, San Jose, CA, January-February 1996, 18-27.

We present and compare methods for choosing motion vectors for motion-compensated video coding. Our primary focus is on videophone and videoconferencing applications, where very low bit rates are necessary, where motion is usually limited, and where frames must be coded in the order they are generated. We provide evidence, using established benchmark videos typical of these applications, that choosing motion vectors explicitly to minimize rate, subject to implicit constraints on distortion, yields better rate-distortion tradeoffs than minimizing notions of prediction error. Minimizing a linear combination of rate and distortion results in further rate-distortion improvements. Using a heuristic function of the prediction error and the motion vector codelength results in compression performance comparable to the more computationally intensive coders while running much faster. We incorporate these ideas into coders that operate within the $p \times 64$ standard.


D. T. Hoang, E. Linzer, and J. S. Vitter, "Lexicographic Bit Allocation for MPEG Video," Special issue on high-fidelity media processing in Journal of Visual Communication and Image Representation, 8(4), December 1997, 384-404. An extended abstract appears in Proceedings of the 1997 IEEE International Conference on Image Processing (ICIP'97), Santa Barbara, CA, October 1997. A shorter version appears in "A Lexicographic Framework for MPEG Rate Control," Proceedings of the 1997 IEEE Data Compression Conference (DCC '97), Snowbird, UT, March 1997, 101-110.

D. T. Hoang and J. S. Vitter. Efficient Algorithms for MPEG Video Compression, John Wiley & Sons, New York, NY, 2002. The interplay between compression and buffer control algorithms in order to maximize network performance and achieve high visual clarity has shown great results, and Efficient Algorithms for MPEG Video Compression is the first book dedicated to the subject.

Video belongs to a class of information called continuous media. Continuous media is characterized by the essentially continuous manner in which the information is presented. This is in contrast to discrete media, in which there is no essential temporal component. Text, images, and graphics are examples of discrete media, while movies, sound, and computer animation are examples of continuous media. Even though a slide show is a time-based presentation of images, it is not a continuous medium since each image is viewed as an individual item. On the other hand, a video clip, while also consisting of a sequence of images, is a continuous medium since each image is perceived in the context of past and future images.

With continuous media, therefore, the temporal dimension becomes important. For example, a video sequence compressed with a constant image quality for every frame is often more desirable than one in which the image quality varies noticeably over time. However, because the compressibility of individual frames varies over time, maintaining a constant image quality results in a variation in coding rate over time. The process of controlling the coding rate to meet the requirements of a transmissions channel or storage device, while maintaining a desired level of quality, is called bit rate control. In this monograph, we focus on the rate control of compressed video. Specifically, we present a new framework for allocating bits to the compression of pictures in a video sequence.

Existing optimal rate control techniques typically regulate the coding rate to minimize a sum-distortion measure. While these techniques can leverage the wealth of tools from least-mean-square optimization theory, they do not guarantee constant-quality video, an objective often mentioned in the literature. In this book, we develop a framework that casts rate control as a resource allocation problem with continuous variables, nonlinear constraints, and a novel lexicographic optimality criterion that is motivated for uniform video quality. With the lexicographic criterion, we propose a new concept of coding efficiency to better reflect the constancy in quality that is generally desired from a video coder.

Rigorous analysis within this framework reveals a set of necessary and sufficient conditions for optimality for coding at both constant and variable bit rates. With these conditions, we are able to construct polynomial-time algorithms for optimal bit rate control. Experimental implementations of these algorithms confirm the theoretical analysis and produce encodings that are more uniform in quality than that achieved with existing rate control methods. As evidence of the generality and flexibility of the framework, we show how to extend the framework to allocate bits among multiple variable bit rate bitstreams that are to be transmitted over a common constant bit rate channel and to encompass the case of discrete variables.

## License
[CC-BY-NC-ND 4.0](https://creativecommons.org/licenses/by-nc-nd/4.0/)

