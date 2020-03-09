# Chinese-ChatBot
## 环境
`Keras<br>python3.68<br>windows10<br>jupyter`<br>

  青云语料库10万组对话，在google colaboratory训练。实验表明加入attention机制后训练速度快，收敛快，效果更好。

## 界面用Tkinter
![](https://github.com/jiayiwang5/Chinese-ChatBot/blob/master/image/image.png)

## Attention权重可视化
![](https://github.com/jiayiwang5/Chinese-ChatBot/blob/master/image/image2.png)

## 其他
* 训练文件chat_bot_v2中，最后三块代码前两个是挂载谷歌云盘用的，最后一个是获取那些loss方便画图，不知道为什么回调函数里的tensorbord不好使，故出此下策；<br>
* 预测文件里倒数第二块代码只有文字输入没界面，最后一块代码是界面，根据需求两块跑其一即刻；<br>
* models里面的几个权重我可能传错了，如果你训练的时候因为加载权重报错了，把现有的权重都删掉，重新训练即刻。<br>
