# README: InternLM2 - 全链路开源大型语言模型

## 概述

InternLM2 是一个最先进的开源大型语言模型，旨在推动通用人工智能的发展。本 README 提供了 InternLM2 模型的概述、主要特性、训练方法和评估结果。InternLM2 提供多种配置，以满足不同的研究和应用需求，包括 1.8B、7B 和 20B 参数的模型。

## 主要亮点

- **大上下文窗口**：支持高达 20,000 个 token 的上下文窗口，使其能够有效处理长文本建模。
- **增强功能**：在推理、数学推理和代码任务中表现出色。
- **全面的开源生态系统**：提供全链路开源开放体系，包括数据、预训练、微调、部署、评测和应用。

## 模型开源历程

- **InternLM2-1.8B**  
  [Hugging Face](https://huggingface.co/internlm/internlm2-1_8b)  
  [ModelScope](https://www.modelscope.cn/models/Shanghai_AI_Laboratory/internlm2-1_8b/summary)  
  [OpenXLab](https://openxlab.org.cn/models/detail/OpenLMLab/internlm2-base-1.8b)  
  发布日期：2024-01-31

- **InternLM2-Chat-1.8B-SFT**  
  [Hugging Face](https://huggingface.co/internlm/internlm2-chat-1_8b-sft)  
  [ModelScope](https://www.modelscope.cn/models/Shanghai_AI_Laboratory/internlm2-chat-1_8b-sft/summary)  
  [OpenXLab](https://openxlab.org.cn/models/detail/OpenLMLab/internlm2-chat-1.8b-sft)  
  发布日期：2024-01-31

- **InternLM2-Chat-1.8B**  
  [Hugging Face](https://huggingface.co/internlm/internlm2-chat-1_8b)  
  [ModelScope](https://www.modelscope.cn/models/Shanghai_AI_Laboratory/internlm2-chat-1_8b/summary)  
  [OpenXLab](https://openxlab.org.cn/models/detail/OpenLMLab/internlm2-chat-1.8b)  
  发布日期：2024-02-19

- **InternLM2-Base-7B**  
  [Hugging Face](https://huggingface.co/internlm/internlm2-base-7b)  
  [ModelScope](https://modelscope.cn/models/Shanghai_AI_Laboratory/internlm2-base-7b/summary)  
  [OpenXLab](https://openxlab.org.cn/models/detail/OpenLMLab/internlm2-base-7b)  
  发布日期：2024-01-17

- **InternLM2-7B**  
  [Hugging Face](https://huggingface.co/internlm/internlm2-7b)  
  [ModelScope](https://modelscope.cn/models/Shanghai_AI_Laboratory/internlm2-7b/summary)  
  [OpenXLab](https://openxlab.org.cn/models/detail/OpenLMLab/internlm2-7b)  
  发布日期：2024-01-17

- **InternLM2-Chat-7B-SFT**  
  [Hugging Face](https://huggingface.co/internlm/internlm2-chat-7b-sft)  
  [ModelScope](https://modelscope.cn/models/Shanghai_AI_Laboratory/internlm2-chat-7b-sft/summary)  
  [OpenXLab](https://openxlab.org.cn/models/detail/OpenLMLab/internlm2-chat-7b-sft)  
  发布日期：2024-01-17

- **InternLM2-Chat-7B**  
  [Hugging Face](https://huggingface.co/internlm/internlm2-chat-7b)  
  [ModelScope](https://modelscope.cn/models/Shanghai_AI_Laboratory/internlm2-chat-7b/summary)  
  [OpenXLab](https://openxlab.org.cn/models/detail/OpenLMLab/internlm2-chat-7b)  
  发布日期：2024-01-17

- **InternLM2-Base-20B**  
  [Hugging Face](https://huggingface.co/internlm/internlm2-base-20b)  
  [ModelScope](https://modelscope.cn/models/Shanghai_AI_Laboratory/internlm2-base-20b/summary)  
  [OpenXLab](https://openxlab.org.cn/models/detail/OpenLMLab/internlm2-base-20b)  
  发布日期：2024-01-17

- **InternLM2-20B**  
  [Hugging Face](https://huggingface.co/internlm/internlm2-20b)  
  [ModelScope](https://modelscope.cn/models/Shanghai_AI_Laboratory/internlm2-20b/summary)  
  [OpenXLab](https://openxlab.org.cn/models/detail/OpenLMLab/internlm2-20b)  
  发布日期：2024-01-17

- **InternLM2-Chat-20B-SFT**  
  [Hugging Face](https://huggingface.co/internlm/internlm2-chat-20b-sft)  
  [ModelScope](https://modelscope.cn/models/Shanghai_AI_Laboratory/internlm2-chat-20b-sft/summary)  
  [OpenXLab](https://openxlab.org.cn/models/detail/OpenLMLab/internlm2-chat-20b-sft)  
  发布日期：2024-01-17

- **InternLM2-Chat-20B**  
  [Hugging Face](https://huggingface.co/internlm/internlm2-chat-20b)  
  [ModelScope](https://modelscope.cn/models/Shanghai_AI_Laboratory/internlm2-chat-20b/summary)  
  [OpenXLab](https://openxlab.org.cn/models/detail/OpenLMLab/internlm2-chat-20b)  
  发布日期：2024-01-17

## 技术细节

### 预训练数据

InternLM2 使用了海量的多样化数据进行预训练，包括文本、代码和长文本数据。这些数据涵盖了多个领域，如新闻、科技、文学和社交媒体。通过多样化的数据源，模型能够从多个角度学习语言的规律和结构。

### 预训练设置

- **架构**：基于 LLaMA 的设计原则，使用 RMSNorm 作为归一化方法和 SwiGLU 作为激活函数。
- **训练方法**：采用分布式训练，使用数百个 GPU 并行训练。
- **超参数调整**：经过多次实验和调优，找到了一组适合的超参数设置，包括学习率、批处理大小和训练轮数。

### 长文本能力训练

InternLM2 设计了具有 20,000 token 上下文窗口的能力，使其在长文本任务中表现出色。在“大海捞针”实验中，使用 20,000 token 上下文几乎完美地识别出所有目标。

### 对齐策略

通过对齐损失函数，确保模型在生成文本时能够保持与原始文本的一致性。计算生成文本与原始文本之间的相似度或距离，并将其作为损失函数的一部分进行优化。

### 评估和分析

采用多种评估指标，包括困惑度（Perplexity）、BLEU 分数和 ROUGE 分数。模型在不同数据集和任务上的评估结果显示，InternLM2 在多个方面都取得了显著的性能提升。

## 创新点

- **条件在线 RLHF**：通过条件在线强化学习（COOL RLHF）方法，显著提高了模型在主观对话评估中的性能。
- **长序列处理能力**：采用分组查询注意力（GQA）结构，使得模型在处理长文本时更加高效稳定。

## 贡献和发布

InternLM2 以不同规模（1.8B、7B 和 20B 参数）的模型形式公开发布，这些模型在主观和客观评估中都展现出了卓越的性能。发布不同训练阶段的模型，为社区提供了模型演化的见解。

## 总结

InternLM2 通过一系列创新和细节处理，使其在多个领域都展现出了良好的性能。全链路开源开放体系提供了数据、预训练、微调、部署、评测和应用的一条龙服务框架，为社区的研究和应用提供了宝贵的资源。

## 参与贡献

更多信息请访问 [InternLM2 项目页面](https://internlm.openxlab.org.cn)。