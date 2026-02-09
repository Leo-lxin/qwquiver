# 3D医疗影像与大语言模型综述策划工具

## 概述

本仓库新增了一个专门的工具，用于帮助生物医学工程（BME）研究生和研究人员策划**动态3D医疗影像与大语言模型（LLM）**领域的综述论文。

## 工具位置

📁 `medical_review_planner/`

## 核心功能

基于三篇重要的医学LLM综述文献，自动生成**三个独特的综述大纲方向**：

### 方向 1: 从"看图"到"看片"
医学3D视频大模型的现状与未来
- 关注时空表征学习和架构演进
- 适合AI研究者和计算机视觉背景

### 方向 2: 时空推理与临床决策
医学4D数据的大模型范式
- 强调因果推断和临床决策支持
- 适合BME研究生和临床应用研究者

### 方向 3: 实时手术智能
基于4D视觉的大模型导航系统
- 聚焦系统集成和实时性能
- 适合手术机器人和系统工程方向

## 快速开始

```bash
cd medical_review_planner
python review_generator.py
```

## 输出内容

- ✅ 三个完整的综述大纲（中英文标题）
- ✅ 核心叙事逻辑（为什么从3D到4D，解决什么痛点）
- ✅ 文献分类维度建议
- ✅ BME研究生的研究启发
- ✅ 综合对比分析
- ✅ JSON格式的详细输出

## 文档

- 📖 [README.md](medical_review_planner/README.md) - 工具介绍
- 📘 [USER_GUIDE.md](medical_review_planner/USER_GUIDE.md) - 详细使用指南
- 📄 [medical_review_outlines.json](medical_review_planner/medical_review_outlines.json) - 示例输出

## 适用人群

- 🎓 生物医学工程研究生
- 👨‍🔬 医学影像AI研究者
- 🏥 临床AI应用开发者
- 🤖 手术机器人研究人员
- 📝 需要撰写综述论文的学者

## 特色亮点

### 从Static到Dynamic的技术跨越
- Point-Cloud/Voxel架构如何演进到处理时序3D视频
- Video-LLM的时空注意力机制在医学领域的应用
- 长序列帧的内存优化策略

### BME视角下的数据挑战
- 多模态对齐（视频-文本、影像-生理信号）
- 实时性要求（<100ms延迟）
- 隐私保护与联邦学习

### 应用场景的升维
- 从"辅助诊断（静态）"到"术中引导（动态）"
- 动态生理功能评估（心脏功能、血流动力学）
- 虚拟手术训练与技能评估

## 参考文献

本工具基于以下三篇重要综述：
1. Vision-language foundation model for 3D medical imaging
2. A Survey of Large Language Models in Medicine: Progress, Application, and Challenge
3. Large Language Models for Medicine: A Survey

## 贡献

欢迎提交Issue和Pull Request改进本工具！

---

**详细使用说明请查看**: [medical_review_planner/USER_GUIDE.md](medical_review_planner/USER_GUIDE.md)
