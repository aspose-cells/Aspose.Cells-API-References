---
title: "ChartTextFrame.LinkedSource"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ChartTextFrame-egenskap. Hämtar och anger en referens till arbetsbladet"
type: docs
url: /sv/net/aspose.cells.charts/charttextframe/linkedsource/
---
## ChartTextFrame.LinkedSource property

Hämtar och anger en referens till arbetsbladet.

```csharp
public virtual string LinkedSource { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartTextFramePropertyLinkedSourceDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första arbetsbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata
            worksheet.Cells["P1"].PutValue("Chart Title");
            
            // Lägg till diagram
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Ställ in diagramrubrik och länka den till cell P1
            chart.Title.Text = "Linked Title";
            chart.Title.LinkedSource = "='" + worksheet.Name + "'!$P$1";
            
            // Spara arbetsboken
            workbook.Save("output.xlsx");
            
            // Verifiera den länkade källan
            Console.WriteLine("Chart Title Linked Source: " + chart.Title.LinkedSource);
        }
    }
}
```

### Se även

* class [ChartTextFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


