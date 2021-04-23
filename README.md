## CPM官方GitHub地址：https://github.com/TsinghuaAI/CPM-Finetune

本项目的主要目的是本人在使用CPM的过程中遇到的坑，以及能够使用CPM进行下游任务。

## 1 安装

首先安装 pytorch 等基础依赖，再安装[APEX](https://github.com/NVIDIA/apex#quick-start)以支持 fp16，然后安装 deepspeed：

**安装基础依赖：**

```[bash]
conda create -n CPM python=3.7
source activate CPM
cd CPM-Finetune
pip install -r requirements.txt
```

**安装 apex：**

```[bash]
git clone https://github.com/NVIDIA/apex
cd apex
python setup.py install
```

若是无法手动安装：
进入apex官方: GitHub https://github.com/NVIDIA/apex 将其下载下来：我第一次用了git clone，显示出错，要注意。

```[bash]
cd apex-master
python setup.py install
```

**安装 deepspeed**

```[bash]
pip install deepspeed

