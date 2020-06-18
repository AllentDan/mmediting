# Deep Image Matting

## Introduction

```
@inproceedings{xu2017deep,
  title={Deep image matting},
  author={Xu, Ning and Price, Brian and Cohen, Scott and Huang, Thomas},
  booktitle={Proceedings of the IEEE Conference on Computer Vision and Pattern Recognition},
  pages={2970--2979},
  year={2017}
}
```

## Results and Models

|   Method   |  SAD |  MSE  | GRAD | CONN | Download |
|:----------:|:----:|:-----:|:----:|:----:|:--------:|
| stage1 (paper) | 54.6  | 0.017  | 36.7  | 55.3 | - |
| stage3 (paper) | **50.4**  | **0.014**  | 31.0  | 50.8 | - |
| stage1 (our) | 53.8 | 0.017 | 32.7 | 54.5 | [model](TODO) \| [log](TODO) |
| stage2 (our) | 52.3 | 0.016 | 29.4 | 52.4 | [model](TODO) \| [log](TODO) |
| stage3 (our) | 50.6 | 0.015 | **29.0** | **50.7** | [model](TODO) \| [log](TODO) |

> stage1: train the encoder-decoder part without the refinement part. \
> stage2: fix the encoder-decoder part and train the refinement part. \
> stage3: fine-tune the whole network.