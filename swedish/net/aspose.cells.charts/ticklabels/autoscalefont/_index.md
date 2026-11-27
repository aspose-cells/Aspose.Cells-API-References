---
title: "TickLabels.AutoScaleFont"
second_title: "Aspose.Cells för .NET API‑referens"
description: "TickLabels-egenskap. Sant om texten i objektet ändrar teckenstorlek när objektets storlek ändras. Standardvärdet är Sant"
type: docs
url: /sv/net/aspose.cells.charts/ticklabels/autoscalefont/
---
## TickLabels.AutoScaleFont property

Sant om texten i objektet ändrar teckenstorlek när objektets storlek ändras. Standardvärdet är Sant.

```csharp
public bool AutoScaleFont { get; set; }
```

### Exempel

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class TickLabelsPropertyAutoScaleFontDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            Cells cells = sheet.Cells;

            // Exempeldata
            cells["A1"].PutValue("Region");
            cells["A2"].PutValue("France");
            cells["A3"].PutValue("Germany");
            cells["A4"].PutValue("England");
            cells["B1"].PutValue("Sales");
            cells["B2"].PutValue(100000);
            cells["B3"].PutValue(150000);
            cells["B4"].PutValue(90000);

            // Skapa diagram
            int chartIndex = sheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 1, 20, 10);
            Aspose.Cells.Charts.Chart chart = sheet.Charts[chartIndex];
            
            // Konfigurera diagramdata
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            
            // Konfigurera axelrubriker med AutoScaleFont
            chart.CategoryAxis.TickLabels.AutoScaleFont = true;
            chart.CategoryAxis.TickLabels.Font.Size = 12; // Initial size
            
            // Spara arbetsboken
            workbook.Save("TickLabelsAutoScaleFontDemo.xlsx");
        }
    }
}
```

### Se även

* class [TickLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


