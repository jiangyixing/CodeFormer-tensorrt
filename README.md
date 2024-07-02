# CodeFormer-tensorrt
​
源码：
1.环境说明
        cuda==11.8,cudnn==8.6
        TensorRT-8.5.1.7.Windows10.x86_64.cuda-11.8.cudnn8.6(不能用pip安装。要用tensorrt安装包中的python文件夹下的wsl文件进行安装)
        python==3.9
        pytorch==2.3.0
        gpu==4070ti

具体库对应的版本见，项目的new_requirements.txt 脚本

2.效果对比
 1.tensorrt推理634*360大小的图像，每帧速度在0.055-0.075之间。而原始的codeformer的pytorch推理在每帧速度0.10-0.12之间
2.tensorrt推理844*480大小的视频，一共5s合计169帧。全部推理完耗时120.37s。而原始的codeformer的pytorch推理在124s

没有使用tensorrt加速的结果，即使用官方的pytorch进行推理



使用tensorrt加速的结果：



3. 本人参考教程
（1）tensorrt安装教程

https://avoid.overfit.cn/post/1ee573c219354fe0ad850909ba9f8699#/
（2）tensorrt使用教程

https://www.bilibili.com/video/BV1yg4y1t71M/?spm_id_from=333.788&vd_source=36dfc93b8d0b29437be5ed1a8b6c7d66

https://www.bilibili.com/video/BV16r421V7MA/?spm_id_from=333.788&vd_source=36dfc93b8d0b29437be5ed1a8b6c7d66

​
