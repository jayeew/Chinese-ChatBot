# Chinese-ChatBot/中文聊天机器人
* 作者已经全面转到~~GNN图神经网络方向~~C++开发，不再跟进NLP方面，项目代码停止维护。遥想项目完成时，网上资源甚少，作者一时兴起初次接触NLP与Deep Learning，克服重重困难，终于写出这个Toy Model。因此，作者深知小白不易，所以即使项目不再维护，但issue或邮件(jayeew@qq.com)一定会及时答复，以帮助Deep Learning新人。(Tensorflow我用的版本太老了，建议后来者用Pytorch重构一遍，我懒得写了)<br>
* GNN方面:
- 改编整理了一套基准对比模型：[GNNs-Baseline](https://github.com/jayeew/GNNs-Baseline) ，以方便快速验证idea。
- 本人的论文ACMMM 2023 (CCF-A) 开源代码在这[LSTGM](https://github.com/jayeew/LSTGM)。
- 本人的论文ICDM 2023 (CCF-B) 开源代码还在整理中。。。[GRN]()
* 欢迎同好补充、交流、学习。
## 环境配置
| 程序         | 版本      |
| ---------- | ------- |
| python     | 3.68    |
| tensorflow | 1.13.1  |
| Keras      | 2.2.4   |
| windows10  |         |
| jupyter    |         |

## 主要参考资料
* 论文[《NEURAL MACHINE TRANSLATION BY JOINTLY LEARNING TO ALIGN AND TRANSLATE(**点击标题下载**)》](https://arxiv.org/pdf/1409.0473.pdf)
* Attention结构图<br>![](https://github.com/jiayiwang5/Chinese-ChatBot/blob/master/image/image3.png)

## 关键点
* LSTM
* seq2seq
* attention 实验表明加入attention机制后训练速度快，收敛快，效果更好。
## 语料及训练环境
  青云语料库10万组对话，在google colaboratory训练。
## 运行
### 方式一：完整过程
- **数据预处理**<br>
  `get_data`<br>
- **模型训练**<br>
  `chatbot_train`(此为挂载到google colab版本，本地跑对路径等需略加修改)<br>
- **模型预测**<br>
  `chatbot_inference_Attention`<br>
### 方式二：加载现有模型
- 运行`chatbot_inference_Attention`<br>
- 加载`models/W--184-0.5949-.h5` 
## 界面(Tkinter)
![](https://github.com/jiayiwang5/Chinese-ChatBot/blob/master/image/image.png)

## Attention权重可视化
![](https://github.com/jiayiwang5/Chinese-ChatBot/blob/master/image/image2.png)

## 其他
* 训练文件chat_bot中，最后三块代码前两个是挂载谷歌云盘用的，最后一个是获取那些loss方便画图，不知道为什么回调函数里的tensorbord不好使，故出此下策；<br>
* 预测文件里倒数第二块代码只有文字输入没界面，最后一块代码是界面，根据需求两块跑其一即刻；<br>
* 代码中有很多中间输出，希望对你理解代码提供了些许帮助;<br>
* models里面有一个我训练好的模型，正常运行应该是没有问题的，你也可以自己训练<br>
* 作者能力有限，并未找到量化对话效果的指标，因此loss只能大致反映训练进度。<br>

