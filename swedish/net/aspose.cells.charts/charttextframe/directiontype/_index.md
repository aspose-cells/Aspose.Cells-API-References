---
title: "ChartTextFrame.DirectionType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ChartTextFrame-egenskap. Hämtar och anger textens riktning"
type: docs
url: /sv/net/aspose.cells.charts/charttextframe/directiontype/
---
## ChartTextFrame.DirectionType property

Hämtar och anger textens riktning.

```csharp
public virtual ChartTextDirectionType DirectionType { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartTextFramePropertyDirectionTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            // När du lägger till ett kalkylblad returneras dess index, sedan hämtar vi kalkylbladet med indexet
            int sheetIndex = workbook.Worksheets.Add();
            Worksheet worksheet = workbook.Worksheets[sheetIndex];
            
            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["B3"].PutValue(50);
            worksheet.Cells["C1"].PutValue("Q1");
            worksheet.Cells["C2"].PutValue("Q2");
            worksheet.Cells["C3"].PutValue("Q3");

            // Lägg till diagram
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:B3", true);
            chart.NSeries.CategoryData = "C1:C3";

            // Kom åt och konfigurera titel
            ChartTextFrame title = chart.Title;
            title.Text = "Sample Chart";
            
            // Demonstrera egenskapen DirectionType
            title.DirectionType = ChartTextDirectionType.Vertical;
            
            // Spara arbetsboken
            workbook.Save("ChartTextDirectionDemo.xlsx");
        }
    }
}
```

### Se även

* enum [ChartTextDirectionType](../../charttextdirectiontype/)
* class [ChartTextFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


