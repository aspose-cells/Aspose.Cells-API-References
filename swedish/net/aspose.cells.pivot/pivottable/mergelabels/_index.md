---
title: "PivotTable.MergeLabels"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotTable-egenskap. Hämtar eller anger om rad‑/kolumnetiketter som sträcker sig över flera celler ska slås ihop"
type: docs
url: /sv/net/aspose.cells.pivot/pivottable/mergelabels/
---
## PivotTable.MergeLabels property

Hämtar eller anger om rad-/kolumnfältetiketter som sträcker sig över flera celler ska slås ihop.

```csharp
public bool MergeLabels { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyMergeLabelsDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok med exempeldata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata för pivottabell
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["B1"].Value = "Quantity";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Apple";
            worksheet.Cells["A4"].Value = "Orange";
            worksheet.Cells["A5"].Value = "Orange";
            worksheet.Cells["B2"].Value = 10;
            worksheet.Cells["B3"].Value = 15;
            worksheet.Cells["B4"].Value = 8;
            worksheet.Cells["B5"].Value = 12;

            // Skapa pivottabell
            int pivotIndex = worksheet.PivotTables.Add("A1:B5", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // Lägg till radfält och datafält
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
            
            // Aktivera sammanslagning av etiketter
            pivotTable.MergeLabels = true;
            
            // Spara arbetsboken
            workbook.Save("PivotTableMergeLabelsDemo.xlsx");
        }
    }
}
```

### Se även

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


