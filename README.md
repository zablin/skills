<p align="center">
  <img src="assets/banner.svg" alt="zablin / skills — 把理解变成可复用的方法" width="100%" />
</p>

<p align="center">
  <strong>学习 · 阅读 · 研究</strong><br />
  我的个人 AI 技能集，把反复打磨的方法整理成可以持续使用的 Skill。
</p>

<p align="center">
  <a href="#技能目录">技能目录</a> ·
  <a href="#如何使用">如何使用</a> ·
  <a href="#仓库结构">仓库结构</a> ·
  <a href="#参考与致谢">参考与致谢</a>
</p>

---

## 关于这个仓库

好的方法值得留下来。

这里存放我制作和持续改进的 Skill：从读懂一篇论文，到理清一个知识的概念、关系与适用边界，让每次与 AI 协作都能复用此前积累的方法。

每个 Skill 都会说明三件事：**什么时候用、怎样做、怎样判断做得好。**

## 技能目录

每个技能独立维护，点击名称查看完整规则与配套文件。

| 技能 | 用来做什么 | 状态 |
| --- | --- | --- |
| [**zablin-Paper**](skills/zablin-paper/) | 讲清论文的研究问题、作者贡献、关键证据与结论边界，提炼可迁移的认知模型。 | 已收录 |
| [**zablin-GradualLearning**](skills/zablin-gradual-learning/) | 渐构学习：拆解知识、建立判别与联结模型、伴读文本，并用未见情境验证学习成果。 | 已收录 · v2.0.0 |
| [**zablin-security**](skills/zablin-security/) | 三问主线 · 六问验证：追踪产业稀缺性、价值传导与价值捕获，以公司证据检验利润、现金及反转条件。 | 已收录 |

## 如何使用

打开对应的主规则，查看适用场景与执行流程：

- [zablin-Paper](skills/zablin-paper/SKILL.md)：论文阅读与分析。
- [zablin-GradualLearning](skills/zablin-gradual-learning/SKILL.md)：知识拆解、伴读与学习验证。

- [zablin-security](skills/zablin-security/SKILL.md)：产业与公司商业判断，配套数据溯源规则。

参考材料、模板和评测用例均保留在同一技能目录中。

安装后的调用示例：

```text
用 zablin-Paper 解读这篇论文：<论文链接或文件>
重点说明作者解决了什么问题、证据支持到哪里，以及哪些方法值得迁移。

用 zablin-GradualLearning 帮我理解这个概念，
用正例、反例与未见情境检验我是否真正会用。

用 zablin-security 按三问主线、六问验证分析这家公司，
重点检查价值如何传导到公司、能否转化为利润与现金。
```

在 GitHub 点击 **Code → Download ZIP**，解压后将 `skills/` 下需要的完整技能文件夹放入 Codex 的技能目录 `~/.agents/skills/`。保留参考材料、模板和示例等子目录；已安装的技能无需重复安装。

## 仓库结构

当前目录结构：

```text
zablin-skills/
├── README.md
├── assets/banner.svg
└── skills/
    ├── zablin-paper/
    │   ├── SKILL.md
    │   ├── references/
    │   ├── templates/
    │   └── evals/
    ├── zablin-gradual-learning/
        ├── SKILL.md
        ├── README.md
        ├── references/
        ├── templates/
        ├── examples/
        └── evals/
    └── zablin-security/
        ├── SKILL.md
        ├── agents/openai.yaml
        └── references/data-provenance.md
```

## 维护方式

- **从真实任务出发**：先在实际使用中验证，再沉淀为 Skill。
- **把边界写清楚**：说明适用与不适用的任务，避免把一种方法套到所有问题上。
- **随使用持续改进**：根据反馈更新规则、示例与检查标准。
- **保留来源**：改编或引用他人内容时，在对应 Skill 中注明出处并遵守原许可。

## 参考与致谢

首页的信息组织参考了 [李继刚的 ljg-skills](https://github.com/lijigang/ljg-skills)：用简洁的说明和技能目录，让方法便于发现与使用。本仓库的 Skill 文件将单独维护。

---

<p align="center"><sub>由 <a href="https://github.com/zablin">zablin</a> 持续整理</sub></p>
