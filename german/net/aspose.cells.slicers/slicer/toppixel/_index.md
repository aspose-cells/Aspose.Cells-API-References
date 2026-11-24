---
title: "Slicer.TopPixel"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Slicer-Eigenschaft. Gibt den vertikalen Abstand der Slicer-Form von ihrer oberen Zeile in Pixeln zurück oder legt ihn fest"
type: docs
url: /de/net/aspose.cells.slicers/slicer/toppixel/
---
## Slicer.TopPixel property

Gibt den vertikalen Abstand der Slicer-Form von ihrer oberen Zeile zurück oder legt ihn fest, in Pixeln.

```csharp
[Obsolete("Use Shape.Top property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int TopPixel { get; set; }
```

### Hinweise

HINWEIS: Dieses Mitglied ist jetzt veraltet. Stattdessen verwenden Sie bitte die Shape.Top‑Eigenschaft. Diese Eigenschaft wird 12 Monate später, seit Mai 2025, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie erlebt haben.

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Slicers;

namespace AsposeCellsExamples
{
    public class SlicerPropertyTopPixelDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Erstelle Beispieldaten
            sheet.Cells["A1"].Value = "Product";
            sheet.Cells["A2"].Value = "Apple";
            sheet.Cells["A3"].Value = "Orange";
            sheet.Cells["A4"].Value = "Banana";
            sheet.Cells["B1"].Value = "Sales";
            sheet.Cells["B2"].Value = 100;
            sheet.Cells["B3"].Value = 200;
            sheet.Cells["B4"].Value = 300;

            // Pivot-Tabelle erstellen und ihren Index abrufen
            int pivotIndex = sheet.PivotTables.Add("=A1:B4", "D1", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Slicer hinzufügen und seinen Index abrufen
            int slicerIndex = sheet.Slicers.Add(pivotTable, "A6", 0);
            Slicer slicer = sheet.Slicers[slicerIndex];
            
            // TopPixel-Eigenschaft festlegen
            slicer.TopPixel = 6;
            
            workbook.Save("SlicerTopPixelDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Slicer](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)


