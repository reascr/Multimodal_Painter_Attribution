### Multimodal Painter Attribution: Integrating Visual and Textual Features for Improved Classification Performance 

This repo contains code and data used for the final project in the class "Computational Cognitive Science II" for the MSc in IT and Cognition and the University of Copenhagen. 

#### data
This folder contains the data used for training the models. For this, a subsample of the SemArt data set was used (https://researchdata.aston.ac.uk/id/eprint/380/), including images and metadata (including descriptions pf the paintings, painter, title, timeframe, school, and type). Includes the unbalanced as well as the balanced data sets. 

#### data_preprocessing

- ##### Data_Pipeline.ipynb:
  Code to invesitgate, clean, and balance data set.
- ##### Get_ImageLIsts.ipynb:
  Code to obtain ImageLists needed for Detectron2.
- ##### Get_Visual_and_Joint_Features.ipynb:
  Code to obtain visual features by Detectron 2 to pass VisualBERT and to obtain joint visual-textual feature representations by extracting the last hidden layer of VisualBERT.

#### models 

- ##### 
