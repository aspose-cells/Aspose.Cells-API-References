---
title: Aspose::Cells::Drawing::Shape::UpdateSelectedValue method
linktitle: UpdateSelectedValue
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Drawing::Shape::UpdateSelectedValue method. Update the selected value by the value of the linked cell in C++.'
type: docs
weight: 14900
url: /ar/cpp/aspose.cells.drawing/shape/updateselectedvalue/
---
## Shape::UpdateSelectedValue method


Update the selected value by the value of the linked cell.

```cpp
void Aspose::Cells::Drawing::Shape::UpdateSelectedValue()
```


## Examples


```cpp
for (int i = 0; i < 10; ++i)
{
    Cell cell = book.GetWorksheets().Get(0).GetCells().Get(i, 0);
    cell.PutValue(i + 1);
}

//إنشاء كائن ListBox

//عناصر تحكم ActiveX
//Aspose.Cells.Drawing.Shape listBox = book.GetWorksheets().Get(0).GetShapes().AddActiveXControl( Aspose.Cells.Drawing.ActiveXControls.ControlType::ListBox,2, 0, 2, 0, 130, 130);

//عناصر تحكم النموذج
Shape listBox = book.GetWorksheets().Get(0).GetShapes().AddListBox(2, 0, 2, 0, 130, 130);

//يضبط النطاق المستخدم لملء العنصر.
listBox.SetInputRange(u"$A$1:$A$6", false, false);

//يضبط النطاق المرتبط بقيمة العنصر.
listBox.SetLinkedCell(u"$A$12", false, true);

ListBox listbx = (ListBox)listBox;

//تعيين قيمة الخلية A12
Cell cell = book.GetWorksheets().Get(0).GetCells().Get(11, 0);
cell.PutValue(3);

//تحديث القيمة المحددة بقيمة الخلية المرتبطة.
listBox.UpdateSelectedValue();

//-1 افتراضي، لا خيار محدد
if (listbx.IsSelected(2))
{
    //تم تحديد الخيار 3 من ListBox
}

//تغيير قيمة خلية مرتبطة
cell.PutValue(4);

//تحديث القيمة المحددة بقيمة الخلية المرتبطة.
listBox.UpdateSelectedValue();
if (listbx.IsSelected(3))
{
    //تم تحديد الخيار 4 من ListBox
}
```

## See Also

* Class [Vector](../../../aspose.cells/vector/)
* Class [Shape](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
