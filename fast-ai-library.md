When calling `learner.fit()` 

The output numbers in each row are:  *epoch-number*, *training loss*, *validation loss*, *accuracy*.

`learn.lr_find()`: runs training with an increasing learning rate schedule to see find an optimal value of learning rate

`learn.sched.plot_lr()` shows the learning rate used for each iteration of `lr_find()`? 

`learn.sched.plot()` Plot of learning rate against loss.  The best learning rate is not the minimum, because at that point it is no longer improving. 
Best learning rate is probably one order of magnitude lower, where it is clear still decreasing. 

`learn.save`  save weights onto a file. `learn.load` load weight back to restore network.




