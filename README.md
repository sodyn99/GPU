# GPU

## Tensorflow

[Docs](https://www.tensorflow.org/install/source?hl=ko&_gl=1*1cor0de*_up*MQ..*_ga*MTEzNTY5MzExMi4xNzE5ODMyOTcw*_ga_W0YLR4190T*MTcxOTgzMjk3MC4xLjAuMTcxOTgzMjk3MC4wLjAuMA..#gpu)

```bash
pip install tensorflow[and-cuda]
```

```python
import tensorflow as tf
print(tf.config.list_physical_devices('GPU'))
```

## Pytorch

[Start Locally](https://pytorch.org/get-started/locally/)

```bash
conda install pytorch torchvision torchaudio pytorch-cuda=12.1 -c pytorch -c nvidia
```

```python
import torch
torch.cuda.is_available()
```
