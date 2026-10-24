# 如何写论文-Abstract

## 基本思路

论文摘要并非“论文简介”，而更应被视为一份**贡献说明书（statement of contribution）**。其目标不是全面概述论文内容，而是在有限篇幅内，使审稿人清晰地理解：**本文解决了什么问题、提出了什么关键思想、以及这些贡献对领域的意义何在**。因此，摘要不宜冗长，而应高度凝练、逻辑清晰。

## 五句话原则

在一般情况下，摘要可以遵循下面的 **“五句话原则”**，对应五个核心要素：

1. **任务背景(Context)-- 1句话**

    1. 用最精炼的语言描述论文的大方向与任务范畴，使审稿人能够在第一时间判断论文所属领域以及所关注的核心问题。不要铺垫过多常识，直接切入主题。

2. **科学问题(Problem)--1-2句（最关键）**

    1. 这是比方法还要关键的部分，要讲出来现有研究的挑战与痛点

    2. 理想情况下，这里要是一个“结构性问题”而不是一个“经验现象”，或者从经验现象出发，总结出来的结构性问题。

    3. 比如，LLMs often fail in xxxx task，这就属于经验现象，给人一种修修补补、贡献不大的感觉，一下子就掉到了borderline区域。

    4. 要给出一些更加本质的问题，从现象上升到机理，比如是理论有缺陷，泛化能力弱，还是稳健性不足？

3. **方法创新(Methodology)--1-2句**

    1. 提出核心的解决方案，要尽可能的凝练出思想，不要堆太多细节，比如要解决稳健性弱的问题，是通过什么方法解决的，提出了新的架构？新的损失？还是新的数据合成方法？核心的思想是什么？

    2. 关键在于让审稿人理解“为什么这种方法在逻辑上能够解决前述问题”

4. **结论与贡献(Results)--1句**

    1. 实验描述应以**具体、可量化的指标**为主，而非泛泛而谈；很多同学喜欢直接写一句significant performance improvement，这种写法就很普通，因为所有的论文都可以这么写。反之，明确指出在多少个数据集、对比了哪些代表性方法，以及在什么指标上取得了多大幅度的提升，会更具说服力。

    2. 另外有一点非常重要但是经常被忽略的，**实验结论应当与前文提出的科学问题形成明确呼应与逻辑闭环**，比如，如果论文声称解决的是稳健性不足的问题，那么实验中就应突出在何种干扰或变化下，本文方法相较于现有方法提升了多少稳健性；相比之下，仅报告整体 accuracy 往往不足以支撑核心 claim。

## 优秀案例

1. 下面这个例子取自论文Train for the Worst, Plan for the Best: Understanding Token Ordering in Masked Diffusions（ICML 2025 Outstanding Paper)，是一个从问题分析出发提出算法的文章。问题部分非常明确和本质“trade off complexity at training time with flexibility at inference time"，结论部分，非常有说服力：from 7% to 90%，超越了7倍参数量的模型

![摘要优秀案例 1](../../assets/images/abstract/example-1.png)

2. 下面这一个例子，取自ICML 2025 Oral Paper: Accelerating LLM Inference with Lossless Speculative Decoding Algorithms for Heterogeneous Vocabularies。属于非常常见的解决现有xxx方法xx问题的文章，跟大部分同学做的比较像。也是一句话确定背景，LLM推理加速很重要。然后用两句话指出问题，SD方法require the drafter and target models share the same vocabulary。然后一句话讲清楚本文工作，提出了一种不依赖shared-vocabulary constraint的方法，实验结果，回应LLM加速的问题，不依赖约束，实现了2.8倍的加速。

![摘要优秀案例 2](../../assets/images/abstract/example-2.png)

3. 这是一个benchmark论文的例子，取自ICML 2025 Oral Paper: LLM-SRBench: A New Benchmark for Scientific Equation Discovery with Large Language Models。也是一句话确定背景，Scientific equation discovery很重要。然后2句话明确背景与问题，LLM用于SR得到了很多关注，但是难以评估，不能反映真实能力；本文提出了一个LLM-SRBench，覆盖了多少个问题（有数字，239），4个领域，2大类别LLM-Transform和LSR-Synth。最后实验评估了多少模型，这里如果把several SOTA methods换成评估了几类算法、多少个模型会更好。结论发现了什么现象、对该领域有何贡献。

![摘要优秀案例 3](../../assets/images/abstract/example-3.png)

[← 上一篇：论文画图指南](figures.md) · [返回目录](README.md) · [下一篇：如何写论文-Introduction →](introduction.md)

来源：[飞书原文](https://dy8q0bnq8y.feishu.cn/wiki/Tz2pwvxTyiBK0zkCVszcZmJ3nwd?from=from_copylink)
