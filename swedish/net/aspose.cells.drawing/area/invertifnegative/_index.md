---
title: "Area.InvertIfNegative"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Area-egenskap. Om egenskapen är sann och värdet för diagrampunkten är ett negativt tal kommer förgrundsfärgen och bakgrundsfärgen att bytas."
type: docs
url: /sv/net/aspose.cells.drawing/area/invertifnegative/
---
## Area.InvertIfNegative property

Om egenskapen är sann och värdet för diagrampunkten är ett negativt tal, kommer förgrundsfärgen och bakgrundsfärgen att bytas ut.

```csharp
public bool InvertIfNegative { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class AreaPropertyInvertIfNegativeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata med negativt värde
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(-100);
            worksheet.Cells["A3"].PutValue(150);
            
            // Lägg till stapeldiagram
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Lägg till dataserier och konfigurera områdesegenskaper
            chart.NSeries.Add("A1:A3", true);
            chart.NSeries[0].Area.InvertIfNegative = true;
            chart.NSeries[0].Area.ForegroundColor = Color.Red;
            chart.NSeries[0].Area.BackgroundColor = Color.Yellow;
            
            workbook.Save("AreaPropertyInvertIfNegativeDemo.xls");
        }
    }
}
```

### Se även

* class [Area](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


