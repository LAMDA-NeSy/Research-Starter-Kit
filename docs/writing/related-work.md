# 如何写论文-Related Works

> 📣 Related Work 不是文献罗列，也不是把读过的论文逐篇摘要。它的核心任务是帮助读者理解：
>
> 1. 本文处在什么研究脉络中。
>
> 2. 已有方法可以分成哪些主要路线。
>
> 3. 每条路线解决了什么问题，又留下了什么不足。
>
> 4. 本文与已有工作的关系是什么：延续、区别、补充还是超越。
>
> **一句话说，Related Work 要回答：**
>
> **“别人已经做了什么？我们的工作和他们有什么关系？为什么还需要我们的工作？”**
>
> **Related Work = 分类 + 概括 + 代表工作 + 局限 + 本文定位。**

## Related Work 和 Introduction的区别

Introduction 中也会提到已有工作，但它的目的主要是引出研究问题和 gap

Related Work 的目的更具体：系统梳理与本文最相关的研究脉络，并定位本文贡献

可以这样区分：

- Introduction：讲故事，建立动机

- Related Work：画地图，说明位置

## Related Works的常见组织结构

### 按研究方向组织

适合大多数论文，每一节对应一个研究方向

### 按方法类别组织

如果针对本文研究的问题，已经有大量的方法了，可以尝试按照不同的技术路线来组织，重点比较不同技术路线的假设、优势和限制。

## 每一段的推荐写法

**Related Work 中的每一段通常可以按下面逻辑写：**

1. **先概括一个研究方向**

2. **再列举代表性工作**

3. **然后总结这些工作的特点**

4. **最后指出它们与本文的关系或局限**

例如：

“已有研究从……角度研究了该问题。早期工作主要……；近期方法进一步……。这些方法在……方面取得了进展，但通常依赖……，因此难以处理……。与这些工作不同，本文关注……。”

## 写 Related Work 时要避免的问题

1. **不要逐篇论文平铺直叙**\
    错误写法：A 做了什么，B 做了什么，C 做了什么。\
    更好的写法：A、B、C 属于同一类方法，它们共同解决了什么问题，但仍存在什么限制。

2. **不要只夸别人，也不要只批评别人**\
    Related Work 的语气应客观。重点是定位本文，而不是证明别人都不行。

3. **不要引用过多但没有分类**\
    引用多不等于相关工作写得好。分类清楚比引用数量更重要。

4. **不要把 Related Work 写成 Introduction 的重复**\
    如果 Introduction 已经讲过动机，Related Work 应进一步展开技术路线和差异。

5. **不要只写相似工作，不写差异**\
    读者最关心的是：你的工作和这些论文到底有什么不同。

## 常用表达方式

### 引入一个研究方向

- A large body of work has studied ...

- Prior research on X can be broadly divided into ...

- Existing approaches to X typically fall into three categories.

- Recent studies have explored X from the perspective of ...

### 总结已有方法

- These methods generally rely on ...

- Most existing approaches assume that ...

- A common strategy is to ...

- Previous work has mainly focused on ...

### 指出不足

- However, these methods are limited in ...

- Despite their success, they often fail to ...

- This line of work does not explicitly consider ...

- Few studies have systematically examined ...

### 说明本文区别

- In contrast, our work focuses on ...

- Unlike prior work, we ...

- Our work is complementary to ...

- While these studies address ..., we investigate ...

- The closest work to ours is ..., but it differs in ...

## 贡献定位的几种关系

写 Related Work 时，不一定总要说“我们比别人更好”。可以更精确地说明关系：

1. **Extension**\
    本文扩展了已有工作，例如扩展到新场景、新任务、新数据或新模型。

2. **Complement**\
    本文与已有工作互补，例如已有工作研究方法，本文研究评测。

3. **Contrast**\
    本文与已有工作不同，例如假设、任务定义、评价目标不同。

4. **Unification**\
    本文统一了多个过去分散的问题或方法。

5. **Re-evaluation**\
    本文重新评估已有方法，发现过去评价存在遗漏或偏差。

## 图表

如果需要比较多个已有工作在若干维度上的差异，适合使用表格的方式来补充说明，比如下面的表格。但这种情况下需要注意的是，**表格中的比较维度应当是该领域公认且合理的评价维度，并且与论文的核心问题直接相关**。应避免为了突出本文优势而临时拼凑若干“本文有、相关工作没有”的特征，否则容易让审稿人觉得比较标准不够客观，甚至是在刻意制造差异。

![相关工作比较表格](../../assets/images/related-work/comparison-table.png)

下面这个MMMU的related works表格很适合 benchmark 论文参考：展示数据覆盖的学科、subjects、subfields、image types 等。

![MMMU 与已有基准的比较](../../assets/images/related-work/benchmark-comparison.png)

[← 上一篇：如何写论文-Introduction](introduction.md) · [返回目录](README.md) · [下一篇：如何写论文-Methods →](methods.md)

来源：[飞书原文](https://dy8q0bnq8y.feishu.cn/wiki/CLSAwWm6qifjwQkTd82czgMNnYf?from=from_copylink)
