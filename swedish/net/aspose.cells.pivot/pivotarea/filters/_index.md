---
title: "PivotArea.Filters"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotArea-egenskap. Hämtar alla filter för detta PivotArea"
type: docs
url: /sv/net/aspose.cells.pivot/pivotarea/filters/
---
## PivotArea.Filters property

Hämtar alla filter för detta PivotArea.

```csharp
public PivotAreaFilterCollection Filters { get; }
```

### Exempel

```csharp
using Aspose.Cells;
using Aspose.Cells.Pivot;
using System;

namespace AsposeCellsExamples
{
    public class PivotAreaPropertyFiltersDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet dataSheet = workbook.Worksheets[0];
            dataSheet.Name = "SalesData";
            
            // Skapa exempeldata
            dataSheet.Cells["A1"].PutValue("Category");
            dataSheet.Cells["B1"].PutValue("Revenue");
            dataSheet.Cells["A2"].PutValue("Electronics");
            dataSheet.Cells["B2"].PutValue(1500);
            dataSheet.Cells["A3"].PutValue("Furniture");
            dataSheet.Cells["B3"].PutValue(800);
            dataSheet.Cells["A4"].PutValue("Electronics");
            dataSheet.Cells["B4"].PutValue(2200);

            // Skapa pivottabell
            Worksheet pivotSheet = workbook.Worksheets.Add("PivotReport");
            int pivotIndex = pivotSheet.PivotTables.Add("A3", "SalesData!A1:B4", "RevenueAnalysis");
            PivotTable pivotTable = pivotSheet.PivotTables[pivotIndex];

            // Konfigurera radfält med delsummer
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            PivotField rowField = pivotTable.RowFields["Category"];
            rowField.IsAutoSubtotals = true;

            // Lägg till datafält
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Revenue");

            // Skapa pivotområde och välj fält
            PivotArea pivotArea = new PivotArea(pivotTable);
            pivotArea.SelectField(PivotFieldType.Data, "Sum of Revenue");
            pivotArea.SelectField(PivotFieldType.Row, "Category");

            // Demonstrera användning av Filters-egenskapen
            Console.WriteLine($"Filter count: {pivotArea.Filters.Count}");
            if (pivotArea.Filters.Count > 1)
            {
                bool hasAutomaticSubtotal = pivotArea.Filters[1].IsSubtotalSet(PivotFieldSubtotalType.Automatic);
                Console.WriteLine($"Row field has automatic subtotal: {hasAutomaticSubtotal}");
            }

            workbook.Save("PivotFiltersDemo.xlsx");
        }
    }
}
```

### Se även

* class [PivotAreaFilterCollection](../../pivotareafiltercollection/)
* class [PivotArea](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


