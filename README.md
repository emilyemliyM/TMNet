#  Contrastive Learning-based Place Descriptor Representation for Cross-modality Place Recognition

This repo contains the details for "Contrastive Learning-based Place Descriptor Representation for Cross-modality Place Recognition".

## 🔑 Set up 
Our experiment is tested on Ubuntu 20.04 with Python 3.8 with PyTorch 1.13.6.
- build environment
  ```
  conda create -n tmnet python=3.8
  conda activate tmnet
  pip install -r requirements.txt
  ```

## 📚 DataSet
We conduct the image-to-point-cloud place recognition based on KITTI dataset and KITTI-360 dataset.

- The KITTI DATASET
The used data for the experiment can be downloaded from [here](https://www.cvlibs.net/datasets/kitti/index.php).

Folder structure:

  ```
  data  
  ├── sequences  
  │   └── 00  
  │       ├── image_2  
  │       ├── Velodyne  
  │       └── poses.txt  
  └── ...
  ```

- The KITTI-360 DATASET
The used data can be downloaded from [here](https://www.cvlibs.net/datasets/kitti-360/index.php).

Folder structure:

  ```
  data  
  ├── data_2d_raw    
  │   ├── 2013_05_28_drive_0002_sync  
  │   │   ├── image_00  
  │   │   └── ...  
  │   └── ...  
  ├── data_3d_raw  
  │   ├── 2013_05_28_drive_0002_sync  
  │   │   ├── image_00  
  │   │   └── ...  
  │   └── ...  
  └── data_poses  
      ├── 2013_05_28_drive_0002_sync  
      │   ├── image_00  
      │   └── ...  
      └── ...
  ```

## 💡  Visualization
Our image-to-point-cloud place recognition on the unseen KITTI test sequence.

<div>
<img src="https://github.com/emilyemliyM/TMNet/blob/main/img/kitti08_demo2.gif" alt="描述文本" width="720" height="360">
</div>



