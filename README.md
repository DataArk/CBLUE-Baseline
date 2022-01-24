# CBLUE-阿里天池中文医疗NLP打榜Baseline

## 简介

名称：CBLUE: A Chinese Biomedical Language Understanding Evaluation Benchmark

测评任务：CBLUE 1.0是由CHIP会议往届的学术评测比赛和阿里夸克医疗搜索业务的数据集组成，包括医学文本信息抽取（实体识别、关系抽取）、医学术语归一化、医学文本分类、医学句子关系判定和医学QA共5大类任务8个子任务。

任务类型：文本分类、文本相似、命名实体识别、关系抽取和术语标准化（可以看成没有上下文的实体链接任务）

测评链接：https://tianchi.aliyun.com/dataset/dataDetail?dataId=95414

baseline方法介绍：https://mp.weixin.qq.com/s/O4r-gSr3EWdoCG5nHZIghQ

## 环境

```
pip install ark-nlp
pip install pandas
```

## 使用说明

项目目录按以下格式设置，注意运行CHIP-CDN时，需要其代码移动到code目录下

```shell
│
├── data                                    # 数据文件夹
│   ├── source_datasets                     
│   ├── task_datasets           
│   └── output_datasets                           
│
├── checkpoint                              # 存放训练好的模型
│   ├── ...           
│   └── ...                                      
│
└── code                                    # 代码
```


下载数据并解压到`data/source_datasets`中，运行`code`文件夹中的`.ipynb`文件，最终提交文件会生成在`data/output_datasets`

