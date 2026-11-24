---
title: "Slicer.WidthPixel"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Slicer-Eigenschaft. Gibt die Breite des angegebenen Slicers in Pixel zurück oder legt sie fest."
type: docs
url: /de/net/aspose.cells.slicers/slicer/widthpixel/
---
## Slicer.WidthPixel property

Gibt die Breite des angegebenen Slicers zurück oder legt sie fest, in Pixel.

```csharp
[Obsolete("Use Shape.Width property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int WidthPixel { get; set; }
```

### Hinweise

HINWEIS: Dieses Mitglied ist jetzt veraltet. Verwenden Sie stattdessen die Shape.Width‑Eigenschaft. Diese Eigenschaft wird 12 Monate nach Mai 2025 entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Ihnen entstanden sein könnten.

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;
using Aspose.Cells.Slicers;

namespace AsposeCellsExamples
{
    public class SlicerPropertyWidthPixelDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            sheet.Cells["A1"].PutValue("Product");
            sheet.Cells["A2"].PutValue("Apple");
            sheet.Cells["A3"].PutValue("Banana");
            sheet.Cells["B1"].PutValue("Sales");
            sheet.Cells["B2"].PutValue(150);
            sheet.Cells["B3"].PutValue(200);
            
            int tableIndex = sheet.ListObjects.Add(0, 0, 2, 1, true);
            ListObject table = sheet.ListObjects[tableIndex];
            
            int slicerIndex = sheet.Slicers.Add(table, 0, "A5");
            Slicer slicer = sheet.Slicers[slicerIndex];
            slicer.LeftPixel = 50;
            slicer.TopPixel = 100;
            slicer.WidthPixel = 120;
            
            workbook.Save("SlicerWidthDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Slicer](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)


