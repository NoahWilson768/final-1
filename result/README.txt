RESULT DIRECTORY OVERVIEW
==========================

This file describes how experimental outputs are organized.

实验结果目录结构（按照中文实验分类）:
  result/01_基础走廊生成实验(Reference_Table2)/
    - 水平走廊/                          # Category A: 水平走廊基础实验 (paths, metrics, tensor_fields)
    - 垂直走廊/                          # Category A: 垂直走廊基础实验 (paths, metrics)
  result/02_多层空域走廊生成实验(Reference_Fig3)/
    - 北京CBD/                          # Category B: 北京多层实验 (paths, metrics, tensor_fields)
    - 上海陆家嘴/                        # Category B: 上海多层实验
    - 广州珠江新城/                      # Category B: 广州多层实验
    - 深圳福田/                          # Category B: 深圳多层实验
  result/03_水平走廊参数敏感性实验(Reference_Fig5)/
    - C1-C3_网格分辨率/                  # Category C: 网格分辨率实验
    - C4-C6_粘度系数/                    # Category C: 粘度系数实验
    - C7-C9_Poisson迭代/                 # Category C: Poisson迭代实验
    - C10-C11_安全边界/                  # Category C: 安全边界实验
    - C12_B样条平滑/                     # Category C: B样条平滑实验
  result/04_垂直走廊参数敏感性实验(Reference_Fig6)/
    - 策略矩阵/                           # Category D: 策略×分辨率矩阵 (paths, metrics, tensor_fields)
  result/05_消融实验(Ablation_Study)/    # Category E: 消融实验 (paths, metrics, tensor_fields)
  result/06_数学验证实验(Validation)/    # Category F: 验证实验 (数学正确性)
    - F1_稳定域热图/                     # F.1: 稳定域热图
    - F2_条件数消融/                     # F.2: 条件数消融
    - F3_散度验证/                       # F.3: 散度验证
    - F4_能量守恒/                       # F.4: 能量守恒验证
    - F5_边界一致性/                     # F.5: 边界一致性
    - F6_张量消融/                       # F.6: 张量消融
    - F7_CFL自适应压力测试/              # F.7: CFL自适应压力测试
    - F8_旋转各向异性压力测试/          # F.8: 旋转各向异性压力测试
  result/07_综合分析报告(Comprehensive_Report)/  # 综合分析报告 (performance, sensitivity, reference comparison)
  result/Reference对照/                  # Reference.pdf对照图表
    - Fig_3/                             # 12个子图：多层空域走廊
    - Fig_5/                             # 12个子图：水平参数敏感性
    - Fig_6/                             # 12个子图：垂直参数敏感性
  logs/                                  # 执行日志和实验摘要

Notes:
- 所有实验数据按照实验类别（Category A-F）进行中文分类组织
- 每个实验子目录包含 paths/（图片）、metrics/（性能指标）、tensor_fields/（张量场可视化）
- Reference对照文件夹包含与Reference.pdf对应的图表
- 详细实验摘要保存在 logs/experiment_summary.json
