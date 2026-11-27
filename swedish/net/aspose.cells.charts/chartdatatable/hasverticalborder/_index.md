---
title: "ChartDataTable.HasVerticalBorder"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ChartDataTable-egenskap. True om diagrammets datatabell har vertikala cellramar"
type: docs
url: /sv/net/aspose.cells.charts/chartdatatable/hasverticalborder/
---
## ChartDataTable.HasVerticalBorder property

Sant om diagramdatatabellen har vertikala cellramar

```csharp
public bool HasVerticalBorder { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartDataTablePropertyHasVerticalBorderDemo
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

            // Visa datatabell
            chart.ShowDataTable = true;
            
            // Kom åt datatabellen via ChartDataTable‑egenskapen
            ChartDataTable dataTable = chart.ChartDataTable;

            // Demonstrera HasVerticalBorder‑egenskapen
            Console.WriteLine("Initial HasVerticalBorder value: " + dataTable.HasVerticalBorder);
            
            // Växla vertikala kanter
            dataTable.HasVerticalBorder = true;
            Console.WriteLine("After setting HasVerticalBorder to true: " + dataTable.HasVerticalBorder);
            
            dataTable.HasVerticalBorder = false;
            Console.WriteLine("After setting HasVerticalBorder to false: " + dataTable.HasVerticalBorder);

            // Spara arbetsboken
            workbook.Save("ChartDataTable_HasVerticalBorderDemo.xlsx");
        }
    }
}
```

### Se även

* class [ChartDataTable](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


