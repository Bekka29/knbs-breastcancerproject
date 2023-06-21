# knbs-breastcancerproject
A course project on machine learning using breast ultrasound images

# Segmentation of Breast Ultrasound Images using U-Net on Pytorch 
**Background**

Breast cancer is responsible for 1 in every 8 cncer diagnoses globally. it was the most prevalent cancer in women in 2020 and caused about 685,000 deaths in women. Projections show that by 2040, the incidence of breast cancer is expected to rise globally by over 40%, and mortality by 50%. WHO recently launched the Global Breast Cancer initiative to reduce its mortality by recommending regular population-based screening for those at risk, and seeking to improve timely diagnosis, treatment, and patient management.(1)

Breast imaging for cancer screening, diagnosis and evaluation, is an effective tool for prevention. However, the process is tedious and subject to error in interpretation when performed on a sizeable population.(2) Additionally, there are limited experts in the field of medical imaging.(3) The development of artificial  intelligence tools and techniques for the diagnosis, risk assessment, and prediction of patient response to therapy has been found to have great potential for automated screening and diagnosis. Using deep learning to perform some of these tasks would reduce the use of invasive techniques and also reduce errors from human interpretation of images.(2)

Image segmentation is a branch of digital image processing that assists in highlighting a region of interest. (3) UNet is an encoder-decoder deep neural network architecture for biomedical image segmentation. It was developed by Ronneberger et al. at the University of Freiburg, Germany in 2015.(4) The UNet arhitectures encodes, decodes and performs skip connections to transfer select features from an input image to generate a segmentation mask.
Previous sudies have used the Keras in Python and UNet to segment normal, benign and malignant classes of images(5) but in this work, PyTorch and U-Net will be used for the segmentation of a breast cancer ultrasound image dataset.

**Method**
1. Image Acquisition: The dataset of breast cancer ultrasound images and masks is downloaded from Kaggle. Data source: https://www.kaggle.com/datasets/aryashah2k/breast-ultrasound-images-dataset/download?datasetVersionNumber=1

2. Image preprocessing: The data classes, size and shape are explored and images are resized, visualized, and transformed to tensors.
Training,test and validation sets are created with data loaders.
3. Training of model: Feature extraction and segmentation using U-Net.
Plot accuracy and losses.
4. Testing of model

**REFERENCES**

1.Bhowmik A, Eskreis-Winkler S. Deep learning in breast imaging. BJR Open. 2022 May 13;4(1):20210060. doi: 10.1259/bjro.20210060. PMID: 36105427; PMCID: PMC9459862.

2.Arnold M, Morgan E, Rumgay H, Mafra A, Singh D, Laversanne M, Vignat J, Gralow J R, Cardoso F, Siesling S, Soerjomataram I, Current and future burden of breast cancer: Global statistics for 2020 and 2040, The Breast, Volume 66,2022, Pages 15-23,ISSN 0960-9776, https://doi.org/10.1016/j.breast.2022.08.010.
(https://www.sciencedirect.com/science/article/pii/S0960977622001448)

3.Malhotra P, Gupta S, Koundal D, Zaguia A, Enbeyle W. Deep Neural Networks for Medical Image Segmentation. J Healthc Eng. 2022 Mar 10;2022:9580991. doi: 10.1155/2022/9580991. PMID: 35310182; PMCID: PMC8930223.

4.Ronneberger, O., Fischer, P., Brox, T. (2015). U-Net: Convolutional Networks for Biomedical Image Segmentation. In: Navab, N., Hornegger, J., Wells, W., Frangi, A. (eds) Medical Image Computing and Computer-Assisted Intervention – MICCAI 2015. MICCAI 2015. Lecture Notes in Computer Science(), vol 9351. Springer, Cham. https://doi.org/10.1007/978-3-319-24574-4_28

5.https://www.kaggle.com/code/saidislombek/biomedical-image-segmentation-with-u-net/notebook

6. Al-Dhabyani W, Gomaa M, Khaled H, Fahmy A. Dataset of breast ultrasound images. Data in Brief. 2020 Feb;28:104863. DOI: 10.1016/j.dib.2019.104863.

