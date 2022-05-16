# Design of synthetic promoters for cyanobacteria with generative deep-learning model
In this research, we generated synthetic promoter sequence of cyanobactera(*Synechocystis* sp.PCC6803) and predicted their promoter strength. We generated newly synthetized promoter seqeunce via **variational autoencoder(VAE)** model, which is one of the popular deep-generative model. After synthetic promoter generation, we predicted their gene expression level through **convolutional neural network(CNN)** model. The predicted results were validated by **cell-free transcription(CF-TX) analysis**. Using these deep-learning models and CF-TX analysis, we can generate the synthetic promoters which have the valid features of the native promoters and predict their promoter strength. By using CF-TX ananlysis, we also evaluate the deep learning results without time-consuming experiments.

![Figure 1](https://user-images.githubusercontent.com/97028331/168530899-fbe16990-76a7-44d8-a5d5-317660996a67.png)

### Promoter data mining
We uploaded jupyter notebook file(Promoter data mining.ipynb) for promoter data mining. We used whole-genome sequence and differential-RNA sequencing results from Kopf et al., which are available at [http://www.cyanolab.de/Supplementary.html]. Through this code, user can obtain the promoter sequences(100 base pairs) and their strength.  

### VAE model training and evaulation
We uploaded jupyter notebook file(VAE training.ipynb) for training VAE model. We used result of **Promoter data mining.ipynb** as training dataset. For evaluation of the VAE model results, we also uploaded the code(VAE validation.ipynb) for 6-mer(TATAAT, TAAAAT, TAGAAT, AAAATA) frequency analysis.

### CNN model training
We uploaded jupyter notebooke file(CNN training.ipynb) for tranining CNN model. 5-Fold cross validation was used in the model training to avoid overfitting which can occur in small dataset. 

### Data refinement and new CNN model training
We uploaded jupyter notebook file(Data refinement and new CNN model training.ipynb) for data refinement and new CNN model training, which is the process selecting the **NANNNT-containing**, **NANANT-containing**, **TANNNT-containing** and **TANANT-containing promoters** from native promoter dataset. We also uploaded code for training the 4 CNN models that are trained in each refined dataset.

## Prerequisites
- Python, NumPy, TensorFlow, SciPy, Matplotlib, Keras
- NVIDIA GPU
- TensorFlow == 2.0.0
- Cuda == 10.0
- Python == 3.6.0

## Citation
Seo, E.†, Choi, Y.-N.†, Shin, Y., Kim, D., and Lee, J.W.* “Design of synthetic promoters for cyanobacteria with generative deep-learning model”, (in revision). († co-first)

## Reference
1. Kingma D, Welling M. Auto-encoding variational bayes 2013 arXiv preprint arXiv:1312.6114.
2. Kopf M, Klähn S, Scholz I, Matthiessen JKF, Hess WR, Voß B. Comparative analysis of the primary transcriptome of Synechocystis sp. PCC 6803. DNA Res. 2014 Oct;21(5):527–539. 
3. Wang Y, Wang H, Wei L, Li S, Liu L, Wang X. Synthetic promoter design in Escherichia coli based on a deep generative network. Nucleic Acids Res. 2020 Jul 9;48(12):6403–6412. 
