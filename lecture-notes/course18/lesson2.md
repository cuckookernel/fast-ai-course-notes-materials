# CNNs

## About the learning rate

If the loss is increasing from iteration to iteration, then the learning rate is almost certainly too high. 

The question is, what's the best value of the learning rate. 

Even so called dynamic LR  methods such as Adam use a base lr parameter that needs to be set. 

## Data augmentation

One of the _most important_ techniques that you can do to make a better model.
To do data augmentation, add `aug_tfms` to call to `tfms_from_model`. For example `transforms_side_on`.

Then pass obtained transforms to function `ImageClassifierData.from_paths`.


### SGDR 

**TRICK**: A fairly recent discovery.  

Learning rate annealing, decrease the learning rate as one gets closer to local optimum.
Cosine annealing. The learning rate schedule decreses slowly at first and then more rapidly.

Restarting the learning rate periodically helps to get out of local minima that are two narrow and unstable 
in favor of flatter parts of the objective function surface that could give more stable performance upon variations
of the data distribution.

The parameter `cycle_len` passed to `learn.fit` controls the number of epochs we go through between restarts of the learning rate schedule. 











