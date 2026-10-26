# Qonur · HCI 作品集研究分支

上游： https://github.com/fammad/Qonur_Robotic_Bear

本分支： https://github.com/KINGKAZMAX/hci-robot-qonur

原作者与团队：Fuad Mammadov、Jameel Hamzayev 及上游 README 列出的合作团队。许可证 Apache-2.0；保留上游历史、许可证和版权通知。

## 内容与当前状态

上游包含 Python 语音／对话控制、ESP32 固件、可打印结构和装配说明。机器人结合 AI 对话与人工动作编排，不宜描述成完全自主系统。

本轮完成 fork、中文研究说明、状态设计及作品集页面结构。没有运行实体机器人、没有儿童试验、没有康复疗效数据。本分支新增文字是对上游的分析与拟议迭代，不是原作作者的研究结论。

## 第一性原理：希望检验什么

当机器人回应存在延迟时，使用者能否分辨“正在倾听”“正在等待服务”“正在回应”“需要人工接管”？通过把内部状态变成可理解反馈，研究交互理解与期待管理。机器人只是研究载体，研究贡献来自问题、机制和可核查证据。

## 拟议迭代

1. 桌面控制台区分 Idle / Listening / Waiting / Speaking / Handoff / Error。
2. 每个状态显示开始时间、触发原因与操作者可执行动作。
3. 超时后提供取消和接管；先在无硬件的合成事件回放中验证流程，再连接设备。
4. 只记录研究需要的事件，不把音频或儿童身份放入公开作品集。
5. 把人工操控动作与模型生成回复分别标注，便于解释系统边界。

## 评估方案（尚未实施）

先做成年人参与的低风险界面理解测试：比较只有等待动画与明确状态说明的界面。任务为辨认当前状态、选择恢复动作、回忆系统是否正在录音。记录正确率、完成时间和访谈反馈；样本规模与分析方法在正式研究前确定。此类测试不能支持儿童长期心理或康复效果结论。

## 六页作品集结构

1. 问题：延迟与不确定性；注明原作者及本人的新增工作。
2. 系统：语音 → 对话服务 → 输出 → 动作；明确人工编排。
3. 机制：六状态转换及失败恢复。
4. 原型：桌面状态台和实体反馈的对应；概念图标 AI concept。
5. 评估：先展示方法；只有完成研究后才能填真实结果。
6. 反思：适用人群、延迟、隐私、硬件限制及下一步。

## English brief

This fork preserves the Qonur authorship and Apache-2.0 license. The proposed HCI contribution is a legible interaction-state interface for a conversational animatronic system. A desktop view would distinguish listening, waiting, speaking and human handoff. This branch currently adds research framing and a portfolio structure; hardware integration and user evaluation have not been performed. AI visuals communicate a proposed direction, not an implemented or clinically validated outcome.
