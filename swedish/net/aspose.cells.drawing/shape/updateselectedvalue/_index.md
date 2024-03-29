---
title: UpdateSelectedValue
second_title: Aspose.Cells för .NET API-referens
description: Uppdatera det valda värdet med värdet för den länkade cellen.
type: docs
weight: 1170
url: /sv/net/aspose.cells.drawing/shape/updateselectedvalue/
---
## Shape.UpdateSelectedValue method

Uppdatera det valda värdet med värdet för den länkade cellen.

```csharp
public void UpdateSelectedValue()
```

### Exempel

```csharp

[C#]
//Initiera en ny arbetsbok.
//Arbetsbok bok = ny arbetsbok();

Cell cell = null;
for (int i = 0; i< 10; ++i)
{
    cell = book.Worksheets[0].Cells[i, 0];
    cell.Value = i + 1;
}
   
//Skapa ett ListBox-objekt

//ActiveX-kontroller
//Aspose.Cells.Drawing.Shape listBox = book.Worksheets[0].Shapes.AddActiveXControl( Aspose.Cells.Drawing.ActiveXControls.ControlType.ListBox,2, 0, 2, 0, 130, 130);

//Formularkontroller
Aspose.Cells.Drawing.Shape listBox = book.Worksheets[0].Shapes.AddListBox(2, 0, 2, 0, 130, 130);

//Ställer in intervallet som används för att fylla kontrollen.
listBox.SetInputRange("$A$1:$A$6", false, false);

//Ställer in intervallet kopplat till kontrollens värde.
listBox.SetLinkedCell("$A$12", false, true);

ListBox listbx = (ListBox)listBox;

//Ställ in värdet för cell A12
cell = book.Worksheets[0].Cells[11, 0];
cell.Value = 3;

//Uppdatera det valda värdet med värdet för den länkade cellen.
listBox.UpdateSelectedValue();

//-1 standard, inget alternativ valt
if(listbx.IsSelected(2))
{
    //Alternativ 3 i ListBox är valt
}

//Ändra värdet på en länkad cell
cell.Value = 4;

//Uppdatera det valda värdet med värdet för den länkade cellen.
listBox.UpdateSelectedValue();
if(listbx.IsSelected(3))
{
    //Alternativ 4 i ListBox är valt
}

```

### Se även

* class [Shape](../../shape)
* namnutrymme [Aspose.Cells.Drawing](../../shape)
* hopsättning [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
