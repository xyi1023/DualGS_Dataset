# DualGS_Dataset
The dataset of the paper "DualGS: Robust Dual Gaussian Splatting for Immersive Human-centric Volumetric Videos".

## DualGS: Robust Dual Gaussian Splatting for Immersive Human-centric Volumetric Videos

**[Yuheng Jiang](https://nowheretrix.github.io/), [Zhehao Shen](https://github.com/moqiyinlun), [Yu Hong](https://github.com/xyi1023), [Chengcheng Guo](https://github.com/gcccccccccccc12345), [Yize Wu](https://github.com/wuyize25), [Yingliang Zhang](https://cn.linkedin.com/in/yingliangzhang),  [Jingyi Yu](http://www.yu-jingyi.com/), [Lan Xu](http://xu-lan.com/).** 

*ACM SIGGRAPH ASIA 2024*

[[Project Page]](https://nowheretrix.github.io/DualGS/) [[Paper Link]](https://export.arxiv.org/abs/2409.08353) [[Dataset Link]](https://cvrmkura-my.sharepoint.com/:f:/g/personal/sdjnes_cvrmkura_onmicrosoft_com/Et4niDRbacBHgKgBOlSDxZEB3VBp24gkh9DEpxaiAbk3sg?e=8B9lzi)

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
The dataset is publicly accessible at [Link](https://cvrmkura-my.sharepoint.com/:f:/g/personal/sdjnes_cvrmkura_onmicrosoft_com/Et4niDRbacBHgKgBOlSDxZEB3VBp24gkh9DEpxaiAbk3sg?e=8B9lzi). It is authorized for non-commercial use only. For commercial use, please contact Yuheng Jiang (jiangyh2@shanghaitech.edu.cn) and cc Lan Xu(xulan1@shanghaitech.edu.cn) to obtain necessary permissions.

### Citation

If you use this dataset for your research, please cite our paper:

```
@article{jiang2024robust,
  title={Robust Dual Gaussian Splatting for Immersive Human-centric Volumetric Videos},
  author={Jiang, Yuheng and Shen, Zhehao and Hong, Yu and Guo, Chengcheng and Wu, Yize and Zhang, Yingliang and Yu, Jingyi and Xu, Lan},
  journal={arXiv preprint arXiv:2409.08353},
  year={2024}
}
```



