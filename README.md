# fudan_bert_homework

### 介绍

中文新闻标题分类， 基于pytorch，Bert的预训练模型 进行 finetune.

#### 地址

[GitHub - tengshiquan/fudan_bert_homework](https://github.com/tengshiquan/fudan_bert_homework)

bert预训练模型 pytorch_model.bin
下载地址：https://s3.amazonaws.com/models.huggingface.co/bert/bert-base-chinese.tar.gz

### 中文数据集

从[THUCNews](http://thuctc.thunlp.org/)中抽取了20万条新闻标题，文本长度在20到30之间。一共10个类别，每类2万条。数据以字为单位输入模型。

类别：0财经、1房产、2股票、3教育、4科技、5社会、6时政、7体育、8游戏、9娱乐。

数据集划分：

| 数据集 | 数据量 |
| --- | --- |
| 训练集 | 18万 |
| 验证集 | 1万  |
| 测试集 | 1万  |

##### 例子

| 标题                     | 分类  |
| ---------------------- | --- |
| 60年铁树开花形状似玉米芯(组图)      | 5   |
| 体验2D巅峰 倚天屠龙记十大创新概览     | 8   |
| 发改委治理涉企收费每年为企业减负超百亿    | 6   |
| 一年网事扫荡10年纷扰开心网李鬼之争和平落幕 | 4   |
| 2010英国新政府“三把火”或影响留学业   | 3   |
| 朝鲜要求日本对过去罪行道歉和赔偿       | 6   |
| 《口袋妖怪 黑白》日本首周贩售255万    | 8   |
| 图文：借贷成本上涨致俄罗斯铝业净利下滑21% | 2   |
| 组图：新《三国》再曝海量剧照 火战场面极震撼 | 9   |

#### 

#### 环境

python 3.7  
pytorch 1.1  
tqdm  
sklearn  
tensorboardX

## 效果

| 模型   | acc    | 备注      |
| ---- | ------ | ------- |
| bert | 93.47% | 单纯的bert |

#### 使用说明

```
# 训练并测试：
python run.py 
```
