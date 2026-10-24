# 如何写论文-Reference

> 💡 **参考文献绝对不是从Google Scholar、DBLP复制下来bib贴进去就行了，而是每一个都要自己手动编辑！！！确保格式正确、统一！**

## 参考文献整理步骤

1. 从DBLP复制bib条目

2. 修改统一的key，**统一采用作者姓+年份+关键词**，例如，

> **@inproceedings{zhou2024symagent,**

而不是<strong>@inproceedings{DBLP:conf/icml/ZhouL24</strong> 这种

3. 修改正确的标识，**会议是@inproceedings，期刊是@Article**

4. 删除publisher等无用字段，一般来说保留以下字段即可

> **author**
>
> **title**
>
> **booktitle / journal**
>
> **volume（期刊）**
>
> **number（期刊）**
>
> **pages**
>
> **year**

5. 统一大小写保护，直接复制下来的bib会把原本应该大写的自动变成小写，需要使用 **{}** 保护。

例如，<strong>title={{SymSkill}: Symbol and Skill Co-Invention for Data-Efficient Robot Learning}，</strong>如果不加{}就会全都变成小写。对于论文标题、或者一些常见的名字，例如LLM、GPT等，都需要使用大写保护，例如：

```text
title = {{GPT}-4o mini}
title = {{Qwen3}-8B}
title = {{LLM-SR:} {S}cientific Equation Discovery}
```

6. 关于Author：除非作者太多的情况，建议保留所有作者，如果作者实在太多，可以用et al.,代替，作者名称可以保留DBLP导出的作者格式，不需要改写

7. 关于booktitle / journal：

    1. **确保在参考文献中，同一个会议的引用，格式完全一致，不要有的用全称，有的用缩写；有的首字母大写，有的不大写等等。**

    2. 对于大部分会议，都应该写成如下形式，**Proceedings of   the xxth International Conference on Machine Learning。需要注意：**

        1. **届数用数字表示，注意序数词不要用错，1st, 2nd, 3rd, 4th, 5th……**

        2. **有些特殊会议没有届数而是年份，保证同一个会议的引用格式一致即可，例如：**

            1. **EMNLP：{Proceedings of the 2024 Conference on Empirical Methods in Natural Language Processing}**

            2. **CVPR:  booktitle =  {Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition}**

        3. 部分会议没有Proceedings，保证同一个会议格式一致即可，例如

            1. **NeurIPS： booktitle = {Advances in Neural Information Processing Systems}（注意很多时候NeurIPS引用后面会有一个数字，例如[Advances in Neural Information Processing Systems 34](https://proceedings.neurips.cc/paper_files/paper/2021)，34这种数字删掉）**

        4. **会议名称首字母都改为大写**

8. Volume/Number：对于期刊引用，需要有准确的期卷号，例如：

    ```text
    journal={Nature},
    volume = {529},
    number = {7587},
    pages = {484--489},
    year={2016}
    ```

9. Pages：除部分特殊会议没有pages，例如ICLR，其余保持一致即可。

## 投稿前自检

- [ ] 无关的字段是否删除，例如Publisher、URL等

- [ ] Title：是否有标题大小写混乱，即有的文章标题每个首字母都大写，有的只有第一个字母大写

- [ ] Author：作者名称是否写全，作者太多的改为et al.，是否有大小写混乱

- [ ] Booktitle/Journal：同一个会议格式是否统一、是否有无关词汇（例如NeurIPS的数字）、大小写是否一致。

- [ ] Volume/Number：期刊引用期卷号不要缺失

- [ ] Pages：除了ICLR等没有页码的会议，其他不要缺失页码

- [ ] 是否有重复的文献

[← 上一篇：如何写论文-Experiments](experiments.md) · [返回目录](README.md) · [下一篇：如何 Rebuttal →](rebuttal.md)

来源：[飞书原文](https://dy8q0bnq8y.feishu.cn/wiki/A4q2wSnmRi91rykHke1cQIhnnAh?from=from_copylink)
