---
title: add方法
second_title: Aspose.Cells for Python via .NET API 参考文献
description:
type: docs
weight: 20
url: /zh/python-net/aspose.cells.drawing/textboxcollection/add/
is_root: false
---
##  add(upper_left_row, upper_left_column, height, width) {#int-int-int-int}
向集合中添加一个文本框。


### 返回

[TextBox](/cells/zh/python-net/aspose.cells.drawing/textbox) 对象索引。


```python
def add(self, upper_left_row, upper_left_column, height, width):
    ...
```


|参数|类型|描述|
| :- | :- | :- |
| upper_left_row | int |左上行索引。|
| upper_left_column | int |左上列索引。|
| height | int |文本框的高度，以像素为单位。|
| width | int |文本框的宽度，以像素为单位。|

### 例子

```python

# add a TextBox
index2 = textBoxCollection.add(1, 1, 50, 100)

```



### 也可以看看
* 模块 [aspose.cells.drawing](../../)
* 类 [TextBox](/cells/zh/python-net/aspose.cells.drawing/textbox)
* 类 [TextBoxCollection](/cells/zh/python-net/aspose.cells.drawing/textboxcollection)
