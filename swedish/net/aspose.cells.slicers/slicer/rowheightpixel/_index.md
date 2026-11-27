---
title: "Slicer.RowHeightPixel"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Slicer-egenskap. Returnerar eller anger höjden på varje rad i den angivna slicern i enheten pixlar"
type: docs
url: /sv/net/aspose.cells.slicers/slicer/rowheightpixel/
---
## Slicer.RowHeightPixel property

Returnerar eller anger höjden på varje rad i den angivna slicern, i enheter av pixlar.

```csharp
public int RowHeightPixel { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Slicers;

namespace AsposeCellsExamples
{
    public class SlicerPropertyRowHeightPixelDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Skapa exempeldata för pivottabell
            sheet.Cells["A1"].PutValue("Fruit");
            sheet.Cells["B1"].PutValue("Quantity");
            sheet.Cells["A2"].PutValue("Apple");
            sheet.Cells["B2"].PutValue(50);
            sheet.Cells["A3"].PutValue("Orange");
            sheet.Cells["B3"].PutValue(30);
            sheet.Cells["A4"].PutValue("Banana");
            sheet.Cells["B4"].PutValue(40);

            // Skapa pivottabell
            int pivotIndex = workbook.Worksheets[0].PivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Lägg till slicer och hämta referens
            int slicerIndex = sheet.Slicers.Add(pivotTable, "A1", "Fruit");
            Slicer slicer = sheet.Slicers[slicerIndex];
            
            // Ange skivkontrollens egenskaper
            slicer.RowHeightPixel = 30;
            slicer.Width = 150;

            workbook.Save("SlicerRowHeightDemo_output.xlsx");
        }
    }
}
```

### Se även

* class [Slicer](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)


