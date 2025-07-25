# ❤ HEART 共情力打分模型
![模型演示](https://github.com/Rinnnnzy/HEART_Empathy_score/blob/main/%E8%AF%84%E5%88%86%E6%BC%94%E7%A4%BA.gif)

### 项目背景：

在社交媒体上，人们热衷分析人生经历与感悟。高热度文章常以触发情绪、引发共鸣的文字为特征。
本项目专注于文案生成场景，特别是以小红书风格为特点的创造性AI输出。项目的核心目标是建立一套科学且可量化的评测体系，用于评估LLM在**情感共鸣**方面的表现，甚至利用LLM评估文本共情力从而实现**文本热度的预测**。


### 项目目标：

开发文本共情力打分模型，通过具体指标量化文本共情力，评估LLM生成文本的共情力。目标是生成更具情感穿透力的文案，并利用打分模型预测文本的热点程度。


### 具体工作内容：

1. 根据[HEART分类法](https://arxiv.org/abs/2405.17633)设计文本共情力评分指标

  指标如下：
- Vividness of emotions
- Vividness of setting
- Character vulnerability
- Cognition
- Optimistic tone
- Plot volume
- Resolution
- Character development
- Emotion shifts

2. 运用[deepeval](https://github.com/confident-ai/deepeval)搭建好的DAG算法框架构建评分框架


### 最终成果：
项目通过9个指标对文本进行打分，实现了共情力的量化评估。同时，项目实现了批量文本打分，其中大部分指标的拟合效果良好，MSE值低，展示了其在实际应用中的有效性。

---
### To do list
- 细化指标分数设定与prompt
- LLM裁判易对环境描述、人类认知描述产生误判。需引入机器学习等更复杂的方法训练模型
- 共情还关系读者自身的共情能力，相似经历与文化背景等。需描绘用户画像。根据用户特征动态调整评分标准
- 落实到社交媒体等应用场景。利用打分系统进行文本热度预测


>模型运行不稳定😢。我将继续完善该模型！！
