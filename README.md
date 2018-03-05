# cs224n-win18-squad
Code for the Default Final Project (SQuAD) for [CS224n](http://web.stanford.edu/class/cs224n/), Winter 2018

Note: this code is adapted in part from the [Neural Language Correction](https://github.com/stanfordmlgroup/nlc/) code by the Stanford Machine Learning Group.

## Model name and explanations.

`qa_model.py`: the baseline model.

`edsa_model.py`: shortened from end-dep-start-add model. It borrows the idea from handout section 5.3. After making the prediction of the start position. Create a start attention vector using the sum of blended position representation weighted by the probability distribution of that position being the start position. Then it adds that attention vector to the blended vector for every postion to make the end prediction.

`edsc_model.py`: shortened from end-dep-start-concat model. Similar to `edsa_model.py`, except it concatenates the attention vector to the blended vector.
