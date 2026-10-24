# AI辅助科研的一些Tips

## 快捷键

- **`!`** → 执行会话外的 shell 命令，输出会进入上下文

- **`@`** → 引用文件 / 路径 (带自动补全)

- **`#`** → 写记忆：把一条内容追加进 `CLAUDE.md`，不用打开文件

---

- **换行(不发送)：**`Command + J` 或 `Option + Enter`

- <strong>`Command + U`：</strong>清空当前输入行

- <strong>`Command + R`：</strong>搜索历史 prompt

- <strong>`Command + V`：</strong>粘贴截图

---

- **`Shift + Tab`** → 循环切换三种模式：

    1. 普通：每次动手前询问

    2. plan mode：只规划、不改文件；先规划后编码

    3. auto-accept edits：自动接受编辑、连续执行

  `d. claude --dangerously-skip-permissions`：允许所有操作

- prompt 里写 `think` / `think hard` / `ultrathink` → 逐级提高推理预算

---

- **`Esc`** → 立刻打断当前动作(不退出会话)

- **双击 `Esc`(= `/rewind`)** → 回退到之前某条消息

- **`/rewind`(checkpoints)** → 把对话或代码文件回滚

    - 双击 Esc 回退对话；`/rewind` 能回滚代码文件

---

- <strong>上下文(context)是当前这段对话，</strong>临时的，会话越长越满、越慢，退出当前会话就没了

- <strong>记忆(`CLAUDE.md`)是写进文件的项目约定，</strong>持久的、清空上下文也不丢

- **`/compact`** → 压缩成摘要后继续，会话变慢 / 快满时用

- **`/clear`** → 彻底清空，换全新会话

- **`/cost`** → 查看本次 token 消耗

- **`#`** → 随手追加一条约定

- **`/init`** → 扫描代码库、生成 `CLAUDE.md` 初稿

- **`/export`** → 把当前所有会话内容导出成一个文件

- **`/remote-control`**(新版本)→ 开启远程控制，从别的设备(如手机 Claude App)监控 / 操控

## 其他技巧

### 用 /branch 管理上下文

- 整个会话就像一棵树，branch 是在任意 turn 标记一个检查点，可以从这些检查点 resume

- 每个对话尽量只干一件相同研究方向的事，让上下文干净一些~

- 发现某个 turn 的尝试比较失败，可以用 /rewind 或者连续按两下 Esc 来回退

### 在动手前对齐尽可能多的细节

- cc 老师在遇到不确定的细节时，会自以为是地以它的意思来写，并且会静默、不汇报

- 在动手前把所有细节讲解出来，与我们对齐

### 搭建 cc 自己提交任务的 pipeline

- 这样 AI 在任务初期可以有 smoke test 以及频繁的 debug 流程

### 尽量提出具体、确切的 goal

- 例如一个可以对着一个可验证的 ground truth 自我验证的任务

- 可以让它起一个 subagent 作为验证者，来评判是否达成目标，若未达成能不断重启

### 可以先用其他论文搜索工具/网站把相关文献检索好

- 多篇论文阅读的 context 是较长的，可以尝试将其用 subagent 实现，使上下文干净~

### 如果有可能，可以反复地检查代码、论文细节

- 即使是简单的重复prompt、重复检查，push 它从各种角度检查也能发现新东西

- 在 prompt 中可以表达 “不怕困难” 这样的意思，让它持续探索、不退化

### 养成 git diff 的情况，有不明白的地方要及时问它

- 它的总结总是很漂亮的，但是可能和实际改动对不上，特别是一些小细节

- 养成看 `git diff` 的习惯，阅读真实代码，以真实 diff 为准

- 可以开多个 branch 来向它提问某个你不理解的、关键的 section

- 及时 commit~

### 对 wandb 中的数据，要先人看

- 实验中 wandb 所体现的现象，可以人先指出 xx指标出现了xx

- 它直接读 wandb 保存的数据可能需要长时间的搜索，并且可能污染上下文

- 对于实验的log（几千行），可以新开 branch 给它，它会细致地查找、定位

## 打通自动化科研需要

1. 自动放实验、停实验、调整配置（用于监控昂贵的训练过程）

2. 完成之后会有消息提示（在cc中可以配置hook）

### 一些其他的小技巧~

- 学会使用每个项目下的`CLAUDE.md`

- 它完成后提示，可以让它自己配置一个 hook

- 向它解释一些禁止行为的原因

[← 上一篇：有哪些能申请的奖学金？](scholarships.md) · [返回目录](README.md)

来源：[飞书原文](https://lamda3-nju.feishu.cn/wiki/Uf9fwnQFxiJS1akJZkPc87gFniq?from=from_copylink)
