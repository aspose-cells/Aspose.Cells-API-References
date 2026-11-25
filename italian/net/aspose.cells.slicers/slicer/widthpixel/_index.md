---
title: "Slicer.WidthPixel"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Slicer. Restituisce o imposta la larghezza dello slicer specificato in pixel"
type: docs
url: /it/net/aspose.cells.slicers/slicer/widthpixel/
---
## Slicer.WidthPixel property

Restituisce o imposta la larghezza dello slicer specificato, in pixel.

```csharp
[Obsolete("Use Shape.Width property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int WidthPixel { get; set; }
```

### Osservazioni

NOTA: Questo membro è ora obsoleto. Invece, si prega di utilizzare la proprietà Shape.Width. Questa proprietà sarà rimossa 12 mesi dopo, a partire da maggio 2025. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

### Esempi

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

### Vedi anche

* class [Slicer](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)


