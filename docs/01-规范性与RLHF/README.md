# 线 01｜规范性与 RLHF

问题清单见 `../../AGENDA.md` 线 01。这里是工作区。

## 这条线要打赢的一仗

先把「规范性」这个词从含混里救出来。至少三层，混着谈就必然滑坡：

| 层 | 内容 | 谁在谈 |
|---|---|---|
| 规则的规范性 | 这一步走法对不对 | 维特根斯坦 §§143–242 |
| 语义的规范性 | 这个词该不该这么用 | 维特根斯坦、克里普克 |
| 评价的规范性 | 这个回答好不好 | RLHF |

**初步怀疑（待打）**：RLHF 训的几乎全在第三层，而维特根斯坦谈的主要是前两层。如果这个错位成立，「RLHF 是不是把模型接进了生活形式」这个问题就要重写——它可能连维特根斯坦关心的那种规范性都没碰到，只是给偏好排了个序。

## 进度

- 2026-08-24：第 1 步「概念清理」已做，见 `01-概念清理-三层规范性.md`。**结论是三层框架要改用法**——前两层在 §§143–242 里是同一论证的两个实例，且「RLHF 只训第三层」按内容立会被证伪，要改成按形式立。新判断 F–J 已进台账。
- 2026-08-24：第 2 步的前半「§208 之争」已打，见 `02-§208之争.md`。**天敌性部分解除，§208 由天敌转为尺子。** 三条发现：在场提供的是「接纳变体」这个选项（§143）；争议要三分而非二分，RLHF 生产的是无争议的外观；对错被采集为二值元数据但没有喂进奖励模型。新判断 K／L／M 进台账，H 改判，G 精确化。
- 克里普克之争仍未打，且已判明它决定的是赌注不是胜负。**手上无 Kripke／Baker & Hacker／McDowell 原文。**
- 下一步两个候选：(a) 查中间化预测（台账 K，第一个可证伪命题）；(b) 打 Anthropic 宪法路线一侧。

## 阅读清单

### 一手（必须回原文）
- Wittgenstein, *Philosophical Investigations*，§§143–242（规则遵守），重点 §201、§202、§§240–242。中译建议对照陈嘉映译本与 Hacker/Schulte 英译第四版。
- Wittgenstein, *Remarks on the Foundations of Mathematics*，第六部分。
- Wittgenstein, *On Certainty*（涉及「河床」与实践的无根基性，与规范性的最终来源直接相关）。

### 二手：克里普克之争（这条线的主战场）
- Kripke, *Wittgenstein on Rules and Private Language* (1982) — 怀疑论悖论与共同体式的「怀疑论解答」。
- Baker & Hacker, *Scepticism, Rules and Language* (1984) — 对克里普克的正面反驳。
- McDowell, "Wittgenstein on Following a Rule" (1984) — 第三条路。
- McGinn, *Wittgenstein on Meaning* (1984)。
- Brandom, *Making It Explicit* (1994) — 把规范性做成系统的推论主义版本。

> 关键判别问题：「共同体是对错的唯一来源」到底是维特根斯坦的观点，还是**克里普克的**维特根斯坦的观点？这个问题不解决，后面对 RLHF 的所有推论都悬空。

### AI 侧
- Christiano et al. (2017), *Deep Reinforcement Learning from Human Preferences*。
- Ouyang et al. (2022), *Training language models to follow instructions with human feedback*（InstructGPT）。
- Bai et al. (2022), *Constitutional AI: Harmlessness from AI Feedback* — 判定权从人转给模型的那一刻。
- Casper et al. (2023), *Open Problems and Fundamental Limitations of RLHF* — 系统性列出 RLHF 的结构缺陷，是这条线最有用的一篇。
- Anthropic, *Collective Constitutional AI*（2023，与 Polis 合作的公众参与制宪实验）— 与「规范性的定义权」直接相关。
- Krakovna et al. (2020), specification gaming 案例集 — 规则遵守悖论的工程版。

### 劳动与权力侧
- Gray & Suri, *Ghost Work* (2019)。
- Perrigo, TIME (2023)，OpenAI 与肯尼亚标注工的报道 `[待核验]`。

> 这一支不是花边。「外包」这个环节直接冲击规范性的合法性：判定者不承担判定的后果，这在维特根斯坦的实践图景里是个畸形结构。

## 工作顺序（建议）

1. 先做**概念清理**：三层规范性的区分，写成一页，作为后面所有讨论的地基。
2. 再打**克里普克之争**：读 §§201–202 原文 + 克里普克 + 至少一个反对者，形成自己的判定。
3. 然后才谈 **RLHF 的哲学身份**，把「一次性 / 离线 / 外包 / 不担后果」四个变量分别对照。
4. 最后是**定义权与分布式系统**那一问——它依赖前三步的结论，先做会空转。
