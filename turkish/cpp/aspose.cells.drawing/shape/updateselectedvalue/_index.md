---
title: Aspose::Cells::Drawing::Shape::UpdateSelectedValue method
linktitle: UpdateSelectedValue
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Drawing::Shape::UpdateSelectedValue method. Update the selected value by the value of the linked cell in C++.'
type: docs
weight: 14900
url: /tr/cpp/aspose.cells.drawing/shape/updateselectedvalue/
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

//Bir ListBox nesnesi oluştur

//ActiveX Kontrolleri
//Aspose.Cells.Drawing.Shape listBox = book.GetWorksheets().Get(0).GetShapes().AddActiveXControl( Aspose.Cells.Drawing.ActiveXControls.ControlType::ListBox,2, 0, 2, 0, 130, 130);

//Form Kontrolleri
Shape listBox = book.GetWorksheets().Get(0).GetShapes().AddListBox(2, 0, 2, 0, 130, 130);

//Kontrolü doldurmak için kullanılan aralığı ayarlar.
listBox.SetInputRange(u"$A$1:$A$6", false, false);

//Kontrolün değerine bağlı aralığı ayarlar.
listBox.SetLinkedCell(u"$A$12", false, true);

ListBox listbx = (ListBox)listBox;

//A12 hücresinin değerini ayarla
Cell cell = book.GetWorksheets().Get(0).GetCells().Get(11, 0);
cell.PutValue(3);

//Seçili değeri bağlı hücrenin değeriyle güncelle.
listBox.UpdateSelectedValue();

//-1 varsayılan, seçenek seçilmedi
if (listbx.IsSelected(2))
{
    //ListBox'ın 3. seçeneği seçildi
}

//Bağlı bir hücrenin değerini değiştir
cell.PutValue(4);

//Seçili değeri bağlı hücrenin değeriyle güncelle.
listBox.UpdateSelectedValue();
if (listbx.IsSelected(3))
{
    //ListBox'ın 4. seçeneği seçildi
}
```

## See Also

* Class [Vector](../../../aspose.cells/vector/)
* Class [Shape](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
