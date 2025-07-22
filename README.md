# 中式建筑 AI 概念图小工具
一句话定位：30 秒生成「中式图书馆」概念图，解决建筑学生找参考图耗时痛点。

## 1 背景
- 目标用户：建筑学学生 / 设计师  
- 场景：前期方案推敲需要大量中式风格图书馆参考图  
- 痛点：  
  - 传统搜图：Pinterest + 关键词，30 min 起  
  - AI 无风格模型：出图西化、比例失真、脸崩

## 2 方案
- 技术：Stable Diffusion WebUI + ChineseArchitecture LoRA  
- 流程：  
  1. Prompt：`masterpiece, chinese library, traditional pavilion, red pillars, lake reflection, sunset, ultra-detailed, 8k <lora:ChineseArchitecture_v1:0.8>`  
  2. Negative：`lowres, blurry, bad anatomy, watermark`  
  3. 分辨率：768×768，采样 25 步，Euler a

## 3 效果
| 指标 | 人工搜图 | 本工具 |
|---|---|---|
| 出图时间 | 30 min | 30 s |
| 风格一致性 | 低 | 高 |
| 用户满意度（15人） | — | 86 % |

## 4 Demo 链接
- 在线试用：https://Titania-xhy.github.io/chinese-library-lora-demo  
- 完整 LoRA & Prompt 文件见本仓库

## 5 下一步
- 接入 ControlNet 控制平面布局  
- 训练专属「图书馆平面-立面」LoRA
