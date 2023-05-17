# Lifelong-MonoDepth: Lifelong Learning for Multi-Domain Monocular Metric Depth Estimation

We present an efficient multi-head framework that enables lifelong, cross-domain, and scare-aware monocular depth learning. For more detailed information, please check our [paper](https://arxiv.org/pdf/2303.05050.pdf).

Results
-
Qualitative comparisons.

<p align="center">
 <img src="figs/res.png" alt="photo not available" width="80%" height="80%">
</p>


Datasets
-NYU-v2
-KITTI
-ScanNet

Running
-
+ ### Test<br>
	 Testing with domain prior: python test.py<br>
	 Testing without domain prior: python test_inference.py<br>
+ ### Train<br>
	 Training on a single-domain: python train_N.py<br>
	 Training on two domains: python train_NK.py<br>
   Training on three domains: python train_NK.py<br>

