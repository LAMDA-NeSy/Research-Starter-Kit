# 如何Rebuttal

## Rebuttal技巧和一些原则

- Rebuttal时不要漏点，要逐点回应做到有问必答。若因篇幅有限，可将类似的意见合成一点，万不可因篇幅有限擅自删除一些要点或遗漏要点，以免造成含糊不清、浑水摸鱼之嫌，一旦被审稿人发现会在paper discussion阶段当作硬伤来“置于死地”；

- Rebuttal时需要揣摩审稿人倾向，“一切可以团结的力量都要团结，不中立的可以争取为中立，反动的也可以分化和利用”。有的审稿人会在意见中明确表示，“如果解决了xxx，我就会提升评分”，对此一定要充分争取；对于某些审稿人提出的不足（如novelty），可能刚巧是另一位审稿人提出的优点（“This paper is interesting and novel”），一定要为我所用，让两位审稿人在paper discussion中“短兵相接”；对于borderline的审稿人，一定要充分“拉拢腐蚀”；对于初审给了positive分数的审稿人，一定要巩固基础；对于初审给了negative分数的审稿人，一定要放绝大多数的精力和rebuttal篇幅来解释澄清，争取“冰释前嫌”；

- Rebuttal是“一盘棋”，整篇rebuttal需要统筹协调，与正文、review配合的相得益彰，同时还需注意rebuttal篇幅资源的分配和优化。哪位审稿人应多分配笔墨、哪个问题应多着力回应都需要根据整体审稿意见情况深入思考、统筹安排；

- Rebuttal中能缩写的尽量缩写，从而节省空间，将资源留给更需要的回应；

- Rebuttal时若发现审稿人的factual error，如ta提出的某个观点有显然错误、提出需要对比的数据集显然不是该领域常用的数据等，作者可在rebuttal回应此人时首先指出其错误，先下一城，赢得主动。要知道rebuttal除了该审稿人之外，其他审稿人以及AC都会看到。此外，这一问题还可以在AC Message中指出，降低该审稿人意见在AC心中的置信度；

## 常见问题和回答技巧

### 针对Novelty不足的问题

一般而言，Novelty不足主要包括两个方面：1）与别人的方法差异不大；2）简单的A+B的组合；

可以尝试重新梳理和强调文章的重要贡献，然后澄清并不是trivial的简单combine，再强调一下motivation和intuition，用另一种方式将文章亮点表达出来。

同时，可以尝试“围魏救赵”，即：若审稿人针对方法的某个部件提出novelty不足，可强调其他部件或整个方法的范式是前所未有的；或claim说方法简单有效，效果好，性能SOTA等。

### 针对Factual Error的问题

这种比较麻烦，基本没有太多可以rebuttal的余地，往往只能大方承认，并表示感谢，同时表示会在final version中更正错误。如果是因为写作问题，导致reviewer没有理解正确，也可以承认，并解释一下，说“我们已经修改了这部分描述，实际上是这样做的，并不是你理解的那样，blabla”；

### 效果不明显（提升有限）

1. 可以尝试找一些参考文献，论证自己方法的涨点幅度和其它SOTA的涨点幅度是可比的，“你看，别人发在顶会的结果相比baseline也是涨这么多”

2. 可试着找出自己的方法有没有什么性能提升特别明显的场景，作为一个特色展示出来，并说明这些场景非常重要，或者看一下是否有实验设置的不公平之处，如果可以，最好能够加上公平的设置下的对比结果，“你看，虽然他们的论文汇报的性能是xxx，但是这个实验是在xx条件下进行的，我们的更困难，如果换成我们的设置，他们的性能就不行了”

3. 其他方面的好处，比如效率？通用性？鲁棒性？等等

### 实验不充分

尽量补充实验，如果不能补充，想办法做出解释，比如实验规模太大，rebuttal期间无条件做出，可在rebuttal中承诺final version中补上；而对于要求不合理的实验意见，可实事求是的说明为何无需做实验，可以多加一些“证据” 比如参考文献，支撑你的说法；

### 语法，结构，参考文献遗漏等问题

大部分时候承认、感谢、并修改即可。

## AC Message

对于有恶意、或者出现事实错误被你抓到把柄的审稿人，可以向AC写投诉信举报

如果在审稿意见中发现了审稿人的“问题”，如不专业、对文章涉及领域不熟悉、自我矛盾等，可以抓到把柄，向AC写投诉信举报从而引起AC注意。

以下列举一些可能的AC message的写法：

- 违背常识：Please note that Assigned Reviewer #id has made some statements that are either **against the common-sense** in our field or self-contradictory (ironically his/her own confidence rating is "very confident").

- 自相矛盾：We want to bring to your attention the very flawed review #id. This reviewer is s**elf-contradictory**, cf. Comment #id1, Comment #id2, and Response #id. blabla

- 严重偏见：We would like to raise attention to AC that unfortunately Reviewer #id holds a **very biased view** towards the contributions of our paper. blabla

## 常用表达

以下列举一些rebuttal中的常用句式，供大家选择使用：

- <u>开头</u>

    - Thank you for your suggestion.

    - Thank you for the positive/detailed/constructive comments.

    - We sincerely thank all reviewers and ACs for their time and efforts. Below please find the responses to some specific comments.

    - We thank the reviewers for their useful comments. The common questions are first answered, then we clarify questions from every individual review.

    - We thank the useful suggestions from the reviewers. Some important or common questions are first addressed, followed by answers to individual reviews.

- <u>表达同意</u>

    - We thank the reviewer for pointing out this issue.

    - We agree with you and have incorporated this suggestion throughout our paper.

    - We have reflected this comment by …

    - We can/will add/compare/revise/correct ... in our revised manuscript/our final version.

- <u>表达不同意</u>

    - We respectfully disagree with Reviewer #id that ...

    - The reviewer might have overlooked Table #id ...

    - We can compare ... but it is not quite related to our work ...

    - We have to emphasize that ...

    - The reviewer raises an interesting concern. However, our work ...

    - Thank you for the comment, but we cannot fully agree with the comment. As stated/emphasized ...

    - You have raised an important point; however, we believe that ... would be outside the scope of our paper because …

    - This is a valid assessment of …; however, we believe that ... would be more appropriate because ...

- <u>解释澄清</u>

    - We have indeed stated/included/discussed/compared/reported/clarified/elaborated ... in our original paper ... (cf. Line #id).

    - As we stated in Line #id, ...

    - We have rewritten ... to be more in line with your comments. We hope that the edited section clarifies …

- <u>额外信息与解释</u>

    - We have included a new figure/table (cf. Figure/Table #id) to further illustrate…

    - We have supplemented the xxx section with explanations of ...

    - Thank you for the comment. We will explore this in future work.

## 更多资料

1. Rebuttal指南：https://github.com/MLNLP-World/Paper-Rebuttal-Tips

[← 上一篇：如何写论文-Reference](references.md) · [返回目录](README.md)

来源：[飞书原文](https://dy8q0bnq8y.feishu.cn/wiki/M9d1wv5Efi2aG4kH4IDc5zqVnQh?from=from_copylink)
