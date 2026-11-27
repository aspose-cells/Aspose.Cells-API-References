---
title: "ChartDataTable.AutoScaleFont"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ChartDataTable‑egenskap. Sant om texten i objektet ändrar teckenstorlek när objektets storlek ändras. Standardvärdet är Sant"
type: docs
url: /sv/net/aspose.cells.charts/chartdatatable/autoscalefont/
---
## ChartDataTable.AutoScaleFont property

Sant om texten i objektet ändrar teckenstorlek när objektets storlek ändras. Standardvärdet är Sant.

```csharp
public bool AutoScaleFont { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartDataTablePropertyAutoScaleFontDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata för diagrammet
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Lägg till ett diagram
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Ställ in diagramdatakälla
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Aktivera datatabell
            chart.ShowDataTable = true;
            
            // Kom åt diagrammets datatabells egenskaper
            // Korrekt sätt att hämta ChartDataTable när ShowDataTable är sant
            ChartDataTable dataTable = chart.ChartDataTable;
            
            // Demonstrera egenskapen AutoScaleFont
            dataTable.AutoScaleFont = false; // Disable auto-scaling
            Console.WriteLine("AutoScaleFont (false): " + dataTable.AutoScaleFont);
            
            dataTable.AutoScaleFont = true; // Enable auto-scaling
            Console.WriteLine("AutoScaleFont (true): " + dataTable.AutoScaleFont);

            // Spara arbetsboken
            workbook.Save("ChartDataTableAutoScaleFontDemo.xlsx");
        }
    }
}
```

### Se även

* class [ChartDataTable](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


