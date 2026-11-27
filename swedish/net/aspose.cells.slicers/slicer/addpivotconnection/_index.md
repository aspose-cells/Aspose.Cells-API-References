---
title: "Slicer.AddPivotConnection"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Slicer-metod. Lägger till PivotTable-anslutning"
type: docs
url: /sv/net/aspose.cells.slicers/slicer/addpivotconnection/
---
## Slicer.AddPivotConnection method

Lägger till PivotTable-anslutning.

```csharp
public void AddPivotConnection(PivotTable pivot)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| pivot | PivotTable | PivotTable‑objektet |

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Slicers;

namespace AsposeCellsExamples
{
    public class SlicerMethodAddPivotConnectionWithPivotTableDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Lägg till exempeldata för pivottabell
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["B1"].Value = "Quantity";
            cells["A2"].Value = "Apple";
            cells["A3"].Value = "Orange";
            cells["A4"].Value = "Banana";
            cells["B2"].Value = 10;
            cells["B3"].Value = 15;
            cells["B4"].Value = 5;

            // Skapa pivottabell
            PivotTableCollection pivotTables = sheet.PivotTables;
            int index = pivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivotTable = pivotTables[index];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");

            // Lägg till slicer - korrigerade parametrar
            int slicerIndex = sheet.Slicers.Add(pivotTable, 0, 0, "Slicer1");
            Slicer slicer = sheet.Slicers[slicerIndex];

            // Lägg till pivottabellsanslutning till slicer
            slicer.AddPivotConnection(pivotTable);

            // Spara arbetsboken
            workbook.Save("SlicerAddPivotConnectionDemo.xlsx");
        }
    }
}
```

### Se även

* class [PivotTable](../../../aspose.cells.pivot/pivottable/)
* class [Slicer](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)


