# PaddleRec 推荐系统框架（学习副本）

本仓库为飞桨 [PaddleRec](https://github.com/PaddlePaddle/PaddleRec) 推荐系统开源框架的完整代码副本，用于学习与研究。

## 简介

PaddleRec 是源于飞桨生态的搜索推荐模型**一站式开箱即用工具**，覆盖内容理解、匹配、召回、排序、多任务、重排序等多个任务的完整推荐搜索算法库，适合初学者、开发者与研究者。

## 文档

- 中文文档：[README_CN.md](./README_CN.md)
- 英文文档：[README_EN.md](./README_EN.md)
- 官方仓库：https://github.com/PaddlePaddle/PaddleRec

## 环境要求

- Python 3.7（推荐）
- PaddlePaddle >= 2.0
- 操作系统：Windows / Mac / Linux

## 快速运行示例

以排序模型 `dnn` 为例（数据为 Criteo 数据集截取的 100 条）：

```bash
python -u tools/trainer.py -m models/rank/dnn/config.yaml        # 动态图训练
python -u tools/static_trainer.py -m models/rank/dnn/config.yaml # 静态图训练
```
