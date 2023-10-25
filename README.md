# Difficult Word Decison Tree Model

A decision tree machine learning model to identify difficult words for those who are hard of hearing. Built with Python, scikit-learn, and the Difficult Words for Hearing Impaired Children data set:
https://www.kaggle.com/datasets/nusteme/difficult-words-for-hearing-impaired-children

This model was created as part of a larger project to develop a lexical automatic text simplifying browser extension for children who are hard of hearing. The project is currently in production.
## Methods
This model uses a decision tree classifier to identify the difficulty of a word based on it's associated features, how long it is, how many vowels it has, etc.   

First the initital model is created, trained on the data, and has it's accuracy gauged using both an absolute percentage of correct guesses and also a confusion matrix which shows it's accuracy on false guesses and postive guesses. The tree itself is also visually displayed.

This tree is then further refined using a random sampling method. Varying hyperparameter values are tested across 100 different random variations. The best model of this 100 is then tested again, creating a tuned model.

Lastly the features are displayed in order of importance as deemed by the final decision tree model.
