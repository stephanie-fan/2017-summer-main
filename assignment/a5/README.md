# Assignment 5: Part of Speech and Parsing

## Due: Wednesday, August 9nd, 11:59p Pacific

This assignment consists of two parts:

* [Part of Speech](part1/Part-of-Speech.ipynb)
* [Parsing](part2/CKY.ipynb)

### Visualizations (optional)

We've built interactive visualizations of both parts of this assignment, which we hope you'll find useful as you work through your implementations of Viterbi, Forward-Backward, and CKY. In particular, you can inspect partial hypotheses (tag sequences or subtrees), and see how the backpointers trace through the Viterbi table (i.e. δ or the chart):

* [HMM (part1)](https://hmm-dot-nlp-visualizations.appspot.com/hmm?sentence=James+ate+the+food&vizMode=viterbi&numFormat=log)
* [CKY (part2)](https://cky-dot-nlp-visualizations.appspot.com/cky?sentence=James+ate+the+food)

_Note: the tag set and grammar in these demos is simplified to reduce visual clutter, so don't be surprised if numbers don't match with your implementation!_

### The Penn Treebank (optional)

NLTK includes the `treebank` corpus, which is an abbreviated sample (3900 sentences) of the full (73k sentence) corpus.

The full corpus is available through Berkeley for research and academic purposes. We've included a copy in `ptb.zip` in this directory, along with a script that will install it to the proper directory for NLTK to access. Run as:
```
./install_ptb.sh
```
If it installs successfully, you can substitute `nltk.corpus.ptb` for `nltk.corpus.treebank`, and most functions should work normally - but with access to much more data. See [NLTK - Parsed Corpora](http://www.nltk.org/howto/corpus.html#parsed-corpora) for more information.

## Submission instructions

As always, you should commit your changes often with `git add` and `git commit`. As this is a new assignment, there may be bugfixes and corrections - so keep your eye on Piazza and GitHub for any updates.

Please submit by running the submit script:
```
./assignment/submit.sh -u your-github-username -a 5
```
You can view your work in your usual submission repo on the `a5-submit` branch.
