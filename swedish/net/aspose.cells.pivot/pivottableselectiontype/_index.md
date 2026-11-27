---
title: "Enum PivotTableSelectionType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Pivot.PivotTableSelectionType‑enum. Anger vad som kan väljas i en pivottabell under en strukturerad markering. Dessa konstanter kan kombineras för att välja flera typer."
type: docs
url: /sv/net/aspose.cells.pivot/pivottableselectiontype/
---
## PivotTableSelectionType enumeration

Anger vad som kan väljas i en PivotTable under en strukturerad markering. Dessa konstanter kan kombineras för att välja flera typer.

```csharp
public enum PivotTableSelectionType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| DataAndLabel | `0` | Data och etiketter |
| DataOnly | `2` | Väljer endast data |
| LabelOnly | `1` | Väljer endast etiketter |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTableSelectionTypeDemo
    {
        public static void PivotTableSelectionTypeExample()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till lite data för pivottabellen
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(150);
            worksheet.Cells["A4"].PutValue("A");
            worksheet.Cells["B4"].PutValue(200);
            worksheet.Cells["A5"].PutValue("B");
            worksheet.Cells["B5"].PutValue(250);

            // Skapa en pivottabell
            int pivotIndex = worksheet.PivotTables.Add("A1:B5", "D1", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Lägg till fält i pivottabellen
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Skapa ett PivotArea och ange dess egenskaper
            PivotArea pivotArea = new PivotArea(pivotTable);
            pivotArea.AxisType = PivotFieldType.Row;
            pivotArea.OnlyData = false;
            pivotArea.OnlyLabel = true;
            pivotArea.IsRowGrandIncluded = true;
            pivotArea.IsColumnGrandIncluded = true;
            pivotArea.IsOutline = false;

            // Markera området med en specifik markeringstyp
            pivotArea.Select(PivotFieldType.Row, 0, PivotTableSelectionType.LabelOnly);

            // Spara arbetsboken
            workbook.Save("PivotTableSelectionTypeExample.xlsx");

            return;
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


