# Fault Detection System for Bearings in Electric Motors using Variational Auto Encoders

This repository contains the necessary files to replicate the work done for the IEEE Latin America Transactions submission with ID 9554. This README provides a description of the files, information regarding the submission, and author details.

## Manuscript information
**Title:** Fault Detection System for Bearings in Electric Motors using Variational Auto Encoders

**Submission ID:** 9554

### Authors
**A. Menéndez-González**
- **Affiliation:** University of Oviedo 
- **Email:** alonsomenendezgonzalez@gmail.com

**L. Magadán**
- **Affiliation:** University of Oviedo  
- **Email:** magadanluis@uniovi.es

**J. C. Granda**
- **Affiliation:** University of Oviedo   
- **Email:** jcgranda@uniovi.es

**F. J. Suárez**
- **Affiliation:** University of Oviedo   
- **Email:** fjsuarez@uniovi.es

### Abstract
Electric motors play a fundamental role in essential industries such as energy, transport, and aeronautics, which require efficient maintenance to ensure productivity. Bearings are the most common failure point, making Prognostics and Health Management of this component crucial for Industry 4.0. This paper introduces a Fault Detection System based on Variational Auto Encoders (VAEs) trained exclusively on healthy vibration data from two public datasets. By analyzing the resultant Gaussian distributions, the system identifies early indicators of faults. This approach overcomes the common challenge of requiring faulty data for training, while also making it applicable to any other dataset. The study reveals an initial degradation stage in the training datasets, a critical oversight in previous studies, providing a more accurate depiction of bearing degradation profiles.

## Repository Index
The files of the repository are organized as follows:

- **Code**
  - `VAE-IMS.ipynb`: Definition, training, and inference for the VAEs used for the IMS dataset. 
  - `VAE-XJTU.ipynb`: Definition, training, and inference for the VAEs used for the XJTU-SY dataset.
  - `HealthStageDivision.ipynb`: Notebook for analyzing the resultant distributions with 5 techniques.
- **CSVs**
  - This folder contains the means and variances obtained for each dataset, split into 7 files. They were inferred after the models' training in `VAE-IMS.ipynb` and `VAE-XJTU.ipynb`, and these CSVs are used in `HealthStageDivision.ipynb`

The trained models used in the manuscript can be provided upon request.
