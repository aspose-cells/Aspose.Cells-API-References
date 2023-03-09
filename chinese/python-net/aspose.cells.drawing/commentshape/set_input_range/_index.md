---
title: set_input_range方法
second_title: Aspose.Cells for Python via .NET API 参考文献
description:
type: docs
weight: 170
url: /zh/python-net/aspose.cells.drawing/commentshape/set_input_range/
is_root: false
---
##  set_input_range(formula, is_r1c1, is_local) {#str-bool-bool}
设置用于填充控件的范围。



```python
def set_input_range(self, formula, is_r1c1, is_local):
    ...
```


|参数|类型|描述|
| :- | :- | :- |
| formula | str |用于填充控件的范围。|
| is_r1c1 | bool |公式是否需要格式化为R1C1。|
| is_local | bool |公式是否需要按语言环境格式化。|

### 例子

```python

# After executing the code below, a ListBox object is created in the generated file. When the selected option is clicked, the selected value is displayed in cell A12.
# Initialize a new workbook.
# Workbook book = new Workbook();
for i in range(10):
    cell = book.worksheets[0].cells.get(i, 0)
    cell.value = i + 1
# Create a ListBox object
# ActiveX Controls
# Aspose.Cells.Drawing.Shape listBox = book.Worksheets[0].Shapes.AddActiveXControl( Aspose.Cells.Drawing.ActiveXControls.ControlType.ListBox,2, 0, 2, 0, 130, 130);
# Form Controls
listBox = book.worksheets[0].shapes.add_list_box(2, 0, 2, 0, 130, 130)
# Sets the range used to fill the control.
listBox.set_input_range("$A$1:$A$6", False, False)
# Sets the range linked to the control's value.
listBox.set_linked_cell("$A$12", False, True)

```



### 也可以看看
* 模块 [aspose.cells.drawing](../../)
* 类 [CommentShape](/cells/zh/python-net/aspose.cells.drawing/commentshape)
