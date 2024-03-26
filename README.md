# nanogpt
A small GPT inspired by the tutorial from Andrej Karpathy

Trained on the tiny Shakespeare dataset. (but the architecture is data agnostic and can be used to train on other datasets given the resources and time)

The file bigram.py has a small bigram language model that only trains on the previous token to output the next token(bigrams). Doesn't output very cohesive sentences, but it works to elucidate the architecture that we're using in the more sophisticated model.
