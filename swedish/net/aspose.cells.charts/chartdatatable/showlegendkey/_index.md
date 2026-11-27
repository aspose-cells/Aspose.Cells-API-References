---
title: "ChartDataTable.ShowLegendKey"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ChartDataTable‑egenskap. Sant om legendnyckeln för datalabeln är synlig"
type: docs
url: /sv/net/aspose.cells.charts/chartdatatable/showlegendkey/
---
## ChartDataTable.ShowLegendKey property

Sant om nyckeln för datalabellegenden är synlig.

```csharp
public bool ShowLegendKey { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartDataTablePropertyShowLegendKeyDemo
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
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Ställ in diagramdatakälla
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Aktivera datatabell med legendnyckel
            chart.ShowDataTable = true;
            // Kom åt DataTable via diagrammets egenskaper
            if (chart.ChartDataTable != null)
            {
                chart.ChartDataTable.ShowLegendKey = true;
            }

            // Spara arbetsboken
            workbook.Save("ChartDataTableShowLegendKeyDemo.xlsx");

            Console.WriteLine("Chart created with ShowLegendKey enabled in data table.");
        }
    }
}
```

### Se även

* class [ChartDataTable](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


