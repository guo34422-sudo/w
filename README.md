# 结合视觉与文本特征的多模态隐喻情感识别方法支撑数据说明

## 1. 数据说明

本数据包为论文《结合视觉与文本特征的多模态隐喻情感识别方法》的支撑数据。

## 2. 文件结构

```text
MMSR_supporting_data/
├── README.md
├── results_summary.xlsx
├── human_evaluation_annotations.xlsx
```

## 3. 文件内容说明

### 3.1 README.md

本文件用于说明支撑数据包的整体结构、文件内容、数据来源、使用方式和注意事项。

### 3.3 results_summary.xlsx

该文件为论文主要结果的汇总数据，包含以下工作表：

| Sheet 名称                 | 内容说明                                                 | 对应论文内容      |
| ------------------------ | ---------------------------------------------------- | ----------- |
| dataset_statistics       | 三个数据集的类别统计信息                                         | 表 1、表 2、表 3 |
| main_results             | 各模型在 MET-Meme、MultiMET 和 MultiCMET 数据集上的 ACC 和 F1 结果 | 表 4         |
| ablation_results         | 消融实验结果，包括三跳推理、图像处理和模态融合等模块的影响                        | 表 5         |
| human_evaluation_summary | 生成解释质量人工评估的汇总结果                                      | 表 6         |

其中，`dataset_statistics` 用于支撑论文中的数据集统计结果；`main_results` 用于支撑论文中的整体实验结果；`ablation_results` 用于支撑论文中的模块有效性分析；`human_evaluation_summary` 用于支撑论文中的生成解释质量评估结果。

### 3.4 human_evaluation_annotations.xlsx

该文件为人工评估的样本级标注结果，用于支撑论文中生成解释质量评估部分。文件包含 200 条抽样样本的最终标注结果。

主要字段说明如下：

| 字段名                  | 含义                       |
| -------------------- | ------------------------ |
| Pic_id               | 样本或图片编号                  |
| result       | 多模态大语言模型生成的解释或描述结果       |
| faithfulness_final   | 忠实性最终判断结果，1 表示通过，0 表示未通过 |
| reasonableness_final | 合理性最终判断结果，1 表示通过，0 表示未通过 |


## 4. 数据来源说明

本研究使用的原始图像和文本数据来自以下公开数据集：

1. Multi-MET：英文多模态隐喻理解数据集；
2. MultiCMET：中文多模态隐喻理解数据集；
3. MET-Meme：包含隐喻、情感等标注的多模态模因数据集。

由于上述数据集包含第三方图像资源，本数据包未上传原始图片文件。研究者如需获取原始图像和文本数据，请根据相应数据集的官方发布渠道获取。

