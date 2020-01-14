### 背景简介
研究生入坑机器学习，便学了这本21个项目玩转深度学习 奈何书里版本是基于**Linux+python2.7+tensorflow1.4.0**  
对新人来说很不友好，故希望改成一个友好的版本 大家能直接运行增强自信，不会配置个环境配置一星期 真是心态炸啦  
说一下我的版本 应该萌新都可以装好  **windows+python3.6+tensorflow1.4.0**  
为什么是python3.6呢，因为python3.7只支持有限的几个tensorflow版本 这个坑阻挠了我一个下午 下面进入正题
### 环境配置  
首先每个人应该都具备了Anaconda 如果没有，回去面壁 这个切换不同环境真的挺友好
creat一个新的环境，拿这个专门做这本书上的例子，记得一定要选择
# python 3.6!!
# python 3.6!!
# python 3.6!!  
然后升级下pip这个包 因为新建个环境pip只有9.0，而最新的已经19了 这步在anaconda就可以完成 不多啰嗦  
顺便在anaconda里装一下Jupyter notebook 我以后代码都在这里完成 有及时的反馈
好的 升级完后打开anaconda Powershell Prompt 
输入  
```
conda activate *your env name*激活环境 我的是door 所以输入的是door  
```
然后输入以下指令  
```
pip install tensorflow -i https://pypi.douban.com/simple  
```
再试了各种清华源，中科大源后没想到还是豆瓣最香。。  
听说清华源已经不维护了，对这两个源感兴趣的同学 查看这个 [链接](https://zhuanlan.zhihu.com/p/95100538)
如果中间没错误的话 输入  
```
python  
>>>import tensorflow as tf
>>> tf.__version__ 
```
记住是**两个下划线**哦  
好 到这一步其实我装了一下午 吃个饭一会更。。  
我回来了 接下来终于要正式开始啦
### exp1 MNIST机器学习入门  
+ 首先导入数据集  
