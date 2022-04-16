# Sanitater
本存储库用于存放DL—Task-for-6 minist手写体识别有关代码

Mnist手写体识别
  1.Mnist数据库可以从这里下载，也可以在pytorch中torchvision的datasets.MNIST中直接访问。
  2.模型结构推荐大家用Lenet-5, Resnet18等小模型。注意图片的通道数目和分辨率是否和模型要求的相匹配。 
  3.了解分类任务常用的评价指标，Accuracy，precision,recall, F1 score,CMC等，根据最终目的选择合适的评价指标和模型的损失函数。
  4.撰写代码，了解深度学习代码的大概框架--数据loader,模型创建，优化器创建，损失函数创建，加载数据，模型前向推理并计算损失，后向传播更新模型，模型验证，日志存储等
  5.代码能够运行完后，分析loss和准确率的变化，调整模型超参数（学习率，学习率变化方式，batchsize等等）。
  这个阶段需要大家掌握：
  1.图像分类任务常用的评价指标
  2.卷积神经网络的基本构成
  3.深度学习代码的基本构成和撰写
  4.基本的调参数方式

知识点
一、卷积：
  卷积后尺寸=(输入-卷积核+加边像素数(padding))/步长(padding)+1
  eg:输入32 * 32，通过6个5 * 5 卷积核，步长为一，输出6 * 28 * 28((32-5=0)/1+1 = 28),训练参数为1*（5 * 5） * 6 +6=156
二、letnet网络结构与网络参数：
![image](https://github.com/Eason0921/Sanitater/blob/main/img_folder/letnet.jpg)
