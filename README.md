# Chinese-ChatBot
## 环境配置
`Keras`<br>`python3.68`<br>`windows10`<br>`jupyter`<br>
## 关键点
* LSTM
* seq2seq
* attention 实验表明加入attention机制后训练速度快，收敛快，效果更好。

## 语料及训练环境
  青云语料库10万组对话，在google colaboratory训练。

## 界面用Tkinter
![](https://github.com/jiayiwang5/Chinese-ChatBot/blob/master/image/image.png)

## Attention权重可视化
![](https://github.com/jiayiwang5/Chinese-ChatBot/blob/master/image/image2.png)

## 其他
* 训练文件chat_bot中，最后三块代码前两个是挂载谷歌云盘用的，最后一个是获取那些loss方便画图，不知道为什么回调函数里的tensorbord不好使，故出此下策；<br>
* 预测文件里倒数第二块代码只有文字输入没界面，最后一块代码是界面，根据需求两块跑其一即刻；<br>
* 代码中有很多中间输出，希望对你理解代码提供了些许帮助;<br>
* models里面有一个我训练好的模型，正常运行应该是没有问题的，你也可以自己训练<br>
* 本人能力有限，并未找到量化对话效果的指标，因此loss只能大致反映训练进度。<br>
