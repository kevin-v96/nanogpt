# nanogpt
A small GPT inspired by the tutorial from Andrej Karpathy

Trained on the tiny Shakespeare dataset. (but the architecture is data agnostic and can be used to train on other datasets given the resources and time)

The file gpt.py has a small language model that started out with only training on the previous token to output the next token (bigrams). That doesn't output very cohesive sentences, but it worked to elucidate the architecture that we're now using in the more sophisticated model.

Our current model has multiheaded self-attention as well as the other blocks outlined in the original transformer paper (Vaswani et.al., 2017).

Although pre-training a transformer at the level of GPT3.5 or GPT4 which they use as part of ChatGPT would take immense resources as well as a neural network with billions of parameters, the basic architecture that we use here is similar to what OpenAI uses. 

What makes ChatGPT so good is fine-tuning on top of this pretrained model as well as using RLHF (Reinforcement Learning with Human Feedback).