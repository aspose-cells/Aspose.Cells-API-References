---
title: "SlicerCollection.RemoveAt"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SlicerCollection-metod. Tar bort slicern på angivet index"
type: docs
url: /sv/net/aspose.cells.slicers/slicercollection/removeat/
---
## SlicerCollection.RemoveAt method

Tar bort slicern på angivet index

```csharp
public void RemoveAt(int index)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| index | Int32 | Positionsindex i Slicer-samlingen |

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class SlicerCollectionMethodRemoveAtWithInt32Demo
    {
        public static void Run()
        {
            // Skapa en arbetsbok
            Workbook workbook = new Workbook();
            
            // Lägg till ett kalkylblad
            Worksheet worksheet = workbook.Worksheets.Add("Sheet1");
            
            // Lägg till lite data för pivåtabellen
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B1"].Value = "Quantity";
            worksheet.Cells["B2"].Value = 10;
            worksheet.Cells["B3"].Value = 5;
            worksheet.Cells["B4"].Value = 8;

            // Lägg till en pivottabell
            int index = worksheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");

            // Lägg till slicers
            Aspose.Cells.Slicers.SlicerCollection slicers = worksheet.Slicers;
            slicers.Add(pivotTable, "Fruit", "FruitSlicer1");
            slicers.Add(pivotTable, "Fruit", "FruitSlicer2");

            // Ta bort den andra slicern på index 1
            slicers.RemoveAt(1);
            
            // Spara arbetsboken
            workbook.Save("SlicerCollectionMethodRemoveAtWithInt32Demo.xlsx");
        }
    }
}
```

### Se även

* class [SlicerCollection](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)


