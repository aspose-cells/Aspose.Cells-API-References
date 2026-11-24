---
title: "Slicer.RowHeightPixel"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Slicer-Eigenschaft. Gibt die Höhe jeder Zeile im angegebenen Slicer in Pixel zurück oder legt sie fest"
type: docs
url: /de/net/aspose.cells.slicers/slicer/rowheightpixel/
---
## Slicer.RowHeightPixel property

Gibt die Höhe jeder Zeile im angegebenen Slicer zurück oder legt sie fest, in der Einheit Pixel.

```csharp
public int RowHeightPixel { get; set; }
```

### Beispiele

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

            // Beispieldaten für Pivot‑Tabelle erstellen
            sheet.Cells["A1"].PutValue("Fruit");
            sheet.Cells["B1"].PutValue("Quantity");
            sheet.Cells["A2"].PutValue("Apple");
            sheet.Cells["B2"].PutValue(50);
            sheet.Cells["A3"].PutValue("Orange");
            sheet.Cells["B3"].PutValue(30);
            sheet.Cells["A4"].PutValue("Banana");
            sheet.Cells["B4"].PutValue(40);

            // Pivot-Tabelle erstellen
            int pivotIndex = workbook.Worksheets[0].PivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Slicer hinzufügen und Referenz erhalten
            int slicerIndex = sheet.Slicers.Add(pivotTable, "A1", "Fruit");
            Slicer slicer = sheet.Slicers[slicerIndex];
            
            // Slicer‑Eigenschaften festlegen
            slicer.RowHeightPixel = 30;
            slicer.Width = 150;

            workbook.Save("SlicerRowHeightDemo_output.xlsx");
        }
    }
}
```

### Siehe auch

* class [Slicer](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)


