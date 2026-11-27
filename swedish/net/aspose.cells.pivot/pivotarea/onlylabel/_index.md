---
title: "PivotArea.OnlyLabel"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotArea-egenskap. Anger om endast dataetiketter för ett objektval är markerade"
type: docs
url: /sv/net/aspose.cells.pivot/pivotarea/onlylabel/
---
## PivotArea.OnlyLabel property

Anger om endast datalabels för ett objektval är markerade.

```csharp
public bool OnlyLabel { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotAreaPropertyOnlyLabelDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Exempeldata
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(20);

            // Skapa pivottabell
            int pivotIndex = worksheet.PivotTables.Add("A1:B3", "D1", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Lägg till fält
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Konfigurera pivotområde
            PivotArea pivotArea = new PivotArea(pivotTable);
            pivotArea.AxisType = PivotFieldType.Row;
            pivotArea.OnlyLabel = true; // Key property demonstration
            
            // Tillämpa urval
            pivotArea.Select(PivotFieldType.Row, 0, PivotTableSelectionType.LabelOnly);

            workbook.Save("PivotAreaOnlyLabelDemo.xlsx");
        }
    }
}
```

### Se även

* class [PivotArea](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


