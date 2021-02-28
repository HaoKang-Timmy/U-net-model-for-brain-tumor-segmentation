# A-U-net-model-used-for-brain-tumor-segmentation
This is what I learned from my summer session. The project is based on U-net. It is a model based on CNN model, and uses some fancy technique such as extended path. I use U-net model as well as other techniques. I will introduce them to you.
## Technique I uesd
### Data augmentation
One of the most improtant thing I used is data augmentation. And this is really useful.
I have read the paper about U-net(https://link.springer.com/chapter/10.1007/978-3-319-24574-4_28). They said that elastic scaling is a good way. So I tried it. I also tried rotation.
### Learning rate decay
If we use const learning rate decay, it is not a good way.
![learning rate decay](https://img2018.cnblogs.com/blog/1351564/201906/1351564-20190628111619212-48470440.png "learning rate")

So I used expotentional decrease for my model.
It is helpful for train speed and results.
### Optimiser I used
For U-net, there are many optimisers. Optimiser is used to define gradient descent of our model. So it is really important. I tried 'Adam' and 'SGD'. I found 'Adam' is better.
