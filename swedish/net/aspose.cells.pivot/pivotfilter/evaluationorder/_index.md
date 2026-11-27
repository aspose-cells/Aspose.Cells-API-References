---
title: "PivotFilter.EvaluationOrder"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotFilter-egenskap. Hämtar utvärderingsordningen för pivottfiltret"
type: docs
url: /sv/net/aspose.cells.pivot/pivotfilter/evaluationorder/
---
## PivotFilter.EvaluationOrder property

Hämtar utvärderingsordningen för pivotfiltret.

```csharp
public int EvaluationOrder { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFilterPropertyEvaluationOrderDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook book = new Workbook();
            Worksheet sheet = book.Worksheets[0];
            Cells cells = sheet.Cells;

            // Fyll i exempeldata
            cells["A1"].Value = "Category";
            cells["A2"].Value = "Fruit";
            cells["A3"].Value = "Vegetable";
            cells["A4"].Value = "Fruit";
            cells["A5"].Value = "Vegetable";
            
            cells["B1"].Value = "Sales";
            cells["B2"].Value = 100;
            cells["B3"].Value = 200;
            cells["B4"].Value = 300;
            cells["B5"].Value = 400;

            // Skapa pivottabell
            PivotTableCollection pivots = sheet.PivotTables;
            int pivotIndex = pivots.Add("=Sheet1!A1:B5", "D1", "PivotTable1");
            PivotTable pivot = pivots[pivotIndex];
            
            // Lägg till fält
            pivot.AddFieldToArea(PivotFieldType.Row, "Category");
            pivot.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Lägg till pivotfilter
            int filterIndex = pivot.PivotFilters.Add(0, PivotFilterType.Count);
            PivotFilter filter = pivot.PivotFilters[filterIndex];
            
            // Ställ in filteregenskaper inklusive EvaluationOrder
            filter.EvaluationOrder = 1;
            filter.AutoFilter.FilterTop10(0, false, false, 2);

            // Uppdatera pivottabell
            pivot.RefreshData();
            pivot.CalculateData();

            // Spara arbetsbok
            book.Save("PivotFilterEvaluationOrderDemo.xlsx");
        }
    }
}
```

### Se även

* class [PivotFilter](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


