# Optimizers
Regression Optimizer(Tensorflow)
TensorFlow offers seven optimizers:

1. **GradientDescentOptimizer**  
    This one is sensitive to the problem and you can face lots of problems using it, from getting stuck in saddle points to oscillating around the minimum and slow convergence. I found it useful for Word2Vec, CBOW and feed-forward architectures in general, but Momentum is also good.
2. **AdadeltaOptimizer**  
    Adadelta addresses the issues of using constant of linearly decaying learning rate. In case of recurrent networks it’s among the fastest.
3. **MomentumOptimizer**  
    If you learn a regression and find your loss function oscillating, switching from SGD to Momentum may be the right solution.
4. **AdamOptimizer** 
    Adaptive momentum in addition to the Adadelta features.
5. **FtrlOptimizer**  
    It’s better suited for online learning on large sparse datasets, like recommendation systems.
6. **RMSPropOptimizer**  
    This is a variant Adadelta that serves the same purpose - dynamic decay of a learning rate multiplier.
