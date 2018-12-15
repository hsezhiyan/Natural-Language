# Language Models

Using the language models to be discussed, I developed a basic autocorrect system.

SpellCorrect.py uses all other files/functions to perform autocorrect, and then performs evaluations. Run this file with the following code:

`python SpellCorrect.py`

The file EditModel.py provides the mechanism to edit words based on 4 inputs: insert a character, transpose two characters, replace a character,
and delete a character.

The SmoothUnigram.py and SmoothBigram.py files implement Unigram and Bigram models, respectively. In addition, they use Laplace-1 smoothing
to get better results.

The BackoffModel.py implements stupid backoff, which is a linear combination of smoothed bigram and unsmoothed unigram.

`python BackoffModel.py`

The CustomModel.py implements trigram with stupid backoff, using smoothed trigram and unsmoothed bigram and unigram.

`python CustomModel.py`

