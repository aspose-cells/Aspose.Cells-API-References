---
title: set_locked_property方法
second_title: Aspose.Cells for Python via .NET API 参考资料
description:
type: docs
weight: 190
url: /zh/python-net/aspose.cells.drawing/customxmlshape/set_locked_property/
is_root: false
---
##  set_locked_property(type, value) {#ShapeLockType-bool}
设置锁定属性。



```python
def set_locked_property(self, type, value):
    ...
```


|范围|类型|描述|
| :- | :- | :- |
| type | [ShapeLockType](/cells/zh/python-net/aspose.cells.drawing/shapelocktype) |锁定类型。|
| value | bool |属性的价值。|

### 例子

```python
from aspose.cells.drawing import ShapeLockType

shape.set_locked_property(ShapeLockType.ADJUST_HANDLES, True)

```



### 也可以看看
* 模块 [aspose.cells.drawing](../../)
* 类 [CustomXmlShape](/cells/zh/python-net/aspose.cells.drawing/customxmlshape)
