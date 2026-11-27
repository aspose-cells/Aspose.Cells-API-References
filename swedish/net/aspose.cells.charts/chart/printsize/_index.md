---
title: "Chart.PrintSize"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Chart-egenskap. Hämtar och anger den utskrivna diagramstorleken"
type: docs
url: /sv/net/aspose.cells.charts/chart/printsize/
---
## Chart.PrintSize property

Hämtar och anger den utskrivna diagramstorleken.

```csharp
public PrintSizeType PrintSize { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertyPrintSizeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata för diagrammet
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B4"].PutValue(30);

            // Lägg till ett diagram
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Ställ in diagramdatakälla
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Konfigurera utskriftsinställningar
            chart.PrintSize = PrintSizeType.Full;
            chart.SizeWithWindow = false;
            chart.AutoScaling = false;

            // Spara arbetsboken
            workbook.Save("ChartPrintSizeDemo.pdf", SaveFormat.Pdf);
        }
    }
}
```

### Se även

* enum [PrintSizeType](../../../aspose.cells/printsizetype/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


