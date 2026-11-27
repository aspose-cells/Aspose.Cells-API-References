---
title: "ChartDataTable.Font"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ChartDataTable-egenskap. Hämtar ett Font-objekt som representerar teckensnittinställningen för den angivna diagramdatatabellen"
type: docs
url: /sv/net/aspose.cells.charts/chartdatatable/font/
---
## ChartDataTable.Font property

Hämtar ett `Font`-objekt som representerar teckensnittinställningen för den angivna diagramdatatabellen.

```csharp
public Font Font { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class ChartDataTablePropertyFontDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata för diagrammet
            worksheet.Cells["A1"].PutValue("Item");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["B1"].PutValue("Quantity");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(15);

            // Lägg till ett diagram
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Ställ in diagramdatakälla
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";

            // Aktivera datatabell
            chart.ShowDataTable = true;
            
            // Hämta datatabellobjektet
            ChartDataTable dataTable = chart.ChartDataTable;
            
            // Anpassa datatabellens teckensnitt
            dataTable.Font.Size = 14;
            dataTable.Font.Color = Color.Red;
            dataTable.Font.IsBold = true;
            dataTable.Font.Name = "Arial";

            // Spara arbetsboken
            workbook.Save("ChartDataTableFontDemo.xlsx");
        }
    }
}
```

### Se även

* class [Font](../../../aspose.cells/font/)
* class [ChartDataTable](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


