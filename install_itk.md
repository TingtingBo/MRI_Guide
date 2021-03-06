How to Process MRI Images:

1. [Beginner's Guide to Command-Line Interface](begin_primer)
2. Installation Instructions
    * [Programs](Home)
    * [Fulton Supercomputing Lab specific instructions](fsl)
3. Preprocessing T1 images
     * [Download example files](https://bitbucket.org/njhunsaker/preprocessing-t1-example)
     * [Convert DICOM to NIfTI](preprocessing_dcm2nii)
     * [Align anterior commissure and posterior commisure](preprocessing_acpcdetect)
     * [Correct intensity nonuniformities (bias field)](preprocessing_N4BiasFieldCorrection)
     * [Resample images to isotropic voxel size 1](preprocessing_resample)
     * [Brain Extraction and Tissue Segmentation](preprocessing_antscorticalthickness)
4. Hippocampus Segmentation
     * [Placing Landmarks](hpc_landmarks)

---------------------------------------

* [Firefox](install_firefox)
* [DICOM Toolkit](install_dcmtk)
* [dcm2nii DICOM to NIfTI conversion](install_dcm2nii)
* [Multi-image Analysis GUI (MANGO)](install_mango)
* [MATLAB R2014a](install_matlabR2014a)
* [ACPC Detect](install_acpcdetect)
* [Git](install_git)
* [CMake](install_cmake)
* [C++ Compiler](install_gcc)
* [Advanced Normalization Tools](install_ants)
* [ITK](install_itk)
* [Convert3D](install_convert3d)

---------------------------------------

A PDF of the ITK manual can be found here: [http://www.itk.org/ItkSoftwareGuide.pdf](http://www.itk.org/ItkSoftwareGuide.pdf)

# Linux

* Download the latest version of ITK:

```
#!console
# cd /usr/local/
# git clone git://itk.org/ITK.git
```

* Install ITK:

```
#!console
# mkdir ITK-build
# cd ITK-build
# ccmake ../ITK
```

* Configure ITK by pressing the "c" key. In order to speed up the build process, disable the compilation of the unit tests and examples. This is done with the variables `BUILD TESTING=OFF` and `BUILD EXAMPLES=OFF`. Each time you change a set of variables in CMake, it is necessary to proceed to another configuration step by hitting the "c" key.

* When no new options appear in CMake, you can proceed to generate Makefiles by hitting the "g" key.

```
#!console
# make
```

# Mac

* Download the latest version of ITK:

```
#!console
# cd /usr/local/
# git clone git://itk.org/ITK.git
```

* Install ITK:

```
#!console
# mkdir ITK-build
# cd ITK-build
# ccmake ../ITK
```

* Configure ITK by pressing the "c" key. In order to speed up the build process, disable the compilation of the unit tests and examples. This is done with the variables `BUILD TESTING=OFF` and `BUILD EXAMPLES=OFF`. Each time you change a set of variables in CMake, it is necessary to proceed to another configuration step by hitting the "c" key.

* When no new options appear in CMake, you can proceed to generate Makefiles by hitting the "g" key.

```
#!console
# make
```


# Windows