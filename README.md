# Overview of this research

In this research, we generated synthetic promoter sequence of cyanobactera(*Synechocystis* sp.PCC6803) and predicted their promoter strength. We generated 
newly synthetized promoter seqeunce via variational autoencoder(VAE), which is one of the popular deep-generative model. After synthetic promoter generation, we predicted their gene expression level through convolutional neural network. Using these deep-learning model, we can generate the synthetic promoter that has the valid features of the native promoter and predict their promoter strength without time-consuming experiments. More specific information about our research can be available at [paper link].

# Promoter data mining

We uploaded code for promoter data mining. We used whole-genome sequence and differential-RNA sequencing results from Kopf et al., which are available at [link]. Through this code, user can be obtain the promoters whose lengths are 100 base pairs and their strengts.  

# VAE model traninig and evaulation

We uploaded code for tranining VAE model. We used promoter sequence of **Promoter data mining.ipynb** for training dataset. For evaluation of the VAE model results, we also uploaded the code for 6-mer(TATAAT, TAAAAT, TAGAAT, AAAATA) frequency.

# CNN model training

We uploaded code for tranining CNN model. 5-Fold cross validation was used in the model training to avoid overfitting which can occur in small dataset. 

# Data refinement and new CNN model training

We uploaded the code for data refinment, which is the process selecting the **NANNNT-containing**, **NANANT-containing**, **TANNNT-containing** and **TANANT-containing promoters** from natural promoter dataset. We also uploaded code for training the 4 CNN models that are trained in each refined dataset.
