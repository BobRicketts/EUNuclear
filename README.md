# About this project
This repository contains the code for the joint exam in Digital Methods and Advanced Social Data Science II. <br>
Motivated by the recent inclusion of nuclear energy into the EU taxonomy for sustainable activities, and by the Russian invasion of Ukraine, this project examines the debate around nuclear energy at the EU level.

## Directories
| **Directory** | **Description** |
| :------------ | :-------------- |
| _Data_                                  | Contains data and files used across the project |
| _Twitter data collection_               | Scripts for Twitter data collection |
| _Constructing final dataset_            | Scripts for turning raw Twitter data into subsetted tabular dataset |
| _Retweet network and actor locations_   | Scripts for constructing retweet network and examining user locations |
| _Content analysis_                      | Scripts for dictionary classification of tweets and validation of dictionary |
| _Topic models_                          | Scripts for fitting and analyzing Top2Vec and hSBM topic models|
 
## Note on unfiltered data
We decided not to include the unfiltered data (containing all the data collected in the actor-based snowballing) in this GitHub repository. The two scripts in _Constructing final dataset_ for selecting and categorizing relevant actors serve as documentation, but do not run.

## Notes on topic models
The code used for implementing Top2Vec was forked from [Dimo Angelov's Top2Vec implementation](https://github.com/ddangelov/Top2Vec) while the code for the hSBM topic model was forked from [Gerlach, Peixoto, and Altmann's hSBM implementation](https://github.com/martingerlach/hSBM_Topicmodel). Slight modifications were made to the source code to allow for the modification of model parameters. <br> 
We recommend installing version 2.45 of the `graph_tool` package since dependency issues may be experienced with older versions. <br>
The Top2Vec model reported in the exam paper was too large to upload to GitHub, but can be accessed by following [this Dropbox link](https://www.dropbox.com/s/81z9j1vem89h0nb/top2vec_model.txt?dl=0). The file should be placed in the _Topic models/Models & outputs_ folder. Alternatively, a new Top2Vec model can be fitted.
