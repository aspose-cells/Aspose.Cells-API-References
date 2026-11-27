---
title: "ChartTextFrame.TextVerticalAlignment"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ChartTextFrame-egenskap. Hämtar eller anger den vertikala justeringen av text"
type: docs
url: /sv/net/aspose.cells.charts/charttextframe/textverticalalignment/
---
## ChartTextFrame.TextVerticalAlignment property

Hämtar och anger vertikal justering av texten.

```csharp
public TextAlignmentType TextVerticalAlignment { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartTextFramePropertyTextVerticalAlignmentDemo
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
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];
            chart.SetChartDataRange("A1:B4", true);

            // Ställ in titeln och konfigurera vertikal justering
            chart.Title.Text = "Sample Chart";
            chart.Title.TextVerticalAlignment = TextAlignmentType.Top;

            // Konfigurera visningsenhetsetiketten
            chart.ValueAxis.DisplayUnit = DisplayUnitType.Hundreds;
            chart.ValueAxis.DisplayUnitLabel.Text = "Values in Hundreds";
            chart.ValueAxis.DisplayUnitLabel.TextVerticalAlignment = TextAlignmentType.Center;

            // Spara arbetsboken
            workbook.Save("ChartTextVerticalAlignmentDemo.xlsx");

            Console.WriteLine("Demo executed successfully. Output file: ChartTextVerticalAlignmentDemo.xlsx");
        }
    }
}
```

### Se även

* enum [TextAlignmentType](../../../aspose.cells/textalignmenttype/)
* class [ChartTextFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


