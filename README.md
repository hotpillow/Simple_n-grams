# Simple n-grams
Note: The tokenizer used takes away ALL punctuation, but leaves the ends of connected words (i.e. 's, 'd, 'll, 've)

N-grams are essentially models that predict the probability of a word occurring based on the previous n - 1 words.

This program tokenizes the text file (splits the text into words) then passes the tokens into NLTK's ngram() function along with the number of previous words - 1 the model should look back at (i.e. 3 is passed for a trigram and the model looks at the previous 2 words). Then five sentences, each ten words, are generated using the n-grams.

## How to run 
### Setup
Recommended that this is ran in a virtual environment.
  - Create a virtual environmenet named .env
    - $ python3 -m venv .env
  - Enter the virtual environment
    - $ source .env/bin/activate
  - Install jupyter
    - Note: To install you may have edit the venv's pyvenv.cfg file in your IDE. Set 'include-system-site-packages' key to true to run the '--system-site-packages' option, otherwise you can leave it be.
    - $ pip install jupyter notebook
  - Additional packages to install: nltk, matplotlib, and numpy
  - Open the notebook
    - Note: When exiting a jupyter notebook tab (i.e. the code file was opened), click on file >> close and halt. The icon won't be green in the homepage after
    - $ python3 -m jupyter notebook
  - Leave the venv
    - $ deactivate

### To start
- Install the '5 papers.txt' file or input your own file
- Open the jupyter notebook
- To run the entire code, click kernel then execute all
  - Or you can click the Run button to only run the highlighted cell
  
