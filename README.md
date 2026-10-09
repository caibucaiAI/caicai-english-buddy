# 英语口语与视频学习

一个 Codex Skill，两种学习模式：英语口语练习，以及结合录音转录的英文视频学习。记录保存到你自己的 Obsidian。

## 使用

```text
使用 $obsidian-speaking-practice
```

启动时先问：“你这次想要进入什么模式？英语口语练习，还是英语视频学习？”已明确选择模式时直接开始。

- **英语口语练习**：自然对话、轻量纠错、完整逐字稿、中文记录、单词本与周复盘。
- **英语视频学习**：边看边发术语问题，结合录音上下文用中文解释；结束时可做简短回考，也可以直接归档。保存视频笔记、问答记录、原始录音逐字稿、独立单词本和周复盘材料。

两种模式在语言学习目录下并列，各有自己的索引、单词本、对话记录、待办清单和周复盘。周复盘材料积累不等于已完成回考；学习反馈依据实际回答，不提前判定掌握。

## 安装

```bash
git clone https://github.com/caibucaiAI/obsidian-speaking-practice.git ~/.codex/skills/obsidian-speaking-practice
```

首次使用时提供你的 Obsidian Vault 和目标学习目录。优先沿用现有结构。已安装者应先保留本地定制，再更新文件。

## 两种模式的入口

- **英语口语练习**：实时开口练习使用 Codex 的 **Live 模式**。
- **英语视频学习**：边看边读取录音上下文使用 ChatGPT 的 **Meetings 插件**，并关联当前录音 Page。

截至 2026-10-09，[官方 Meetings 说明](https://help.openai.com/en/articles/20001546-the-meetings-plugin-in-chatgpt)列出的支持范围是 **macOS 桌面应用中的 Pro 和 Business 方案**；Enterprise 仅有有限 alpha。Meetings 与旧版 ChatGPT Record 是不同功能，不能套用旧 Record 的会员范围。

如果找不到入口或不能使用，Skill 会先区分账号方案、平台、插件设置、音频权限、转录访问和 OB 文件访问，再说明原因与下一步。不是所有问题都由会员造成，也不会保证购买 Pro 后一定解决。产品范围可能变化，以最新官方说明和实际账号入口为准。暂时没有 Meetings 时，可以提供字幕或原句继续学习；没有 Live 时，可以先文字练习。

## 视频学习需要什么

在支持录音转录读取的聊天中，关联当前录音 Page 或会话。Skill 不会自行启动录音，也不保证系统声音能被录到；先用短片段试一次。若转录工具不可用，可粘贴原句或字幕继续解释。写入 OB 还需要当前环境能访问本地 Vault。

完整逐字稿保留当前录音工具实际提供的原文、重复和识别误差，不等于完整原视频字幕，也不包含未被录音收录的聊天回复。初步或不完整转录会标明范围。

## 内容范围

仓库只包含可复用 Skill，不包含个人 Vault 路径、录音、对话或学习笔记。Skill 不要求 API Key。技术核对可能使用网页资料；本地归档不会自动发布学习记录。人生记录和阅读划线为按需使用的可选上下文。

## 文件

```text
SKILL.md
agents/openai.yaml
references/record-schema.md
references/video-learning.md
```
