---
title: "PivotFilter.Value1"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotFilter egenskap. Hämtar strängvärdet value1 för etikettpivotfiltret"
type: docs
url: /sv/net/aspose.cells.pivot/pivotfilter/value1/
---
## PivotFilter.Value1 property

Hämtar strängvärdet1 för etikettpivotfiltret.

```csharp
public string Value1 { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFilterPropertyValue1Demo
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
            cells["B2"].Value = 1000;
            cells["B3"].Value = 2000;
            cells["B4"].Value = 3000;

            // Lägg till en pivottabell
            PivotTableCollection pivots = sheet.PivotTables;
            int pivotIndex = pivots.Add("=Sheet1!A1:B4", "D1", "SalesPivot");
            PivotTable pivot = pivots[pivotIndex];
            pivot.AddFieldToArea(PivotFieldType.Row, "Product");
            pivot.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Lägg till ett pivotfilter och ange Value1
            int filterIndex = pivot.PivotFilters.Add(0, PivotFilterType.CaptionEqual);
            PivotFilter filter = pivot.PivotFilters[filterIndex];
            filter.Value1 = "Apple"; // Filter for Apple products only

            // Uppdatera och beräkna data
            pivot.RefreshData();
            pivot.CalculateData();

            // Spara arbetsboken
            book.Save("PivotFilterValue1Demo.xlsx");
        }
    }
}
```

### Se även

* class [PivotFilter](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


