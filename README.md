# No One Idles: Efficient Heterogeneous Federated Learning with Parallel Edge and Server Computation
Official implementation for paper "No One Idles: Efficient Heterogeneous Federated Learning with Parallel Edge and Server Computation", ICML 2023

**TLDR:** We achieve parallel computing between the central server and the edge nodes in Federated Learning.

**If your project requires executing complex computational tasks on the central server, please use our solution! Our framework allows the aggregation process on the central server and the training process on edge devices to conduct in parallel, thereby improving training efficiency.**

## Environment setup

```Shell
conda create -n pfl python=3.8
conda activate pfl
pip install torch==2.3.1 torchvision==0.18.1 torchaudio==2.3.1 --index-url https://download.pytorch.org/whl/cu121
pip install numpy pandas matplotlib wandb tqdm pillow
pip install ipython jupyter notebook
```

## Citation
If you use this code, please cite our paper.
```@inproceedings{shysheya2022fit,
  title={No One Idles: Efficient Heterogeneous Federated Learning with Parallel Edge and Server Computation},
  author={Zhang, Feilong, and Liu, Xianming, and Lin, Shiyi and Wu, Gang and Zhou, Xiong and Jiang, junjun, and Ji, Xiangyang},
  booktitle={International Conference on Machine Learning},
  year={2022},
  organization={PMLR}
}
```
## Usage

Here is an example for PyTorch: 
```
python PFL.py --dataset cifar10 --node_num 10 --max_lost 3 --R 200 --E 5
```
