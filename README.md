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

Trained Models
-
We provide all trained models as follows. We name the model in the order of learning.

| Models | Description |
| --- | --- |
| [N.pth.tar](https://drive.google.com/file/d/1EF9rLkgvM5igo-yT6yVSj4hU_FoqjEiQ/view?usp=sharing) | Trained model on the NYU-v2 |
| [K.pth.tar](https://drive.google.com/file/d/1EF9rLkgvM5igo-yT6yVSj4hU_FoqjEiQ/view?usp=sharing) | Trained model on the KITTI |
| [S.pth.tar](https://drive.google.com/file/d/1IVmJ7-B5VV65PsjIgk4knQ4hhvbYOVqb/view?usp=sharing) | Trained model on the ScanNet |
| [NK.pth.tar](https://drive.google.com/file/d/1lXf9BFCflU5RNoNAGxWZQFDYAjTt7rMV/view?usp=sharing) | Trained model on the NYU-v2 and KITTI |
| [KN.pth.tar](https://drive.google.com/file/d/1EF9rLkgvM5igo-yT6yVSj4hU_FoqjEiQ/view?usp=sharing) | Trained model on the KITTI and NYU-v2|
| [NKS.pth.tar](https://drive.google.com/file/d/1lXf9BFCflU5RNoNAGxWZQFDYAjTt7rMV/view?usp=sharing) | Trained model on the NYU-v2, KITTI, and ScanNet |
| [NSK.pth.tar](https://drive.google.com/file/d/1lXf9BFCflU5RNoNAGxWZQFDYAjTt7rMV/view?usp=sharing) | Trained model on the NYU-v2, ScanNet, and KITTI |
| [SNK.pth.tar](https://drive.google.com/file/d/1ceKrFtlenwYyS6IKLOf3yWcQqYIo6ock/view?usp=sharing) | Trained model on the ScanNet, NYU-v2, and KITTI |
| [SKN.pth.tar](https://drive.google.com/file/d/1EyRf6HRMeRIbYNAEzM67yqMtB1HhWPJH/view?usp=sharing) | Trained model on the ScanNet, KITTI, and NYU-v2 |
| [KSN.pth.tar](https://drive.google.com/file/d/1EF9rLkgvM5igo-yT6yVSj4hU_FoqjEiQ/view?usp=sharing) | Trained model on the KITTI, ScanNet, and NYU-v2|
| [KNS.pth.tar](https://drive.google.com/file/d/1EF9rLkgvM5igo-yT6yVSj4hU_FoqjEiQ/view?usp=sharing) | Trained model on the KITTI, NYU-v2, and ScanNet |

Running
-
+ ### Test<br>
	 Testing with domain prior: python test.py<br>
	 Testing without domain prior: python test_inference.py<br>
+ ### Train<br>
	 Training on a single-domain: python train_N.py<br>
	 Training on two domains: python train_NK.py<br>
   Training on three domains: python train_NK.py<br>

