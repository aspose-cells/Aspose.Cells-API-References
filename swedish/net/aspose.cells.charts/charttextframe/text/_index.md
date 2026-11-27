---
title: "ChartTextFrame.Text"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ChartTextFrame-egenskap. Hämtar eller anger texten för en ramtitel"
type: docs
url: /sv/net/aspose.cells.charts/charttextframe/text/
---
## ChartTextFrame.Text property

Hämtar eller anger texten för ramens titel.

```csharp
public virtual string Text { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartTextFramePropertyTextDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Lägg till exempeldata
            Cells cells = sheet.Cells;
            cells["A1"].PutValue("Category");
            cells["A2"].PutValue("A");
            cells["A3"].PutValue("B");
            cells["A4"].PutValue("C");
            cells["B1"].PutValue("Value");
            cells["B2"].PutValue(10);
            cells["B3"].PutValue(20);
            cells["B4"].PutValue(30);

            // Lägg till diagram
            int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = sheet.Charts[chartIndex];
            chart.SetChartDataRange("A1:B4", true);

            // Ställ in diagramrubrikens text
            chart.Title.Text = "Sample Chart Title";

            // Åtkomst till och ändra förklaringstext
            Legend legend = chart.Legend;
            legend.Text = "Custom Legend Text";

            // Spara arbetsboken
            workbook.Save("ChartTextDemo.xlsx");
        }
    }
}
```

### Se även

* class [ChartTextFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


