# 线 04｜图灵的真面目

问题清单见 `../../AGENDA.md` 线 04。

## 要拆的假对立

流行叙事：图灵 = 符号形式主义，维特根斯坦 = 具身实践派，两人 1939 年吵了一架，赌局延续至今。

反证：
1. 图灵 1948 年那份未发表报告 *Intelligent Machinery* 里，直接讨论了给机器装上肢体与感官、以及「未组织的机器」如何被训练成组织化的机器。
2. 图灵 1950 年论文第 7 节的「儿童机器」：不要试图直接造成人的心智，造一个儿童的心智，然后**教育**它，用奖惩去训练。
3. Juliet Floyd 等人的研究一直在论证，图灵与维特根斯坦在「数学是人的实践」这件事上的距离比叙事要近。

如果这些站得住，那 LeCun 的世界模型路线在血统上是**图灵的**：先学世界，再学语言，靠与环境的交互而非靠形式公理。反自回归不等于反图灵——自回归 LLM 才是那个更接近「形式系统足够」的赌注。

## 「实践的最小单位」这句话怎么理解

这是本项目的一个待验证核心命题：

- 维特根斯坦那里，实践的最小单位是**共同体的习俗**——一个规则之所以有对错，是因为有一群人在一种生活里持续地这样用它。单个人、单次行为，构不成实践。
- 图灵那里，实践的最小单位是**个体与环境的训练回路**——一台机器通过奖惩与试错，可以自己把行为调对。共同体是可选的，回路是必需的。

于是分歧不在「意义要不要实践」，而在**一个孤立的学习者能不能自己产生规范性**。维特根斯坦说不能（这正是私人语言论证），图灵默认能。今天所有关于「智能体自我改进」「自博弈」「无人类反馈的对齐」的争论，都是这一分歧的直系后代。

→ 这句话如果成立，它会同时改写线 01（RLHF 到底提供了什么）与线 03（判据到底判定什么）。所以线 04 虽然排在最后，可能是收口的那条。

## 阅读清单

- Turing (1948), *Intelligent Machinery*（收于 Copeland 编 *The Essential Turing*）。
- Turing (1950), *Computing Machinery and Intelligence*，第 7 节。
- Diamond (ed.), *Wittgenstein's Lectures on the Foundations of Mathematics, Cambridge 1939* — 图灵在场的那些课，逐字记录。
- Floyd & Bokulich (eds.), *Philosophical Explorations of the Legacy of Alan Turing* (2017) `[待核验]`；Floyd, "Turing on 'Common Sense': Cambridge Resonances" `[待核验]`。
- Hodges, *Alan Turing: The Enigma*。
- Sterrett, "Turing's Two Tests for Intelligence" `[待核验]`。
