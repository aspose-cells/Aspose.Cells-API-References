---
title: Aspose::Cells::Drawing::Shape::UpdateSelectedValue method
linktitle: UpdateSelectedValue
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Drawing::Shape::UpdateSelectedValue method. Update the selected value by the value of the linked cell in C++.'
type: docs
weight: 14900
url: /de/cpp/aspose.cells.drawing/shape/updateselectedvalue/
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

//Erstelle ein ListBox-Objekt

//ActiveX-Steuerelemente
//Aspose.Cells.Drawing.Shape listBox = book.GetWorksheets().Get(0).GetShapes().AddActiveXControl( Aspose.Cells.Drawing.ActiveXControls.ControlType::ListBox,2, 0, 2, 0, 130, 130);

//Formularsteuerelemente
Shape listBox = book.GetWorksheets().Get(0).GetShapes().AddListBox(2, 0, 2, 0, 130, 130);

//Setzt den Bereich, der zum Befüllen des Steuerelements verwendet wird.
listBox.SetInputRange(u"$A$1:$A$6", false, false);

//Setzt den Bereich, der mit dem Wert des Steuerelements verknüpft ist.
listBox.SetLinkedCell(u"$A$12", false, true);

ListBox listbx = (ListBox)listBox;

//Setze den Wert der Zelle A12
Cell cell = book.GetWorksheets().Get(0).GetCells().Get(11, 0);
cell.PutValue(3);

//Aktualisiere den ausgewählten Wert anhand des Werts der verknüpften Zelle.
listBox.UpdateSelectedValue();

//-1 Standard, keine Option ausgewählt
if (listbx.IsSelected(2))
{
    //Option 3 der ListBox ist ausgewählt
}

//Ändere den Wert einer verknüpften Zelle
cell.PutValue(4);

//Aktualisiere den ausgewählten Wert anhand des Werts der verknüpften Zelle.
listBox.UpdateSelectedValue();
if (listbx.IsSelected(3))
{
    //Option 4 der ListBox ist ausgewählt
}
```

## See Also

* Class [Vector](../../../aspose.cells/vector/)
* Class [Shape](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
