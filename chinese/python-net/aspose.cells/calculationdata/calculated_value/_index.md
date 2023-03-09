---
title: calculated_value 属性
second_title: Aspose.Cells for Python via .NET API 参考文献
description:
type: docs
weight: 50
url: /zh/python-net/aspose.cells/calculationdata/calculated_value/
is_root: false
---
## calculated_value 属性

获取或设置此函数的计算值。

### 评论

用户应在其自定义计算引擎中为引擎支持的那些功能设置此属性，
稍后获取该属性时返回设置值。
设置值可以是那些可以设置为 Cell(Cell.Value) 的对象的任何值。
它也可以是此类值的数组，或范围、名称、引用区域。
在设置前获取该属性，将使该函数被默认的Aspose.Cells计算引擎计算，并返回计算出的值。
### 定义：
```python
@property
def calculated_value(self):
    ...
@calculated_value.setter
def calculated_value(self, value):
    ...
```

### 也可以看看
* 模块 [aspose.cells](../../)
* 类 [CalculationData](/cells/zh/python-net/aspose.cells/calculationdata)
