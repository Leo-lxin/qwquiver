# 使用指南 | User Guide

## 3D医疗影像与大语言模型综述策划工具
## Medical Review Planning Tool for 3D Imaging & LLMs

---

## 快速开始 | Quick Start

### 1. 运行工具 | Run the Tool

```bash
cd medical_review_planner
python review_generator.py
```

### 2. 查看输出 | View Output

工具会生成两类输出：

**控制台输出 (Console Output)**:
- 三个方向的摘要信息
- 综合对比分析
- 推荐方向建议

**JSON文件 (JSON File)**: `medical_review_outlines.json`
- 完整的综述大纲详情
- 结构化的文献分类
- 详细的研究启发

---

## 详细使用说明 | Detailed Instructions

### 输出文件结构 | Output File Structure

```
medical_review_outlines.json
├── metadata (元数据)
│   ├── generator (生成器信息)
│   ├── version (版本号)
│   ├── date (生成日期)
│   ├── reference_papers (参考文献)
│   └── focus (研究焦点)
│
├── outlines (三个综述大纲)
│   ├── outline_1: 从"看图"到"看片"
│   │   ├── title (中文标题)
│   │   ├── title_en (英文标题)
│   │   ├── core_narrative (核心叙事逻辑)
│   │   │   ├── why_transition (为什么转向4D)
│   │   │   └── pain_points_solved (解决的痛点)
│   │   ├── literature_classification (文献分类维度)
│   │   │   ├── dimension_1: 时空表征学习
│   │   │   ├── dimension_2: 时序建模架构
│   │   │   ├── dimension_3: 多模态对齐与融合
│   │   │   └── dimension_4: 临床应用场景
│   │   ├── bme_research_insights (BME研究启发)
│   │   │   ├── technical_priorities (技术重点)
│   │   │   ├── dataset_construction (数据集构建)
│   │   │   └── evaluation_metrics (评估指标)
│   │   └── outline_structure (大纲结构)
│   │
│   ├── outline_2: 时空推理与临床决策
│   │   └── ... (类似结构)
│   │
│   └── outline_3: 实时手术智能
│       └── ... (类似结构)
│
└── comprehensive_analysis (综合分析)
    ├── comparison (三个方向的对比)
    ├── common_challenges (共同挑战)
    ├── synergies (协同效应)
    └── recommendation (推荐方向)
```

---

## 三个方向详解 | Three Directions Explained

### 方向 1：从"看图"到"看片"

**最适合**: AI研究者、计算机视觉背景的研究生

**核心内容**:
- **时空表征学习**: Point Cloud序列编码、Voxel时空建模
- **架构演进**: 从静态编码器到动态编码器
- **技术迁移**: Video-LLM → Medical 4D LLM

**关键研究方向**:
1. 高效时空编码器设计
2. 医学领域的时序注意力机制
3. 实时性优化技术
4. 小样本/零样本学习
5. 可解释性与临床可信度

**推荐使用场景**:
- 想要全面了解4D医学LLM技术框架
- 从事深度学习架构设计
- 研究Video-LLM在医学领域的应用

---

### 方向 2：时空推理与临床决策

**最适合**: BME研究生、临床应用研究者

**核心内容**:
- **数据模态**: 手术视频、动态增强影像、心血管4D成像、胎儿4D超声
- **任务类型**: 时序分割、动态功能量化、事件检测、技能评估
- **技术路线**: 端到端4D Transformer、分离式时空建模、混合架构、知识增强

**关键研究方向**:
1. 因果时序建模
2. 不确定性量化
3. 多时间尺度融合
4. 联邦学习与隐私保护

**推荐使用场景**:
- 关注临床决策支持系统
- 研究因果推断和时序预测
- 需要平衡技术和临床应用

---

### 方向 3：实时手术智能

**最适合**: 手术机器人方向、系统工程背景

**核心内容**:
- **感知层**: 器械检测、解剖分割、阶段识别、异常检测
- **推理层**: 步骤预测、风险评估、操作建议、技能评估
- **交互层**: AR显示、语音交互、触觉反馈、远程协作
- **系统集成**: 4D重建、LLM推理、机器人控制、影像集成

**关键研究方向**:
1. 极低延迟推理 (<100ms)
2. 鲁棒性与可靠性
3. 手术知识融合
4. 多模态传感器融合
5. 人机协同机制

**推荐使用场景**:
- 从事手术机器人研究
- 关注实时系统工程实现
- 研究人机协同界面

---

## 如何选择方向 | How to Choose a Direction

### 根据研究背景选择

| 背景 | 推荐方向 | 理由 |
|------|---------|------|
| 深度学习/计算机视觉 | 方向1 | 侧重架构设计和表征学习 |
| 生物医学工程 | 方向2 | 平衡技术和临床应用 |
| 机器人/控制工程 | 方向3 | 聚焦系统集成和实时性 |
| 医学影像分析 | 方向1或2 | 可结合影像特点选择 |
| 临床医学 | 方向2或3 | 强调临床决策和应用 |

### 根据研究目标选择

**如果您想**:
- 📚 **撰写技术综述** → 方向1（最全面的技术框架）
- 🏥 **推动临床应用** → 方向2（强调决策支持价值）
- 🤖 **开发实际系统** → 方向3（关注工程实现）
- 🌟 **开创新方向** → 整合三个方向

---

## 使用生成的大纲 | Using the Generated Outlines

### Step 1: 阅读综合分析

打开 `medical_review_outlines.json`，先查看 `comprehensive_analysis` 部分：

```json
{
  "comprehensive_analysis": {
    "comparison": { ... },
    "common_challenges": [ ... ],
    "synergies": [ ... ],
    "recommendation": { ... }
  }
}
```

**重点关注**:
- `comparison`: 三个方向的范围、技术深度、目标读者对比
- `common_challenges`: 所有方向面临的共同挑战
- `recommendation`: 针对不同情况的推荐

### Step 2: 选择适合的方向

根据您的背景和目标，选择一个或多个方向。

### Step 3: 深入研究选定方向

对于选定的方向，详细阅读：

1. **核心叙事逻辑** (`core_narrative`):
   - 理解"为什么要从3D转向4D"
   - 明确"解决了什么痛点"

2. **文献分类维度** (`literature_classification`):
   - 了解如何组织现有文献
   - 识别各个子领域和关键论文

3. **BME研究启发** (`bme_research_insights`):
   - 识别值得深入的技术细节
   - 规划数据集构建和评估方法

4. **大纲结构** (`outline_structure`):
   - 作为综述的章节框架
   - 可根据需要调整和扩展

### Step 4: 文献调研

根据大纲中的分类维度，开始系统的文献调研：

**推荐策略**:
1. 从三篇参考综述开始，提取相关的4D/动态内容
2. 使用大纲中的关键词在Google Scholar搜索
3. 关注大纲中提到的关键论文类型
4. 按照分类维度整理文献

### Step 5: 细化大纲

结合文献调研结果，细化和调整大纲：

- 添加具体的文献引用
- 扩展技术细节
- 补充最新进展
- 调整章节结构

---

## 高级用法 | Advanced Usage

### 整合多个方向

您可以将三个方向整合为一个更全面的综述：

**建议结构**:
```
第一部分: 基础技术（方向1）
├── 时空表征学习
├── 架构演进
└── 多模态融合

第二部分: 临床应用（方向2）
├── 数据模态分析
├── 任务类型分类
└── 推理机制

第三部分: 系统实现（方向3）
├── 感知技术
├── 交互技术
└── 系统集成

第四部分: 挑战与展望
├── 共同挑战
├── 未来方向
└── 研究路线图
```

### 自定义输出

如需自定义输出，可修改 `review_generator.py`:

**修改标题**:
```python
outline = {
    "title": "您的自定义标题",
    "title_en": "Your Custom Title",
    ...
}
```

**添加新的分类维度**:
```python
"literature_classification": {
    "dimension_5_custom": {
        "name": "您的自定义维度",
        "subcategories": [ ... ]
    }
}
```

**扩展研究启发**:
```python
"bme_research_insights": {
    "technical_priorities": [
        {
            "area": "新的研究领域",
            "details": "详细描述",
            "research_value": "研究价值"
        }
    ]
}
```

---

## 常见问题 | FAQ

### Q1: 生成的大纲可以直接用于论文吗？

**A**: 大纲提供了综述的框架和方向，但需要：
- 补充具体的文献引用
- 扩展技术细节
- 添加批判性分析
- 调整以符合目标期刊的要求

### Q2: 如何处理三篇参考综述的内容？

**A**: 建议的处理方式：
1. 提取其中关于3D医学影像的静态分析方法
2. 分析其局限性（无法处理时序信息）
3. 以此为基础，论证向4D方向发展的必要性
4. 借鉴其分类框架，扩展到时序维度

### Q3: 我应该专注一个方向还是整合多个方向？

**A**: 取决于您的目标：
- **硕士论文**: 建议专注一个方向，深入研究
- **博士论文**: 可整合2-3个方向，形成完整体系
- **期刊综述**: 整合三个方向，覆盖整个领域
- **会议综述**: 专注一个方向，突出创新点

### Q4: 生成的JSON文件太大，如何使用？

**A**: 推荐工具：
- **查看**: 使用任何文本编辑器或JSON查看器
- **分析**: 使用Python脚本提取关键信息
- **转换**: 可以编写脚本转换为Markdown或Word

示例Python脚本:
```python
import json

with open('medical_review_outlines.json', 'r', encoding='utf-8') as f:
    data = json.load(f)

# 提取第一个方向的标题
title = data['outlines']['outline_1']['title']
print(f"标题: {title}")

# 提取技术重点
priorities = data['outlines']['outline_1']['bme_research_insights']['technical_priorities']
for p in priorities:
    print(f"- {p['area']}: {p['research_value']}")
```

---

## 示例工作流 | Example Workflow

### 场景：BME研究生撰写硕士论文综述

**目标**: 撰写关于动态心脏影像与LLM的综述

**步骤**:

1. **运行工具** → 生成三个方向的大纲

2. **选择方向** → 选择方向2（时空推理与临床决策）
   - 原因：平衡技术和临床应用，适合BME背景

3. **提取相关内容** → 从方向2中提取心血管4D成像部分
   ```json
   {
     "type": "心血管4D成像",
     "examples": ["心脏电影MRI", "4D心脏CT", "实时3D超声心动图"],
     "challenges": ["心脏运动伪影", "呼吸运动补偿", "高时间分辨率"]
   }
   ```

4. **文献调研** → 按照分类维度搜索文献
   - 数据模态：心血管4D成像技术
   - 任务类型：动态功能量化（射血分数、心肌应变）
   - 技术路线：时空Transformer、知识增强方法

5. **细化大纲** → 形成最终综述大纲
   ```
   1. 引言：心脏疾病诊断中的动态评估需求
   2. 心血管4D成像技术概览
   3. 时空表征学习方法
   4. 临床任务：功能量化、异常检测、预后预测
   5. 挑战：数据标注、实时性、可解释性
   6. 未来方向：多模态融合、因果推断
   7. 结论
   ```

6. **撰写论文** → 在大纲基础上撰写综述内容

---

## 联系与支持 | Contact & Support

如有问题或建议，欢迎：
- 提交GitHub Issue
- 发送邮件至项目维护者
- 参与讨论和改进

---

**祝您研究顺利！Good luck with your research!** 🎓✨
