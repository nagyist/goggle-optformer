# OptFormer: Transformer-based framework for Hyperparameter Optimization
This is the code used for the paper [Towards Learning Universal Hyperparameter Optimizers with Transformers (NeurIPS 2022)](https://arxiv.org/abs/2205.13320).

# Installation
All dependencies can be installed in `requirements.txt`. The two main components are [T5X](https://github.com/google-research/t5x) and [OSS Vizier](https://github.com/google/vizier).

# Usage

## Pre-trained OptFormer as a Policy
To use our pre-trained OptFormer (exactly as-is from the paper), follow the steps:

1. Download the model checkpoint from [TODO].
2. Load the model checkpoint into the `InferenceModel`, as shown in [policies_test.py](https://github.com/google-research/optformer/blob/main/optformer/t5x/policies.py).

The `InferenceModel` will then be wrapped into the `OptFormerDesigner`, which follows the same API as a OSS Vizier standard [`Designer`](https://oss-vizier.readthedocs.io/en/latest/guides/developer/writing_algorithms.html).

## Training the OptFormer (Coming Soon!)
**Work in Progress**

## Benchmark Results (Coming Soon!)
**Work in Progress**

# Citation
If you found this codebase useful, please consider citing our paper. Thanks!

```
@inproceedings{optformer,
  author    = {Yutian Chen and
               Xingyou Song and
               Chansoo Lee and
               Zi Wang and
               Qiuyi Zhang and
               David Dohan and
               Kazuya Kawakami and
               Greg Kochanski and
               Arnaud Doucet and
               Marc'Aurelio Ranzato and
               Sagi Perel and
               Nando de Freitas},
  title     = {Towards Learning Universal Hyperparameter Optimizers with Transformers},
  booktitle = {Neural Information Processing Systems (NeurIPS) 2022},
  year      = {2022}
}
```

**Disclaimer:** This is not an officially supported Google product.