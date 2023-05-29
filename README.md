# Translate-German-to-English
For the thask of Name-Entity recognition i used pre-trained T5-Base model.
The data for training contains German sentence and English sentence.
The test data without labels was German sentence with hints from the translated english sentence, such as roots and modifiers in the sentence.
So for training the data to be accurate on the test data, i used a depedancy parsing model from spacy('en_core_web_sm') to extract the roots and modifiers from the training data.
After this, i create training data with German sentence and hints and English sentence as label.
On this dataset i trained the T5-Base.
The evaluation function was BLEU that stands for translate tasks. 
