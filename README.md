# Ensemble-of-Deep-2D-and-3D-Fully-Convolutional-Neural-Network-for-Brain-Tumor-Segmentation

This repo utilize a ensemble of 2-D and 3-D fully convoultional neural network (CNN) for segmentation of the brain tumor and its constituents from multi modal Magnetic Resonance Images (MRI). The dense connectivity pattern used in the segmentation network enables effective reuse of features with lesser number of network parameters. On the BraTS validation data, the segmentation network achieved a whole tumor, tumor core and active tumor dice of 0.89, 0.76, 0.76 respectively.

# Pipeline
![pipeline](./pipeline.png)

# Results
![Results](./results.png)

### For training code please refer this [repo](https://github.com/koriavinash1/BraTs2018)


# Steps to follow:

+ Our Algo. uses masks to be generated before training/testing. We make use of antsbin for mask generation. Use helper_mask.py for mask generation.

+ This repo. provides ensemble of different models for segmentation. (a) ABLNet (modelABL.py, Air brain Lesion Network), (b) 3DBrainNet (model3DBNET.py, 3D multiresolution CNN), (c) Tiramisu2D (modelTis2D.py, 57 layered 2D CNN) and (d) Tiramisu 3D (modelTir3D.py, 57 layered 3D CNN)

+ More details about network architecture and training procedure can be found [here](https://link.springer.com/chapter/10.1007/978-3-030-11726-9_43)

# Citation

If you use some of our work, please cite our work:

```
@inproceedings{kori2018ensemble,
  title={Ensemble of Fully Convolutional Neural Network for Brain Tumor Segmentation from Magnetic Resonance Images},
  author={Kori, Avinash and Soni, Mehul and Pranjal, B and Khened, Mahendra and Alex, Varghese and Krishnamurthi, Ganapathy},
  booktitle={International MICCAI Brainlesion Workshop},
  pages={485--496},
  year={2018},
  organization={Springer}
}
``` 
## Contact 

* Avinash Kori (avinashgkori@smail.iitm.ac.in or koriavinash1@gmail.com)
