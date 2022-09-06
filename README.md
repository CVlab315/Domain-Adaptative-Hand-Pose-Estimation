
# Multiscale fusion based Domain Adaptative Hand Pose Estimation


# Installation

 python_requires='>=3.6'

 Install_requires:

  	 'torch>=1.7.0',
  	 'torchvision>=0.5.0',
  	 'numpy',
  	 'prettytable',
 	  'tqdm',
 	  'scikit-learn',
 	  'webcolors',
 	  'matplotlib'.
     
# Datasets

 [Rendered Handpose Dataset](https://lmb.informatik.uni-freiburg.de/resources/datasets/RenderedHandposeDataset.en.html) (synthetic dataset)
 
 [Hand-3d-Studio Dataset](https://www.yangangwang.com/papers/ZHAO-H3S-2020-02.html) (real-word dataset)
 
 [Stereo Hand Pose Tracking Benchmark](https://www.dropbox.com/sh/ve1yoar9fwrusz0/AAAfu7Fo4NqUB7Dn9AiN8pCca?dl=0) (real-world dataset) 



 #  Trained models
 
 The trained models can be found [here](https://drive.google.com/drive/folders/1qSaGgL0MzXq-B7QmJQSKFnHwXSMB1cL0?usp=sharing).

 
 
 # Run the code
 
 1. Evaluate on real-world dataset (H3D or STB).
    ```
    python test.py data/H3D -t Hand3DStudio --checkpoint  models/H3D_best_754.pth,
    python test.py data/STB -t STB --checkpoint  models/STB_best_750.pth
    ```
   
   
 2. Training.
    
    Run the following script:
    ```
    python train1.py data/H3D -t Hand3DStudio
    python train1.py data/STB -t STB
    ```
  
