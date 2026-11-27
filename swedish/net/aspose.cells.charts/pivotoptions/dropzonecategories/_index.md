---
title: "PivotOptions.DropZoneCategories"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotOptions-egenskap. Anger om en kontroll för varje PivotTable-fält på PivotTable‑radaxeln i käll‑PivotTable visas i diagrammet när dropZonesVisible är satt till true"
type: docs
url: /sv/net/aspose.cells.charts/pivotoptions/dropzonecategories/
---
## PivotOptions.DropZoneCategories property

Anger om en kontroll för varje PivotTable‑fält på radaxeln i käll‑PivotTable visas i diagrammet när dropZonesVisible är satt till true.

```csharp
public bool DropZoneCategories { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class PivotOptionsPropertyDropZoneCategoriesDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Lägg till ett kalkylblad och lite exempeldata
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(20);
            
            // Lägg till ett diagram som använder pivotdata
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Åtkomst till pivotalternativ från diagrammet
            PivotOptions options = chart.PivotOptions;
            
            // Demonstrera egenskapen DropZoneCategories
            options.DropZoneCategories = true;
            Console.WriteLine("DropZoneCategories enabled: " + options.DropZoneCategories);
            
            // Spara arbetsboken
            workbook.Save("PivotOptionsDemo.xlsx");
        }
    }
}
```

### Se även

* class [PivotOptions](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


