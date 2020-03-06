
Code Sources:

1. Baseline Classifiers: https://developers.google.com/machine-learning/guides/text-classification
   Followed the step by step process to create a classifier with Embedding, Dropout and Dense layer using Keras API

2. BERT Classifiers: https://github.com/ThilinaRajapakse/simpletransformers#minimal-start-for-multiclass-classification
   Used the starter code provided for using the BERT Classification wrapper

3. load_embeddings function picked up from NLP assignments

4. emoticons list for pre-processing: https://towardsdatascience.com/extracting-twitter-data-pre-processing-and-sentiment-analysis-using-python-3-0-7192bd8b47cf

5. embeddings downloaded from: https://worksheets.codalab.org/worksheets/0x84b71dd010cf4bff8d9f59cc22b49344

6. Resampling code referred from: https://elitedatascience.com/imbalanced-classes


Running the code:

1. Change the data directory to point to where the dataset is located.

2. Each of the sections in the IPython Notebook provided - 'Final NLP_Project.ipynb' are clearly marked.

3. If you want to start with the baseline classifiers:
Run all the cells before and including the one under section Model Training
4. This will load the data, perform pre-processing, up-sampling, convert the text to token sequence and start training the models one by one for each experiment.
	Once training is completed, classification report for the validation set will be generated alongwith a submission<Experiment>.csv file to submit to Kaggle.
	Also, the created model is saved in the output/<Model Name> directory.
5. Here on, the rest of the experiments can be run individually.
6. For training the BERT model Run the cells under Bert Loading and Training. The directories for caching and sacing models can be given as parameter to 
the MultiLabelClassification Model Wrapper.
7. For Binary Classification and Twitter Transfer Learning Experiment, run the code under section 7 and 8 respectively.	


Software Requirements:
Code implemented on Google Colab.
1. TensorFlow 2.x	
2. Python 3.6
3. Keras provided by Tensor Flow to be used
4. For SimpleTransformers BERT implementation, the commands are provided within the notebook but some are commented out. Please run them as required:
	i) install Anaconda and by extension conda
	ii) install pytorch cudatoolkit using codalab
	iii) install simpletransformers	