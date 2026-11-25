# 技能选用与恢复

构思时从[故事方法](story-method.md)选一个与眼下难题有关的问题。需做首次阅读体验审读时查[工作流](workflow.md)，需清稿时查[文风审校](prose-style.md)和作品的 `bible/style.md`。这三个入口可直接在仓库中阅读。检索、运行脚本、接入外部账户等能力另由任务环境提供，阅读一份方法说明不会取得这些权限。

## 本次配置与证据

| 对象 | 评估与取舍 | 本任务可用性及验证范围 |
| --- | --- | --- |
| 云端已有的 `develop-screen-story` | 已读技能正文和开发工作页。保留核心画面、让反方有可理解的理由、从转折倒查信息取得过程。小说的感知、叙述距离与内心时间由作品文风决定。分场、时长估算等留给有明确委托的改编。 | 云端技能目录实际列出该名，通过 `skills.read` 取得正文。读取时的云包标识是 `skill://user/6afd5742638c81918e9eaf386aebbd8b/develop-screen-story`，未提供可固定的修订号或公开分发许可。仅就地参考。此任务未运行影视产出流程。 |
| 公开候选 `story-planning`、`reader-sim` | 已查固定快照的技能入口、头脑风暴、方向选择及相关依赖。选用的问题列在下文。 | 已通过终端 Git 下载到仓库外供核读。当前云端技能清单无这两项，未安装，未作原生技能调用测试。 |
| 仓库的中文小说审校方法 | 已写入文风文档和作品文风模板，使用时只读本次文本、保护项与相关文风。单独引入 `Humanizer-zh` 或再包装一份 `novel-prose-editor` 会增加重复入口，当前无需安装。 | 通过 Markdown 手工应用。此仓库未创建 `.agents/skills/`。本次执行环境的技能枚举为空，云端已有技能另见上栏。 |

当前工具清单可读取云端技能，终端已成功从 GitHub 取得下述快照。本次未获专用网页检索接口，网页搜索能力未验证。外部下载依赖具体目的地和当前网络策略。以上核读无须更改凭据、外部账户或共享环境设置。

## 公开快照与取舍

核读对象为 `haowjy/creative-writing-skills` 的提交 `8d39b73661f4413984eef52b1d816e3788c979d9`。其根许可证为 Apache License 2.0。本仓库仅用自己的文字描述适用做法，无第三方技能副本和脚本依赖。复评请比对具体提交与许可，再决定是否引入变更。[源码快照](https://github.com/haowjy/creative-writing-skills/tree/8d39b73661f4413984eef52b1d816e3788c979d9) · [许可](https://github.com/haowjy/creative-writing-skills/blob/8d39b73661f4413984eef52b1d816e3788c979d9/LICENSE)

- **立项与发散。** 原始想法进作品简报。能导致不同故事后果的备选应说明得失，并给出符合本书意图的推荐。涉及核心方向的工作假设记入决定记录，再据用户已授权的范围向前写。上游另设头脑风暴档案、来源标签及分主题资源；这里用少量栏目区分用户决定、候选与暂定，仅在当前难题需要时查单项资源。无需逐句加标签、逐章重新确认或运行上游的 `project-setup` 建立另一套 `kb/`。[策划入口](https://github.com/haowjy/creative-writing-skills/blob/8d39b73661f4413984eef52b1d816e3788c979d9/skills/story-planning/SKILL.md) · [发散资源](https://github.com/haowjy/creative-writing-skills/blob/8d39b73661f4413984eef52b1d816e3788c979d9/skills/story-planning/resources/brainstorming.md)
- **首次阅读体验。** 先给审读者目标读者、阅读截止点、可见的前文，让它在读到某一段时记录一次期待、误解或改判及文字依据。报告写明这次模拟读者的前提与已知信息。上游要求连读 `writing-principles`；本项目用工作流中的审读说明即可，避免把无关偏好带进中文小说。该快照偏向回避英文 em dash，作品中的标点取决于声音和语境。[审读入口](https://github.com/haowjy/creative-writing-skills/blob/8d39b73661f4413984eef52b1d816e3788c979d9/skills/reader-sim/SKILL.md) · [关联写作原则](https://github.com/haowjy/creative-writing-skills/blob/8d39b73661f4413984eef52b1d816e3788c979d9/skills/writing-principles/SKILL.md)
- **中文审校。** 源码核读发现，上游统计脚本按拉丁字母词形取词，以英文句末标点后的空格切句，并识别半角双引号。中文对白和连写句子会漏计。该脚本依赖 Python 标准库，本次仅核读源码，中文验收直接对照原文的语义和阅读效果。[统计脚本](https://github.com/haowjy/creative-writing-skills/blob/8d39b73661f4413984eef52b1d816e3788c979d9/skills/story-review/resources/prose-critique/analyze.py)

## 文档审校走查

本次在当前任务中显式读取文风文档，手工对照其中三段原创教学材料。说明文删去重复的施事表述后，签字与归档仍由同一人依次完成。信封一段只删重复表达“拿不准”的末句，人物的否认、自辩和对弟弟态度的不确定均可从修订稿读出。等电话的一段保留三个“等”和两个称呼，迟疑一直延续到电话中断。三个检查点均通过；这是对该文档的手工走查，尚无新会话触发测试或真实读者反馈。[教学原文与修改对照](prose-style.md#原创教学示例)

## 在后续任务中恢复

从包含上述文档的工作区、分支或提交进入仓库，从根指令定位所需方法。没有远程版本的工作区修改仅保存在该工作区，本地提交也须在后续检出的版本中才可读取。进入新会话后，以该会话技能目录为准；缺少云包或网络不可用时，照常按文档推进。

若后续确需提供单独的原生技能，可在有相应授权的仓库版本中准备 `.agents/skills/<skill-name>/SKILL.md`，在目标任务实际核对技能清单，再用一项代表性任务测试触发、输入范围与输出。分别记录文件、发现和运行结果。账户技能、共享环境配置和环境发布由各自设置管理；此次仅评估与准备仓库内方法，跨会话原生发现与恢复尚未实测。[Codex 技能说明](https://developers.openai.com/codex/skills/)
