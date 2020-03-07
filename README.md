# Chinese-ChatBot

Keras, python3.68, windows10, jupyter;
LSTM, seq2seq, attention.

  青云语料库10万组对话，在google colaboratory训练。实验表明加入attention机制后训练速度快，收敛快，效果更好。

界面用Tkinter
![](https://github.com/jiayiwang5/Chinese-ChatBot/blob/master/image/image.png)

Attention权重可视化
![](https://github.com/jiayiwang5/Chinese-ChatBot/blob/master/image/image2.png)

ps.
训练文件chat_bot_v2中，最后三块代码前两个是挂载谷歌云盘用的，最后一个是获取那些loss方便画图，不知道为什么回调函数里的tensorbord不好使，故出此下策；
预测文件里倒数第二块代码只有文字输入没界面，最后一块代码是界面，根据需求两块跑其一即刻。
