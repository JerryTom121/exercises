---
title: "逻辑回归"
tags: [python, numpy]
---

第一个函数还是初始化数据，dataMat是属性数据集，在dataMat的第一列都设置为1主要是为了方便计算。labelMat存储的是标签数据。第二个函数即是Sigmoid函数公式。第三个函数是最主要的函数，用于计算最佳回归系数。首先将存储特征值的列表转换成矩阵形式。以便进行计算，将标签数据转换成列向量。alpha是向目标移动的步长，maxCycles是迭代次数，我们可以改变这两个值来确定最佳的回归系数。for循环里的前两句是计算真是类别与预测类别的差值，接下来按照差值的方向调整回归系数。