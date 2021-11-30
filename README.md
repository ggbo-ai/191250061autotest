# 191250061autotest

#### 操作视频链接：https://box.nju.edu.cn/f/69e436503fb04e2ea6e6/

starGAN：

依赖

```
conda create -n stargan-v2 python=3.6.7
conda activate stargan-v2
conda install -y pytorch=1.4.0 torchvision=0.5.0 cudatoolkit=10.0 -c pytorch
conda install x264=='1!152.20180717' ffmpeg=4.0.2 -c conda-forge
pip install opencv-python==4.1.2.30 ffmpeg-python==0.2.0 scikit-image==0.16.2
pip install pillow==7.0.0 scipy==1.2.1 tqdm==4.43.0 munch==2.5.0
```



测试的数据集（人脸图像）：

https://www.dropbox.com/s/96fmei6c93o8b8t/100000_nets_ema.ckpt?dl=0

https://www.dropbox.com/s/tjxpypwpt38926e/wing.ckpt?dl=0

运行指令：

python main.py --mode sample --num_domains 2 --resume_iter 100000 --w_hpf 1 \
               --checkpoint_dir expr/checkpoints/celeba_hq \
               --result_dir expr/results/celeba_hq \
               --src_dir assets/representative/celeba_hq/src \
               --ref_dir assets/representative/celeba_hq/ref



MDNet:

依赖：

- python 3.6+
- opencv 3.0+
- [PyTorch 1.0+](http://pytorch.org/) and its dependencies
- for GPU support: a GPU with ~3G memory



运行指令：

```
python tracking/run_tracker.py -s DragonBaby [-d (display fig)] [-f (save fig)]
```

结果存储在results里





#### 