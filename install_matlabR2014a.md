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

# Linux

* Unzip the downloaded file:

```
#!console
# unrar x /home/<username>/Downloads/R2014a_UNIX.rar /usr/local/matlab/
```

* If you have problems installing unrar:

```
#!console
# rpm -Uvh http://pkgs.repoforge.org/rpmforge-release/rpmforge-release-0.5.2-2.el6.rf.i686.rpm
# yum -y --enablerepo=rpmforge install unrar
```
* Change permissions on files before installing:

```
#!console
# cd /usr/local/matlab/
# chmod +x java/
# chmod +x install
# chmod a+x sys/java/jre/glnxa64/jre/bin/
```

* Install:
```
#!console
# ./install
```

> Choose Use a File Installation Key and click Next. 

> If you agree to the licensing terms, choose Yes and click Next.

> Choose I have the File Installation Key for my license and put in the Key from the Downloads area.

> Click Next.

> Keep the installation destination and click Next.

> Select the products to install and click Next.

> Choose the areas for program shortcuts and click Next.

> Review the installation summary and click Install.

> Additional installations may be required depending on the previous product selections. Follow the installation instructions.

> Make certain the check mark is in for Activate MATLAB and click Next.

> A new window will come up after a few moments. Choose Activate automatically using the Internet and click Next.

> Log on to your MathWorks Account or choose to create an account. The Activation Key from the downloads area will be needed to create an account.

> For the license, choose the TAH Designated Computer and click Next.

> Click Confirm to send the information to MathWorks.
 
> Activation is complete. Click Finish.

# Mac

# Windows