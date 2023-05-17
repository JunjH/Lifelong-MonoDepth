# Lifelong-MonoDepth: Lifelong Learning for Multi-Domain Monocular Metric Depth Estimation

We present an efficient multi-head framework that enables lifelong, cross-domain, and scare-aware monocular depth learning. For more detailed information, please check our [paper](https://arxiv.org/pdf/2303.05050.pdf).

Results
-
Qualitative comparisons.

<p align="center">
 <img src="figs/res.png" alt="photo not available" width="80%" height="80%">
</p>


Datasets
-
We provided data index of RGB and depth pairs for both training and test set of all three datasets in csv file, you can find them in ./datasets/. Then, download the data required for training and test.

+ NYU-v2, download via the [link](https://drive.google.com/file/d/1WoOZOBpOWfmwe7bknWS5PMUCLBPFKTOw/view?usp=sharing) <br>
+ KITTI, download via the [official homepage](https://www.cvlibs.net/datasets/kitti/eval_depth.php?benchmark=depth_prediction)<br>
+ ScanNet, download via the [official homepage](http://www.scan-net.org/#code-and-data)<br>

Running
-
+ ### Test<br>
	 Testing with domain prior: python test.py<br>
	 Testing without domain prior: python test_inference.py<br>
+ ### Train<br>
	 Training on a single-domain: python train_N.py<br>
	 Training on two domains: python train_NK.py<br>
   Training on three domains: python train_NK.py<br>

