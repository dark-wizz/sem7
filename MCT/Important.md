### Part A
- **UNIT 1**
- [ ] What is source coding?  
> [!ans]- Ans
> Information theory where data is compressed to remove redundancy and represent the information in the most effective way possible
- [ ] quantization   
> [!ans]- Ans
> mapping large set of input to small set of output, involves converting continuous signal to discrete levels
- **UNIT 2**
- [ ] What is Huffman coding 
> [!ans]- Ans
> lossless data compression - variable length binary code - represent data based on its frequency - higher the freq shorter the code
- [ ] Why coding techniques are important for compression? 
> [!ans]- Ans
> reduce data - enhance effficiency - save storage
- **UNIT 3**
- [ ] How the audio compression is difference from video compression?   
> [!ans]- Ans
> audio - temporal, human auditory limitation
> video - spatial & temporal
- [ ] Applications of speech coding 
> [!ans]- Ans
> mobile comm (voIP, GSM)
> audio streaming, storage
> assistance
> encryption
- **UNIT 4**
- [ ] Why modulation is important for communication?
> [!ans]- Ans
> transmits signal over long distance by converting baseband signals into higher freq
> improve signal stregth, min interference, enabling multiplexing
- [ ] What is a predictive technique? 
> [!ans]- Ans
> estimates future value of a signal based on its past value
> used in compression to reduce redundancy by encoding only diff bt actual and predicted val.
- **UNIT 5**
- [ ] What is MPEG 
> [!ans]- Ans
> Moving Picture Standard Group - standard for compressing digital audio and video
> efficient streaming and storage (MPEG 1 2 4)
- [ ] Define motion estimation.  
> [!ans]- Ans
> detecting and analyzing the movement of object bt consecutive video frames 
> reduce temporal redundancy by encoding changes rather than entire frame

---
### Part B
- **UNIT 1**
- [ ] Define quantization error. 
> [!note]- Notes
> - diff b/w actual analog signal value and its quantized digital value
> - cont range of signal value apprx to finite set of discrete level
> - distortion - lossy compression
> `Qe = x - x^`
> - **Deterministic quan:** error are predictable - ip vals known
> - **indeterministic quan:** erroerappear randon - ip val complex
> - noise / blockiness in image an =d vido
> - **lossy**: error significant
> - **lossless**: error negligable
- [ ] How the performances are measured in the compression techniques? 
- **UNIT 2**
- [ ] Define Quality of measures?
- [ ] Define Arithmetic coding. 
>[!note]- Notes
> - lossless data compression
> - entire msg as single number - fraction bw 0 and 1
> -  probability based on symbols - skewed distribution
> **Encoding process**
> - symbols mapped - intervel line - 0 1
> - probabilty determine size interval - more freq symbol - large interval
> - msg reps as unique fractional value in the final interval
> **Decosing process**
> - fractional value used to trace back the seq of symbol - by identitify intervals corrs to each symbol
- [ ] Explain about vocoder? 
> [!note]- Notes
> **Analysis phase**
> - extract key characteristics - pitch from vocal tract shape
> - frequency band div
> **Synthesis phase**
> - reconstruct speech - modulated career signal 
> - intell - identofy the original speech
> **Application**
> - speech compression
> - music production
> - encryption
- **UNIT 3**
- [ ] Explain about sub band coding ? 
> [!note]- Notes
> - audio compression - divide multiple frequnecy band - encode seperately
> - difff freq - diff sensitivity
> - **signal analysis**
> 	 - filter banks
> - **downsampling**
> 	- down sample each band
> - **encoding**
> 	- qualtiized and encoded
> - **reconstructing**
> 	- deoceded - up sampled - combined (synthesis filters)
- [ ] What is Delta Modulation? 
- **UNIT 4**
- [ ] What is DPCM?
>[!note]- Note 
>advanced version of PCM
>reduces redundancy present in signals by encoding the difference bw successive sample values
>multple bits to reps diff - increase accuracy
> sample - diff bw actual & predicted sample - quantize - encode
- [ ] What is EZW? 
- **UNIT 5**
- [ ] Compare the differentiate between JPEG and MPEG  
- [ ] Summarize the difference between video and audio compression  
>[!note]- Notes
> | audio             | video                     |
> | ----------------- | ------------------------- |
> | temporal          | spatial, temporal         |
> | perceptual coding | motion estimation, quantz |
> | human hearing     | human vision sensitivity  |
> | low bitrate       | high bitrate              |
> | low compress rate | high compress rate        |


---
### Part C
**UNIT 1**
- [ ] Compare the scalar quantization and vector quantization with brief explanation.
- [ ] Develop the briefly explain about the Taxonomy of Multimedia Compression .
> [!note]- Notes
> - bit-rate reduction and source coding
> - save disk space and time
> 	- Lossless data compression
> 	- Lossy data compression
> ###### Lossless
> - w/o loosing quality and data
> - PNG, RAW, GIF, BMP
> 	- Run Length Encoding (RLE)
> 	- lempel Ziv - welch (LZW)
> 	- Huffman coding
> 	- Arithmetic coding 
> ###### Lossy
> - data and quality removed
> - JPEG, GIF, MP3, MP4, MKV, OGG
> - less memory
> 	- Transform coding
> 	- Discrete cosine transform (DCT)
> 	- Discrete wavelet transform (DWT)
> 
- **UNIT 2**
- [ ] Explain briefly about Huffman Algorithm.
> [!note]- Notes
> - text compression algo
> - characters -> coded datas
> - variable length codes
> - high freq symbol represented in min of bits
> - shannon feno top-down, its bottom-up
> - improvement oven shannon - fano algo
> ###### steps
> - arrange the fn sequence in descending order
> - last two into single new sourrce
> - again rearrage in dec order
> - continue this until only two new source msgs left
> - start assign codoes 0,1 in backward direction towrads initial
> 
- [ ] Infer the percentage of efficiency for Huffman Encoding procedure to the following message ensemble.
	```
	X={X1, X2, X3, X4, X5,X6} 
	i. P= {1/5,1/5,1/5,1/5,1/5,1/5}
	ii. P= {1/8,1/8,1/8,1/8,1/8,1/8}
	```
- **UNIT 3**
- [ ] explain briefly about the JPEG 
>[!note]- Notes
> ###### Joint photographic experts group
> ![[img/jpeg.png]]
> - Raw image data
> - color transform
> 	- RBG -> yCbCr
> 	- y - luminance
> 	- Cb - blue chrominance
> 	- Cr - red chrominance
> - downsampling
> - FDCT
> 	- 8x8 pixel blocks
> 	- spacial domain -> frequency domain
> 		- low-frequency components (more visual info)
> 		- high-frequency components (fine details and noise)
> - quantization
> 	- DCT coeff / quantization table and rounded
> 	- large the quantization value - less the precision (data loss)
> - zig-zag scanning
> 	- scans 8x8 quantized coeffs
> 	- this ensures low freq data stored first (imp data)
> 	- high freq data grouped at the end (less imp data)
> - AC and DC components
> 	- DC: first coff of each 8x8 block (avg color val)
> 		- DPCM(Differential pulse code modulation) applied to DC coeff - reduce redundancy
> 	- AC: remaining coefffs (details)
> - positive conversion
> 	- AC coefff -> positive range (simplify further encoding)
> - Huffman encodin
> 	- more the freq occ of value : less the length of binary code
> - create block of symbols (fixed 8 bits)
> - Arithmetic encoding
> 	- represents entire sequence of symbol as a single fractional value
> - compressed data
- [ ] Illustrate the principle of audio compression technique.
- **UNIT 4**
- [ ] Relate the principle of operation of PCM  and DPCM. 
> [!note]- Notes
> - analog compession
> - sampling analog signals -> digital form
> ###### PCM
> - remodels analog to digital signal
> - good signal to noise ratio
> - pcm needs high bandwidth for transmission channel
> - components
> 	- transmission end
> 	- regeneration
> 	- receiving end
> ![[pcm.png]]
> ###### DPCM
>  - moderate signal to noise ratio
>  - quantizes distinction of the particular sample and expected price
> ![[dpcm.png]]
> - current sample from previous sample
> - differential bw actual and predicted sample and that transmitted and encoded
> - low bandwidth
- [ ] Explain briefly about the Delta Modulation.  
- [ ] Explain briefly about the JBIG & SPIHT standards?
- **UNIT 5**
- [ ] Analyze the principle of operation of Motion estimation techniques.  
- [ ] Explain about DVI technology in mm.
> [!note]- Note
> - Digital Video Interface
> - high-quality digital video signals
> - developed by DDWG(Digital Display Working Group) - 1999
> ###### types
>  - DVI-A
> 	 - transmits analog signals
> - DVI-D
> 	- transmits digital signal
> - DVI-I
> 	- both analog and digital