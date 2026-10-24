# 如何写论文-Experiments

## Experiments 的大致结构

常见结构如下：

1. Experimental Setup

2. Main Results

3. Ablation Study

4. Analysis / Further Study

5. Case Study / Visualization

6. Robustness / Generalization

7. Efficiency / Cost Analysis

并不是每篇论文都需要全部包含。实验结构应服务于本文贡献，而不是为了显得实验很多

## 先写 Experimental Setup

Experimental Setup 是 Experiments 的基础，作用是让读者理解实验是在什么条件下完成的。

通常需要交代：

- 使用哪些 datasets / benchmarks

- 比较哪些 baselines

- 使用哪些 evaluation metrics

- 模型实现细节是什么

- 训练和推理参数是什么

- 实验重复次数、随机种子和统计方式是什么

- 所有方法是否在公平条件下比较

这一部分要清楚、具体，避免模糊表达，如果细节过多可以在附录中进一步补充。

## Main Results 要服务于核心结论

Main Results 通常是 Experiments 中最重要的部分，往往对应论文的主表和主图。

这一节要回答：

- 本文方法是否优于已有方法？

- 在哪些数据集或任务上提升明显？

- 哪些结果最能支撑论文贡献？

- 是否存在没有提升或提升较小的情况？

**写 Main Results 时，不要只是说 “Table 1 shows the results”，应该告诉读者从表中应当看什么。**

推荐的结构：

> Table 1 compares our method with existing baselines on ... . Our method achieves the best performance on ... , suggesting that ...

## Ablation Study 说明方法为什么有效

**Ablation Study 的任务是证明：本文提出的关键模块或设计不是随意添加的，而是确实有用。**

常见 ablation 包括：

- 去掉某个模块

- 替换某个模块

- 改变某个训练目标

- 改变 prompt / retrieval / memory / ranking 策略

- 改变数据量或训练配置

- 比较不同模型规模或参数设置

Ablation 的写法应当围绕设计动机展开：

> To evaluate the contribution of ..., we remove ... and compare the resulting model with the full model.

## Analysis 用来加深理解

**除了主结果和消融实验，很多论文还需要 Analysis 部分，用来解释方法的行为。**

常见 analysis 包括：

- 不同类别样本上的表现

- 不同难度任务上的表现

- 不同数据规模下的表现

- 不同模型规模下的趋势

- 不同错误类型的分布

- 对超参数的敏感性

- 对提示词、检索数量、上下文长度的敏感性

- 与人类表现或专家标注的一致性

Analysis 的目标不是重复主表，而是帮助读者理解：

> 方法在哪些情况下更好？为什么更好？什么时候不够好？

## Case Study 和 Visualization

如果方法或任务比较复杂，可以加入 case study 或 visualization。

适合使用 case study 的情况：

- 结果难以只用数字说明

- 需要展示模型输出质量

- 需要比较不同方法的行为差异

- 需要展示失败案例

- 需要让读者理解任务难度

## 一些需要注意的细节：

1. **邀请读者查看图表：不能假设读者会自动去看图。你需要明确地引导：**

    - *Figure 1 shows the results...*

    - *As can be seen in Fig. 1...*

    - *The results are summarized in Table 1...*

2. **描述关键结果：选择重要的、典型的、或特别有趣的结果进行详细描述，不要对所有结果一视同仁。你选择描述哪个，读者就会认为哪个重要。**

3. **使用评价性语言：不要让原始数据自己说话。用评价性的词语告诉读者，这些数字意味着什么**

4. **提及问题与异常**

    如果你的结果中有瑕疵、异常或不符合预期的数据，怎么办？不要隐瞒，但要用弱化语言处理。

    - ❌ 新手：完全不提异常数据 → 看起来像“没发现问题的外行”

    - ✅ 高手：*"Although the average uncertainty slightly exceeds the 50% acceptability limit, nevertheless these results suggest that..."*（承认问题 + 弱化影响 + 转向正面）

    - 常用弱化词：***slightly, somewhat, only approximate, a minor deficit, negligible, not significant, it should be noted that...***

[← 上一篇：如何写论文-Methods](methods.md) · [返回目录](README.md) · [下一篇：如何写论文-Reference →](references.md)

来源：[飞书原文](https://dy8q0bnq8y.feishu.cn/wiki/KHgSw2MkrikxlskGe5qclkdbn2c?from=from_copylink)
