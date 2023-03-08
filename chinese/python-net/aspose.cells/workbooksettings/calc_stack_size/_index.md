---
title: calc_stack_size 属性
second_title: Aspose.Cells for Python via .NET API 参考资料
description:
type: docs
weight: 100
url: /zh/python-net/aspose.cells/workbooksettings/calc_stack_size/
is_root: false
---
## calc_stack_size 属性

指定用于递归计算单元格的堆栈大小。
当需要递归计算大量单元格时，此大小的较大值将提供更好的性能。
另一方面，较大的值会增加 StackOverflowException 的风险。
如果用户在计算公式时出现 StackOverflowException，则应减小此值。

### 评论

注意：该成员现已过时。相反，请使用 CalculationOptions
在计算公式时使用指定的 CalcStackSize。
自 2022 年 2 月起，此属性将在 12 个月后移除。
Aspose 对您可能遇到的任何不便深表歉意。
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
* 类 [WorkbookSettings](/cells/zh/python-net/aspose.cells/workbooksettings)
