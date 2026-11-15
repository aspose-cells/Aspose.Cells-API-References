---
title: Aspose::Cells::Drawing::Shape::UpdateSelectedValue method
linktitle: UpdateSelectedValue
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Drawing::Shape::UpdateSelectedValue method. Update the selected value by the value of the linked cell in C++.'
type: docs
weight: 14900
url: /ru/cpp/aspose.cells.drawing/shape/updateselectedvalue/
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

//Создать объект ListBox

//Элементы управления ActiveX
//Aspose.Cells.Drawing.Shape listBox = book.GetWorksheets().Get(0).GetShapes().AddActiveXControl( Aspose.Cells.Drawing.ActiveXControls.ControlType::ListBox,2, 0, 2, 0, 130, 130);

//Элементы управления формы
Shape listBox = book.GetWorksheets().Get(0).GetShapes().AddListBox(2, 0, 2, 0, 130, 130);

//Устанавливает диапазон, используемый для заполнения элемента управления.
listBox.SetInputRange(u"$A$1:$A$6", false, false);

//Устанавливает диапазон, связанный со значением элемента управления.
listBox.SetLinkedCell(u"$A$12", false, true);

ListBox listbx = (ListBox)listBox;

//Установить значение ячейки A12
Cell cell = book.GetWorksheets().Get(0).GetCells().Get(11, 0);
cell.PutValue(3);

//Обновить выбранное значение значением связанной ячейки.
listBox.UpdateSelectedValue();

//-1 по умолчанию, опция не выбрана
if (listbx.IsSelected(2))
{
    //Опция 3 ListBox выбрана
}

//Изменить значение связанной ячейки
cell.PutValue(4);

//Обновить выбранное значение значением связанной ячейки.
listBox.UpdateSelectedValue();
if (listbx.IsSelected(3))
{
    //Опция 4 ListBox выбрана
}
```

## See Also

* Class [Vector](../../../aspose.cells/vector/)
* Class [Shape](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
