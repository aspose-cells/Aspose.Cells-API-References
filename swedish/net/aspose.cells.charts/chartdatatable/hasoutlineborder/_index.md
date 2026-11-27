---
title: "ChartDataTable.HasOutlineBorder"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ChartDataTable-egenskap. Sant om diagrammets datatabell har konturkanter"
type: docs
url: /sv/net/aspose.cells.charts/chartdatatable/hasoutlineborder/
---
## ChartDataTable.HasOutlineBorder property

Sant om diagramdatatabellen har konturramar

```csharp
public bool HasOutlineBorder { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartDataTablePropertyHasOutlineBorderDemo
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

            // Visa datatabell och hämta ChartDataTable-objektet
            chart.ShowDataTable = true;
            ChartDataTable dataTable = chart.ChartDataTable;

            // Demonstrera HasOutlineBorder-egenskapen
            dataTable.HasOutlineBorder = true; // Enable outline border
            Console.WriteLine("DataTable HasOutlineBorder: " + dataTable.HasOutlineBorder);

            // Spara arbetsboken
            workbook.Save("ChartDataTableHasOutlineBorderDemo.xlsx");
        }
    }
}
```

### Se även

* class [ChartDataTable](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


