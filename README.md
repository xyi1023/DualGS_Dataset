# DualGS_Dataset
The dataset of the paper "DualGS: Robust Dual Gaussian Splatting for Immersive Human-centric Volumetric Videos".

## DualGS: Robust Dual Gaussian Splatting for Immersive Human-centric Volumetric Videos

**[Yuheng Jiang](https://nowheretrix.github.io/), [Zhehao Shen](https://github.com/moqiyinlun), [Yu Hong](https://github.com/xyi1023), [Chengcheng Guo](https://github.com/gcccccccccccc12345), [Yize Wu](https://github.com/wuyize25), [Yingliang Zhang](https://cn.linkedin.com/in/yingliangzhang),  [Jingyi Yu](http://www.yu-jingyi.com/), [Lan Xu](http://xu-lan.com/).** 

*ACM SIGGRAPH ASIA 2024*

[[Project Page]](https://nowheretrix.github.io/DualGS/) [[Paper Link]](https://export.arxiv.org/abs/2409.08353)

![dataset_description](./imgs/gallery.png)

### Description

We have currently uploaded 7 sample cases of data including a diverse range of musical instruments from both Western and Eastern traditions. Meanwhile, 3 single-frame data have been uploaded as examples, which you can access without signing the license agreement.

To run algorithms on single-frame data, you need to move the calibration files. For `image_white` under instant-ngp format, rename the frame folder to `images` and move `transforms.json` to the same directory as `images`. For `image_white_undistortion` in colmap format, rename the frame folder to `images` and move the `sparse/0` folder to the same directory as `images`.

The overall file structure is as follows:
```
├── image_white
│    ├── %d                - The frame number, starts from 0.
│    │   └──%d.png         - Masked RGB images for each view. view number starts from 0.
│    └── transforms.json   - Camera extrinsics and intrinsics in NGP format.
│
├── image_white_undistortion
│    ├── %d                - The frame number, starts from 0.
│    │   └──%d.png         - Undistorted maksed RGB images for each view. view number starts from 0.
│    └── colmap/sparse/0   - Camera extrinsics and intrinsics in Gaussian Splatting format.
```
### Download our dataset

The dataset is available on Onedrive and requires permission to access it. Please carefully read, fill in the [license form](./license.pdf), and send it to Yuheng Jiang (jiangyh2@shanghaitech.edu.cn) and cc Lan Xu(xulan1@shanghaitech.edu.cn) to request access.

By requesting access to the content, you acknowledge that you have read this agreement, understand it, and agree to be bound by its terms and conditions. This agreement constitutes a legal and binding agreement between you and the provider of the protected system or content. The Virtual Reality and Visual Computing Center is the only owner of all intellectual property rights, including copyright, of DualGS Dataset, and VRVC reserves the right to terminate your access to the dataset at any time.

Notes:

Once the license agreement is signed, we will give access to the data.

### Citation

If you use this dataset for your research, please cite our paper:

```
@misc{jiang2024robust,
    title={Robust Dual Gaussian Splatting for Immersive Human-centric Volumetric Videos},
    author={Yuheng Jiang and Zhehao Shen and Yu Hong and Chengcheng Guo and Yize Wu and Yingliang Zhang and Jingyi Yu and Lan Xu},
    year={2024},
    eprint={2409.08353},
    archivePrefix={arXiv},
    primaryClass={cs.GR}
}
```



