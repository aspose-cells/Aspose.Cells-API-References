---
title: "PivotArea.OnlyData"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotArea-egenskap. Anger om endast datavärdena i dataområdet i vyn för ett objektval är markerade och inte inkluderar objektetiketterna"
type: docs
url: /sv/net/aspose.cells.pivot/pivotarea/onlydata/
---
## PivotArea.OnlyData property

Anger om endast datavärdena (i dataområdet i vyn) för ett objektval är markerade och inte inkluderar objektetiketterna.

```csharp
public bool OnlyData { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotAreaPropertyOnlyDataDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Electronics");
            worksheet.Cells["A3"].PutValue("Clothing");
            worksheet.Cells["A4"].PutValue("Food");
            
            worksheet.Cells["B1"].PutValue("Revenue");
            worksheet.Cells["B2"].PutValue(5000);
            worksheet.Cells["B3"].PutValue(3000);
            worksheet.Cells["B4"].PutValue(2000);

            // Skapa pivottabell
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "D1", "SalesPivot");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Lägg till fält
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Konfigurera pivotområde
            PivotArea pivotArea = new PivotArea(pivotTable);
            pivotArea.RuleType = PivotAreaType.Normal;
            pivotArea.OnlyData = true; // Key property demonstration
            pivotArea.IsRowGrandIncluded = false;

            // Utdata-konfiguration
            Console.WriteLine("OnlyData property is set to: " + pivotArea.OnlyData);
            
            workbook.Save("PivotAreaOnlyDataDemo.xlsx");
        }
    }
}
```

### Se även

* class [PivotArea](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


