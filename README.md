# Design of synthetic promoters for cyanobacteria with generative deep-learning model
In our study, 'Design of synthetic promoters for cyanobacteria with generative deep-learning model', we provide a deep-learning based generic framework to generate synthetic promoter sequences for cyanobacteria and predict their strength using a variational autoencoder (VAE) and convolutional neural network (CNN), respectively. We confirmed that the generated sequences showed a very low similarity with the cyanobacteria native promoters, and validated their promoter activity to drive a gene expression using a cell-free transcription assay. Here, we present the code used in this study for promoter data mining, VAE model, CNN model, and data refinement. The codes can be downloaded from each Jupyter notebook file (.ipynb). 

![Figure 1](https://user-images.githubusercontent.com/97028331/168530899-fbe16990-76a7-44d8-a5d5-317660996a67.png)

## Prerequisites
- Python, NumPy, TensorFlow, SciPy, Matplotlib, Keras
- NVIDIA GPU
- TensorFlow = 2.0.0
- Cuda = 10.0
- Python = 3.6.0

## Citation
Seo, E.†, Choi, Y.-N.†, Shin, Y., Kim, D., and Lee, J.W.\* “Design of synthetic promoters for cyanobacteria with generative deep-learning model”, (in revision). († co-first)

## Reference
1. Kingma D, Welling M. Auto-encoding variational bayes 2013 arXiv preprint arXiv:1312.6114.
2. Kopf M, Klähn S, Scholz I, Matthiessen JKF, Hess WR, Voß B. Comparative analysis of the primary transcriptome of Synechocystis sp. PCC 6803. DNA Res. 2014 Oct;21(5):527–539. 
3. Wang Y, Wang H, Wei L, Li S, Liu L, Wang X. Synthetic promoter design in Escherichia coli based on a deep generative network. Nucleic Acids Res. 2020 Jul 9;48(12):6403–6412. 
4. Choi, Y.-N., Shin, Y., Park, J.M.\*, and Lee, J.W.\* “Cell-free transcription-coupled CRISPR/Cas12a assay for prototyping cyanobacterial promoters”, ACS Synth. Biol., 10(6): 1300-1307 (2021). (* co-corresponding)
