---
layout: post
title: TensorFlow的安装（Windows）
category: Tech
tag: [Tech,tensorflow]
---

老板把我分在图像处理组，叫我用TensorFlow框架进行人脸的识别。作为一个初入深度学习的小白，首先遇到的问题就是，如何安装TensorFlow。


----------

1、python安装

首先需要说明的是，在win下安装Python，我建议使用anaconda。anaconda集成了很多必须的库，还可以建立环境使得不同项目分隔开。

 - anaconda下载安装
下载地址：https://www.anaconda.com/download/
安装时注意将添加到路径和作为默认Python勾选上

 - 一些常用的conda命令

查看conda版本

    conda --version
    
创建环境

    conda create --name python35 python=3.5
    
查看当前所处环境

    conda info --envs

激活某个环境

    activate python35
    
返回默认环境（base）

    deactivate
    
删除已有环境

    conda remove --name python35 --all

2、TensorFlow安装

1)创建名为tensorflow的环境

    conda create -n tensorflow pip python=3.66
    
2)验证环境是否创建成功(会显示已创建的tensorflow）
 
    conda info --envs
    
3)激活名为tensorflow的环境

    activate tensorflow

4)安装tensorflow

    pip install --ignore-installed --upgrade tensorflow
    
5)验证是否成功安装

    import tensorflow as tf
    hello = tf.constant('Hello, TensorFlow!')
    sess = tf.Session()
    print(sess.run(hello))
    
**写在最后：**

 - 我尝试装了GPU版本，由于我的显卡比较渣是940MX，用一个例程比较之下我还是选择了CPU版本。如果要安装GPU版本，参考[GPU版本TensorFlow安装][1]。
 - 在Windows下使用Python还是推荐安装anaconda，免去一大堆依赖包的安装，环境创建和删除也容易多了。
 - 学习深度学习还是推荐把[吴恩达的深度学习课程][2]好好吃透。

    



    


    


  [1]: https://blog.csdn.net/u010099080/article/details/53418159
  [2]: http://mooc.study.163.com/smartSpec/detail/1001319001.htm