---
title: "ShapeCollection.UpdateSelectedValue"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ShapeCollection-metod. Uppdatera det valda värdet med värdet från den länkade cellen eller shape-området"
type: docs
url: /sv/net/aspose.cells.drawing/shapecollection/updateselectedvalue/
---
## ShapeCollection.UpdateSelectedValue method

Uppdatera det valda värdet med värdet från den länkade cellen eller området för formen.

```csharp
public void UpdateSelectedValue()
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodUpdateSelectedValueDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok med exempeldata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till en shape (rullgardinslista) i kalkylbladet
            Aspose.Cells.Drawing.ListBox listBox = (Aspose.Cells.Drawing.ListBox)worksheet.Shapes.AddListBox(0, 0, 100, 100, 3, 20);
            
            // Ange listobjekt och valt värde
            listBox.SetInputRange("A1:A3", false, false);
            listBox.SelectedIndex = 1;
            
            // Uppdatera det valda värdet i shape:n
            worksheet.Shapes.UpdateSelectedValue();
            
            // Spara arbetsboken
            workbook.Save("ShapeCollectionUpdateSelectedValueDemo.xlsx");
        }
    }
}
```

### Se även

* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


