---
title: get_locked_property方法
second_title: Aspose.Cells for Python via .NET API 参考资料
description:
type: docs
weight: 110
url: /zh/python-net/aspose.cells.drawing/combobox/get_locked_property/
is_root: false
---
##  get_locked_property(type) {#ShapeLockType}
获取锁定属性的值。


### 返回

返回锁定属性的值。


```python
def get_locked_property(self, type):
    ...
```


|范围|类型|描述|
| :- | :- | :- |
| type | [ShapeLockType](/cells/zh/python-net/aspose.cells.drawing/shapelocktype) |形状锁定属性的类型。|

### 例子

```python
from aspose.cells.drawing import ShapeLockType

noAdjustHandles = 0
if shape.get_locked_property(ShapeLockType.ADJUST_HANDLES):
    noAdjustHandles = 1

```



### 也可以看看
* 模块 [aspose.cells.drawing](../../)
* 类 [ComboBox](/cells/zh/python-net/aspose.cells.drawing/combobox)
