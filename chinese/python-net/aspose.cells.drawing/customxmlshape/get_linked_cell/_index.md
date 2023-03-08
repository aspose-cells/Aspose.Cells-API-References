---
title: get_linked_cell方法
second_title: Aspose.Cells for Python via .NET API 参考资料
description:
type: docs
weight: 100
url: /zh/python-net/aspose.cells.drawing/customxmlshape/get_linked_cell/
is_root: false
---
##  get_linked_cell(is_r1c1, is_local) {#bool-bool}
获取链接到控件值的范围。


### 返回

链接到控件值的范围。


```python
def get_linked_cell(self, is_r1c1, is_local):
    ...
```


|范围|类型|描述|
| :- | :- | :- |
| is_r1c1 | bool |公式是否需要格式化为R1C1。|
| is_local | bool |公式是否需要按语言环境格式化。|

### 例子

```python

# You may get results like '$A$1'
link = shape.get_linked_cell(False, False)

```



### 也可以看看
* 模块 [aspose.cells.drawing](../../)
* 类 [CustomXmlShape](/cells/zh/python-net/aspose.cells.drawing/customxmlshape)
