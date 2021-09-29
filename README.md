# DB-AIAT: A Dual-branch attention-in-attention transformer for single-channel SE
This is the repo of the manuscript "Dual-branch Attention-In-Attention Transformer for speech enhancement", which is to be submitted to ICASSP2022.
 The source code will be released soon!


Abstract：Curriculum learning begins to thrive in the speech enhancement area, which decouples the original spectrum estimation task into multiple easier sub-tasks to achieve better performance. Motivated by that, we propose a dual-branch attention-in-attention transformer-based module dubbed DB-AIAT to handle both coarse- and fine-grained regions of spectrum in parallel. From a complementary perspective, a magnitude masking branch is proposed to estimate the overall spectral magnitude, while a complex refining branch is designed to compensate for the missing complex spectral details and implicitly derive phase information. Within each branch, we propose a novel attention-in-attention transformer-based module to replace the conventional RNNs and temporal convolutional network for temporal sequence modeling. Specifically, the proposed attention-in-attention transformer consists of adaptive temporal-frequency attention transformer blocks and an adaptive hierarchical attention module, which can capture long-term time-frequency dependencies and further aggregate global hierarchical contextual information. The experimental results on VoiceBank + Demand dataset show that DB-AIAT yields state-of-the-art performance (e.g., 3.31 PESQ, 94.7% STOI and 10.79dB SSNR) over previous advanced systems with a relatively light model size (2.81M).

Network architecture:

![image](https://user-images.githubusercontent.com/51236251/135278429-6099d5da-c826-4aa2-8cca-b7c774beb14a.png)

![image](https://user-images.githubusercontent.com/51236251/135278803-b6769574-e70f-480b-8cb1-6a9934328844.png)



Comparison with SOTA:

![Experimental resulst](https://user-images.githubusercontent.com/51236251/134447067-15506636-9dbb-426f-894c-eafcf28940a3.PNG)

Ablation study:

![image](https://user-images.githubusercontent.com/51236251/134447114-74429af8-7c10-465d-8a1e-ddf0ec636b4e.png)
