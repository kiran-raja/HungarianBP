# HungarianBP: Pairwise Matching through Max-Weight Bipartite Belief Propagation

### Introduction
This repository contains the source code of the algorithm described in a [CVPR 2016](http://www.pamitc.org/cvpr16/) paper [Pairwise Matching through Max-Weight Bipartite Belief Propagation](https://zzhang.org/pdfs/ZhangEtal2016Cvpr.pdf). More details are provided on the [project page] (https://zzhang.org/featurematching.html).
This packages has been tested using Matlab R2015b on CentOS 7.0 (a distrubition of Linux) x64.

### Citing HungarianBP

If you find HungarianBP useful in your research, please consider citing:

    @inproceedings{Zhang:2016:CVPR,
        author = {Zhang, Zhen and Shi, Qinfeng and McAuley, Julian and Wei, Wei and Zhang, Yanning and Hengel, Anton},
        booktitle = {CVPR},
        title = {Pairwise Matching through {Max-Weight} Bipartite Belief Propagation},
        year = {2016}, 
    }

### Usage
0. **Prerequisites** 
 0. [Boost] (http://www.boost.org/): Install the boost library via apt-get, yum, or compiling from scratch.
 1. [Matlab] (http://www.mathworks.com/): Install Matlab.

0. **Configuring HungarianBP**
 0. Downloading HungarianBP via 
 
	```
        git clone https://github.com/zzhang1987/HungarianBP
	```
 1. Fetching the mex code via 
 
	```
		cd HungarianBP 
        git submodule init
		git submodule update --remote	
	```
 2. Run compiling.m.
 
	```	
		matlab
		#inside matlab 
			cd HungarianBP
			compiling
	```
 3. Run ``demoCar.m`` and ``demoMotor.m`` to reproduce the results on the [Cars and Motorbikes Dataset] (https://sites.google.com/site/graphmatchingmethods/). Run ``demoCharater.m`` to reproduce the results on the [Chinese Character dataset] (http://www.escience.cn/system/file?fileId=62549). 

### Remarks
Precompiled mex files for linux x64 are included. For other platforms, you can use any compilier that supports matlab and c++11 to compile the mex files.
	
### Feedback

If you have any issues (question, feedback) or find bugs in the code, please contact zhangzhen@mail.nwpu.edu.cn.



