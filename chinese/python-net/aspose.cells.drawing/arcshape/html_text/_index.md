---
title: html_text 属性
second_title: Aspose.Cells for Python via .NET API 参考资料
description:
type: docs
weight: 540
url: /zh/python-net/aspose.cells.drawing/arcshape/html_text/
is_root: false
---
## html_text 属性

获取和设置此文本框中包含数据和某些格式的 html 字符串。

### 例子

```python

html = shape.html_text
if html == null  || html == "":
    shape.html_text = "<Font Style='FONT-FAMILY: Calibri;FONT-SIZE: 11pt;COLOR: #0000ff;TEXT-ALIGN: left;'>This is a <b>test</b>.</Font>"

```
### 定义：
```python
@property
def html_text(self):
    ...
@html_text.setter
def html_text(self, value):
    ...
```

### 也可以看看
* 模块 [aspose.cells.drawing](../../)
* 类 [ArcShape](/cells/zh/python-net/aspose.cells.drawing/arcshape)
