# Training a (gated) RNN

1. Use an LSTM or GRU: _it makes your life so much simple!_
2. Initialize recurrent matrices to be orthogonal
3. Initialize other matrices with a sensible (__small!__) scale
4. Initialize forget gate bias to 1: _default to remembering_
5. Use adaptive learning rate algorithms: _Adam, AdaDelta, ..._
6. Clip the norm of the gradient: _1-5 seems to be a reasonable threshold when used together with Adam or AdaDelta._
7. Either only dropout vertically or look into using Bayesian Dropout (Gal and Gahramani - not natively in PyTorch)
8. _Be patient! Optimization takes time_
