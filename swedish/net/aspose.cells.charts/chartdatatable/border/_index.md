---
title: "ChartDataTable.Border"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ChartDataTable‑egenskap. Returnerar ett Border‑objekt som representerar objektets kant"
type: docs
url: /sv/net/aspose.cells.charts/chartdatatable/border/
---
## ChartDataTable.Border property

Returnerar ett Border-objekt som representerar objektets ram

```csharp
public Line Border { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class ChartDataTablePropertyBorderDemo
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

            // Lägg till ett stapeldiagram
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Ange diagrammets dataområde
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Visa datatabell
            chart.ShowDataTable = true;
            ChartDataTable dataTable = chart.ChartDataTable;

            // Konfigurera kantegenskaper
            Line border = dataTable.Border;
            border.Color = System.Drawing.Color.Blue;
            border.Style = LineType.Solid;
            border.Weight = WeightType.MediumLine;
            border.DashType = MsoLineDashStyle.Solid;
            
            // Konfigurera synlighet för tabellkanter
            dataTable.HasHorizontalBorder = true;
            dataTable.HasVerticalBorder = true;
            dataTable.HasOutlineBorder = true;

            // Spara arbetsboken
            workbook.Save("ChartDataTableBorderDemo.xlsx");
        }
    }
}
```

### Se även

* class [Line](../../../aspose.cells.drawing/line/)
* class [ChartDataTable](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


