---
title: "Axis.Title"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Axis‑egenskap. Hämtar titeln för denna axel i diagrammet"
type: docs
url: /sv/net/aspose.cells.charts/axis/title/
---
## Axis.Title property

Hämtar titeln för denna axel i diagrammet.

```csharp
public Title Title { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class AxisPropertyTitleDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(20);
            
            // Lägg till ett diagram
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Ange diagrammets dataområde
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";
            
            // Konfigurera titlar
            chart.Title.Text = "Sample Chart";
            chart.Title.IsVisible = true;
            chart.Title.Font.Name = "Arial";
            chart.Title.Font.Size = 14;
            
            // Konfigurera axeltitlar
            chart.CategoryAxis.Title.Text = "Categories";
            chart.CategoryAxis.Title.IsVisible = true;
            chart.CategoryAxis.Title.Font.Name = "Arial";
            
            chart.ValueAxis.Title.Text = "Values";
            chart.ValueAxis.Title.IsVisible = true;
            chart.ValueAxis.Title.Font.Name = "Arial";
            
            // Spara arbetsboken
            workbook.Save("AxisPropertyTitleDemo_Output.xlsx");
        }
    }
}
```

### Se även

* class [Title](../../title/)
* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


