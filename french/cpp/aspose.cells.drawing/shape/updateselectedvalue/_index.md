---
title: Aspose::Cells::Drawing::Shape::UpdateSelectedValue method
linktitle: UpdateSelectedValue
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Drawing::Shape::UpdateSelectedValue method. Update the selected value by the value of the linked cell in C++.'
type: docs
weight: 14900
url: /fr/cpp/aspose.cells.drawing/shape/updateselectedvalue/
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

//Créer un objet ListBox

//Contrôles ActiveX
//Aspose.Cells.Drawing.Shape listBox = book.GetWorksheets().Get(0).GetShapes().AddActiveXControl( Aspose.Cells.Drawing.ActiveXControls.ControlType::ListBox,2, 0, 2, 0, 130, 130);

//Contrôles de formulaire
Shape listBox = book.GetWorksheets().Get(0).GetShapes().AddListBox(2, 0, 2, 0, 130, 130);

//Définit la plage utilisée pour remplir le contrôle.
listBox.SetInputRange(u"$A$1:$A$6", false, false);

//Définit la plage liée à la valeur du contrôle.
listBox.SetLinkedCell(u"$A$12", false, true);

ListBox listbx = (ListBox)listBox;

//Définir la valeur de la cellule A12
Cell cell = book.GetWorksheets().Get(0).GetCells().Get(11, 0);
cell.PutValue(3);

//Mettre à jour la valeur sélectionnée par la valeur de la cellule liée.
listBox.UpdateSelectedValue();

//-1 par défaut, aucune option sélectionnée
if (listbx.IsSelected(2))
{
    //L'option 3 de la ListBox est sélectionnée
}

//Modifier la valeur d'une cellule liée
cell.PutValue(4);

//Mettre à jour la valeur sélectionnée par la valeur de la cellule liée.
listBox.UpdateSelectedValue();
if (listbx.IsSelected(3))
{
    //L'option 4 de la ListBox est sélectionnée
}
```

## See Also

* Class [Vector](../../../aspose.cells/vector/)
* Class [Shape](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
