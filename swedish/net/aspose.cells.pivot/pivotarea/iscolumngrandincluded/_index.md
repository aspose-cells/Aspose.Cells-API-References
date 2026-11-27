---
title: "PivotArea.IsColumnGrandIncluded"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotArea-egenskap. Anger om kolumnens totalsumma är inkluderad"
type: docs
url: /sv/net/aspose.cells.pivot/pivotarea/iscolumngrandincluded/
---
## PivotArea.IsColumnGrandIncluded property

Anger om kolumnens totalsumma är inkluderad.

```csharp
public bool IsColumnGrandIncluded { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotAreaPropertyIsColumnGrandIncludedDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Exempeldata
            worksheet.Cells["A1"].Value = "Category";
            worksheet.Cells["A2"].Value = "Fruit";
            worksheet.Cells["A3"].Value = "Vegetable";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 100;
            worksheet.Cells["B3"].Value = 150;

            // Skapa pivottabell
            int pivotIndex = worksheet.PivotTables.Add("=Sheet1!A1:B3", "E5", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Lägg till fält
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Konfigurera pivotområde
            PivotArea pivotArea = new PivotArea(pivotTable);
            pivotArea.IsColumnGrandIncluded = true; // Demonstrate property usage
            pivotArea.IsRowGrandIncluded = true;
            pivotArea.RuleType = PivotAreaType.Normal;

            // Spara arbetsboken
            workbook.Save("PivotAreaIsColumnGrandIncludedDemo.xlsx");
        }
    }
}
```

### Se även

* class [PivotArea](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


