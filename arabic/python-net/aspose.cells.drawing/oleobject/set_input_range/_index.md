---
title: طريقة set_input_range
second_title: Aspose.Cells for Python via .NET API المراجع
description:
type: docs
weight: 180
url: /ar/python-net/aspose.cells.drawing/oleobject/set_input_range/
is_root: false
---
##  set_input_range(formula, is_r1c1, is_local) {#str-bool-bool}
يضبط النطاق المستخدم لتعبئة عنصر التحكم.



```python
def set_input_range(self, formula, is_r1c1, is_local):
    ...
```


| معامل| يكتب| وصف|
| :- | :- | :- |
| formula | str | النطاق المستخدم لملء عنصر التحكم.|
| is_r1c1 | bool | ما إذا كانت الصيغة تحتاج إلى تنسيقها كـ R1C1.|
| is_local | bool | ما إذا كانت الصيغة تحتاج إلى التنسيق بواسطة الإعدادات المحلية.|

###  مثال

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



###  أنظر أيضا
* وحدة [aspose.cells.drawing](../../)
* فئة [OleObject](/cells/ar/python-net/aspose.cells.drawing/oleobject)
