### Part A
- **UNIT 1**
- [ ] What is source coding?  
> [!ans]- Ans
> Information theory where data is compressed to remove redundancy and represent the information in the most effective way possible
- [ ] quantization   
- **UNIT 2**
- [ ] What is Huffman coding 
- [ ] Why coding techniques are important for compression? 
- **UNIT 3**
- [ ] How the audio compression is difference from video compression?   
- [ ] Applications of speech coding 
- **UNIT 4**
- [ ] Why modulation is important for communication?
- [ ] What is a predictive technique? 
- **UNIT 5**
- [ ] What is MPEG 
- [ ] Define motion estimation.  

---
### Part B
- **UNIT 1**
- [ ] Define quantization error. 
- [ ] How the performances are measured in the compression techniques? 
- **UNIT 2**
- [ ] Define Quality of measures?
- [ ] Define Arithmetic coding. 
- [ ] Explain about vocoder? 
- **UNIT 3**
- [ ] Explain about sub band coding ? 
- [ ] What is Delta Modulation? 
- **UNIT 4**
- [ ] What is DPCM?
- [ ] What is EZW? 
- **UNIT 5**
- [ ] Compare the differentiate between JPEG and MPEG  
- [ ] Summarize the difference between video and audio compression  

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
- [ ] Explain briefly about the Delta Modulation.  
- [ ] Explain briefly about the JBIG & SPIHT standards?
- **UNIT 5**
- [ ] Analyze the principle of operation of Motion estimation techniques.  
- [ ] Explain about DVI technology in mm.