# Qwen3.5-0.8B Colab Training Notebook

## Open in Colab

**直接点击下方链接打开**（推荐）：

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/systemoutprintlnnnn/dsaa-5009-qwen-colab/blob/main/qwen_colab.ipynb)

或者使用完整链接：
```
https://colab.research.google.com/github/systemoutprintlnnnn/dsaa-5009-qwen-colab/blob/main/qwen_colab.ipynb
```

## 功能

- Qwen3.5-0.8B 全量训练 (12,460 samples)
- Flash Attention 2 / SDPA 自动降级
- batch_size=16 + gradient_checkpointing
- Colab 内直接评测

## 运行时间（T4）

| 实验 | 时间 |
|------|------|
| Exp0 baseline | ~45 分钟 |
| Exp1 length ctrl | ~45 分钟 |
| Exp1_multi | ~90 分钟 |
| **合计** | **~3 小时** |

## 更新日志

- v5 (当前): 修复 torch_dtype->dtype, 删除 save_safetensors, transformers 升级
- v4: 修复 torch_dtype
- v3: transformers 升级
- v2: 批量数据预处理, batch_size 16, Colab 内评测
