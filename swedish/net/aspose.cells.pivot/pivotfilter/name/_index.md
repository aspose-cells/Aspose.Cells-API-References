---
title: "PivotFilter.Name"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotFilter egenskap. Hämtar namnet på pivotfiltret"
type: docs
url: /sv/net/aspose.cells.pivot/pivotfilter/name/
---
## PivotFilter.Name property

Hämtar namnet på pivotfiltret.

```csharp
public string Name { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFilterPropertyNameDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook book = new Workbook();
            Worksheet sheet = book.Worksheets[0];
            Cells cells = sheet.Cells;

            // Fyll i kalkylbladet med exempeldata
            cells["A1"].Value = "Product";
            cells["A2"].Value = "Apple";
            cells["A3"].Value = "Banana";
            cells["A4"].Value = "Orange";
            cells["B1"].Value = "Sales";
            cells["B2"].Value = 100;
            cells["B3"].Value = 200;
            cells["B4"].Value = 300;

            // Lägg till en pivottabell
            PivotTableCollection pivots = sheet.PivotTables;
            int pivotIndex = pivots.Add("=Sheet1!A1:B4", "D1", "SalesPivot");
            PivotTable pivot = pivots[pivotIndex];
            pivot.AddFieldToArea(PivotFieldType.Row, "Product");
            pivot.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Lägg till och konfigurera ett pivotfilter
            int filterIndex = pivot.PivotFilters.Add(0, PivotFilterType.Count);
            PivotFilter filter = pivot.PivotFilters[filterIndex];
            filter.Name = "ProductFilter"; // Demonstrating Name property usage
            filter.AutoFilter.FilterTop10(0, false, false, 2);

            // Uppdatera och beräkna pivottdata
            pivot.RefreshData();
            pivot.CalculateData();

            // Spara arbetsboken
            book.Save("PivotFilterNameDemo.xlsx");
        }
    }
}
```

### Se även

* class [PivotFilter](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


