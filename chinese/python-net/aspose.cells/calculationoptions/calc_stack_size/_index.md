---
title: calc_stack_size 属性
second_title: Aspose.Cells for Python via .NET API 参考文献
description:
type: docs
weight: 30
url: /zh/python-net/aspose.cells/calculationoptions/calc_stack_size/
is_root: false
---
## calc_stack_size 属性

指定用于递归计算单元格的堆栈大小。

### 评论

当依赖树中有大量cell需要递归计算时，
StackOverflowException可能是在计算过程中引起的。
如果是这样，用户应该为此属性指定较小的值。
对于此类情况，用户应根据实际公式和数据确定该属性的合适值。
太小的值可能会导致公式计算的性能下降。
### 定义：
```python
@property
def calc_stack_size(self):
    ...
@calc_stack_size.setter
def calc_stack_size(self, value):
    ...
```

### 也可以看看
* 模块 [aspose.cells](../../)
* 类 [CalculationOptions](/cells/zh/python-net/aspose.cells/calculationoptions)
