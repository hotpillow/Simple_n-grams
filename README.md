# Simple_n-grams
Note: The tokenizer used takes away ALL punctuation, but leaves the ends of connected words (i.e. 's, 'd, 'll, 've)

N-grams are described as a “language model to capture patterns in n consecutive words of training text.  An estimator smooths the probabilities derived from the text”. But I just like to say the models predict the probability of a word occurring based on the previous words.

Given a text file, the program splits the text into words (tokenize) then passes the words into NLTK's ngram() function along with the number of previous words - 1 the model should look back at (i.e. 3 is passed for a trigram and the model looks at the previous 2 words).

## How to run 
### Recommended that this is ran in a virtual environment.
  - create a virtual environmenet named .env
    - $ python3 -m venv .env
  - enter venv
    - $ source .env/bin/activate
  - install jupyter
    - Note: To install you may have edit the venv's pyvenv.cfg file in your IDE. Set 'include-system-site-packages' key to true to run the '--system-site-packages' option, otherwise you can leave it be.
    - $ pip install jupyter notebook
  - open the notebook
    - Note: When exiting a jupyter notebook tab (i.e. the code file was opened), click on file >> close and halt. The icon won't be green in the homepage after
    - $ python3 -m jupyter notebook
  - leave the venv
    - $ deactivate
### To start
- Install the '5 papers.txt' file or input your own file
- Open the jupyter notebook
- To run the entire code, click kernel then execute all
  - Or you can click the Run button to only run the highlighted cell
  - This program creates 5 sentences made of 10 words, edit cell 5 to change this
