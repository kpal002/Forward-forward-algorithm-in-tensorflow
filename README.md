# Forward-forward-algorithm-in-tensorflow

Paper: [Geoffrey Hinton. The Forward-Forward Algorithm: Some Preliminary Investigations](https://www.cs.toronto.edu/~hinton/FFA13.pdf)
Implemented examples of supervised-wise forward forward (FF) algorithm (paper section 3.2)


In FFA - the input is passed twice through the network in a forward-fashion, while no backward pass happens. Instead of a loss function, a "goodness" function is used to evaluate the predictions of the network. One of the forward passes is a "positive" pass, while the other is the "negative" pass.

- The positive pass aims to maximize the goodness on real data (actual input features and labels)
- The negative pass aims to minimize the goodness on fake data (corrupt input features and wrong labels)
