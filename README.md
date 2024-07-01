# Anaconda

[Archive](https://repo.anaconda.com/archive)

```bash
wget https://repo.anaconda.com/archive/Anaconda3-2024.06-1-Linux-x86_64.sh
chmod +x Anaconda3-2024.06-1-Linux-x86_64.sh
sh Anaconda3-2024.06-1-Linux-x86_64.sh
```

```bash
export PATH=~/anaconda3/bin:~/anaconda3/condabin:$PATH
```

```bash
conda config --set auto_activate_base false
```

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
