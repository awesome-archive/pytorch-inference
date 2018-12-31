# Serving PyTorch Models in C++ on Windows10 platforms

## How to use

- Prepare Data

	examples/data/train/

		- 0
		- 1
		  .
		  .
		  .
		- n

	examples/data/test/

		- 0
		- 1
		  .
		  .
		  .
		- n


- Train Model
```
cd examples && python train.py
```

- Transform Model
```
cd examples && python transform_model.py
```

- Test Model
```
makefile/pytorch/pytorch.sln
```	
- Thirdparty

	thirdpart/

		- libtorch  
		- opencv 

## Environment

- Windows10
- VS2017
- CMake3.13
- CUDA10.0
- CUDNN7.3
- Pytorch1.0
- [Libtorch] (https://download.pytorch.org/libtorch/cu100/libtorch-win-shared-with-deps-latest.zip)
- [OpenCV4.0.1] (https://opencv.org/releases.html)

## Questions

- "torch.jit.trace" doesn’t support nn.DataParallel so far.

	
## Acknowledgement

- https://github.com/Wizaron/pytorch-cpp-inference

- https://zhuanlan.zhihu.com/p/52154049
