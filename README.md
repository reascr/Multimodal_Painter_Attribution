### Multimodal Painter Attribution: Integrating Visual and Textual Features for Improved Classification Performance 

This repo contains code and data used for the final project in the class "Computational Cognitive Science II" for the MSc in IT and Cognition at the University of Copenhagen. 

#### data
This folder contains the data used for training the models. For this, a subsample of the SemArt data set was used (https://researchdata.aston.ac.uk/id/eprint/380/), including images and metadata (descriptions of the paintings, painter, title, timeframe, school, and type). Contains the original data subsample as well as the cleaned and balanced data sets used for training.

#### data_preprocessing

- ##### Data_Pipeline.ipynb:
  Code to invesitgate, clean, and balance the data set.
- ##### Get_ImageLIsts.ipynb:
  Code to obtain ImageLists required by Detectron2.
- ##### Get_Visual_and_Joint_Features.ipynb:
  Code to obtain visual features by Detectron 2 to pass to VisualBERT and to obtain joint visual-textual feature representations by extracting the last hidden layer of VisualBERT.

#### models 

- ##### bert-classifier.ipynb
  Code to train and evaluate a BERT classifier on the whole balanced data set.
- ##### joint-embeddings-classifier-1500.ipynb
  Code to train and evaluate a MLP using joint embeddings on 1500 data points.
- #### visual-features-classifiert.ipynb
  Code to train and evaluate a MLP using visual embeddings on the whole balanced data set.


#### wilcoxon_signed_rank_test
This folder contains a .csv file with accuracy scores obtained after training all models on 10 different random seeds and a notebook to perform statistical significance testing between the multimodal model and the baselines (only visual and only textual features).
