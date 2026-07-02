---
title: 隐私政策
---

# 隐私政策

**最后更新日期**：2026年7月2日

DoodleLanguage（以下简称"本应用"）尊重并保护所有使用者的个人隐私。本隐私政策旨在向你说明我们如何收集、使用、存储及保护你的信息。

## 1. 信息收集

### 1.1 你主动提供的信息

- **涂鸦内容**：你在本应用中绘制的涂鸦图像会被发送到 AI 服务进行识别，以返回对应的外语单词。涂鸦内容仅在识别过程中临时传输，不会被存储或用于其他目的。
- **录音内容**：你在本应用中录制的语音数据仅保存在你的设备本地，不会被上传到任何服务器。

### 1.2 自动收集的信息

本应用使用 Firebase Crashlytics 和 Firebase Performance 来改善应用质量和性能：

- **崩溃数据**：当应用发生崩溃时，Firebase Crashlytics 会收集崩溃堆栈信息（包括设备型号、iOS 版本、应用版本），用于帮助我们排查和修复问题。这些数据不包含个人身份信息。
- **性能数据**：Firebase Performance 会收集识别（recognize）、发音（speak）、录音（record）和播放（playback）等操作的耗时和成功率统计。这些数据仅用于优化应用性能，不包含个人身份信息。

### 1.3 不会收集的信息

- 本应用不收集你的姓名、邮箱、手机号等个人身份信息。
- 本应用不需要创建账号，不需要登录。
- 本应用不收集位置信息。

## 2. 信息使用

所收集的信息仅用于以下目的：

- **涂鸦识别**：将涂鸦发送至 AI 服务（OpenRouter API）进行识别，返回识别结果
- **发音朗读**：使用系统 TTS（AVSpeechSynthesizer）朗读识别出的单词，朗读内容不传输至外部服务
- **崩溃分析**：通过 Firebase Crashlytics 分析崩溃原因
- **性能优化**：通过 Firebase Performance 分析核心操作（识别、发音、录音、播放）的成功率和耗时

## 3. 第三方服务

本应用集成了以下第三方服务：

| 服务 | 用途 | 传输的数据 | 隐私政策 |
|------|------|-----------|---------|
| OpenRouter API | AI 涂鸦识别 | 涂鸦截图 | [OpenRouter Privacy](https://openrouter.ai/privacy) |
| Firebase Crashlytics | 崩溃报告 | 崩溃堆栈、设备信息 | [Google Privacy](https://policies.google.com/privacy) |
| Firebase Performance | 性能监控 | 操作耗时、成功/失败统计 | [Google Privacy](https://policies.google.com/privacy) |
| 系统 TTS（AVSpeechSynthesizer） | 语音发音 | 文本内容 | 系统内置，不传输至外部 |

## 4. 数据存储

- **涂鸦数据**：保存在设备本地 `Documents` 目录，可通过 iCloud 同步至你的其他设备
- **录音数据**：保存在设备本地 `Library/Application Support` 目录，不参与 iCloud 同步
- **设置偏好**：使用 `UserDefaults` 保存，仅存储在设备本地
- **配额信息**：保存在设备本地文件

## 5. 儿童隐私

本应用主要面向各年龄段的语言学习者。我们不会故意收集 13 岁以下儿童的个人信息。如果家长发现儿童未经同意提交了个人信息，请联系我们删除。

## 6. 隐私政策变更

如果本隐私政策发生变更，我们会在应用更新时通过更新本文档的方式通知你。变更后的政策将在发布之日起生效。

## 7. 联系我们

如果你对本隐私政策有任何疑问，请通过以下方式联系我们：

**邮箱**：sidney.wang@foxmail.com
