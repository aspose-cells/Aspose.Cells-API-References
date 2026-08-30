---
title: Aspose::Cells::Drawing::Shape::UpdateSelectedValue method
linktitle: UpdateSelectedValue
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Drawing::Shape::UpdateSelectedValue method. Update the selected value by the value of the linked cell in C++.'
type: docs
weight: 14900
url: /sv/cpp/aspose.cells.drawing/shape/updateselectedvalue/
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

//Skapa ett ListBox-objekt

//ActiveX-kontroller
//Aspose.Cells.Drawing.Shape listBox = book.GetWorksheets().Get(0).GetShapes().AddActiveXControl( Aspose.Cells.Drawing.ActiveXControls.ControlType::ListBox,2, 0, 2, 0, 130, 130);

//Formulärkontroller
Shape listBox = book.GetWorksheets().Get(0).GetShapes().AddListBox(2, 0, 2, 0, 130, 130);

//Ställer in intervallet som används för att fylla kontrollen.
listBox.SetInputRange(u"$A$1:$A$6", false, false);

//Ställer in intervallet som är länkat till kontrollens värde.
listBox.SetLinkedCell(u"$A$12", false, true);

ListBox listbx = (ListBox)listBox;

//Ange värdet för cell A12
Cell cell = book.GetWorksheets().Get(0).GetCells().Get(11, 0);
cell.PutValue(3);

//Uppdatera det valda värdet med värdet från den länkade cellen.
listBox.UpdateSelectedValue();

//-1 standard, inget alternativ valt
if (listbx.IsSelected(2))
{
    //Alternativ 3 i ListBox är valt
}

//Ändra värdet i en länkad cell
cell.PutValue(4);

//Uppdatera det valda värdet med värdet från den länkade cellen.
listBox.UpdateSelectedValue();
if (listbx.IsSelected(3))
{
    //Alternativ 4 i ListBox är valt
}
```

## See Also

* Class [Vector](../../../aspose.cells/vector/)
* Class [Shape](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
