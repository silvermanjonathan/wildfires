# wildfires 

Data Science Process:

Wildfires can have many causes, which are determined by expert investigators. Sometimes, the cause of a fire is obvious: an eyewitness account of arsonists leaving the scene of the crime. However it isn't always an open and shut case nor is it always arson. Other causes can be debris burning, equipment use, lightning, or a campfire gone awry. An investigation is always required. Can machine learning algorithms assist investigators of wildfires? This is the question I set out to explore.

In order to build a model, data is required; the more data the better. Mercifully, there’s a fairly clean dataset of over a million wildfires found on Kaggle. The dataset has many variables. However, not all given variables will be used in the model. Furthermore, part of the art of model building entails bringing in extra variables from different datasets.

A very reasonable feature to include in the modeling process is weather. Getting the weather for 1.88 million rows of data was the most challenging part of the project for a novice coder like myself. Trial and error on 1.88 million rows of data will take forever to compute. Fortunately, I thought of clever shortcuts which are detailed in the notebook.

Modeling is developed iteratively. In other words, a base model whose measures of veracity are overall improved with sequential modeling decisions, leading to new models. At the very least, the model should be better than chance. In a binary classification model, accuracy should be better than 50%. The base model here gives the right answer 61% of the time, and is a simple logistic model without exogenous features.

For evaluating our model simplistically, we can look at accuracy. The number of observations correctly classified over the total possible number of observations is accuracy. This is also called the True Positive rate. Further metrics to get a comprehensive picture of model performance are detailed in the notebook.

Table of Contents:

1 juyter notebook named "Modeling Pipeline".

Reproduction Instructions:

Download the dataset at https://www.kaggle.com/rtatman/188-million-us-wildfires

Future Steps:

Make a classifier for every cause of wildfire in the dataset. 
