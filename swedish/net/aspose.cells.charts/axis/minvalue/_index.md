---
title: "Axis.MinValue"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Axis egenskap. Representerar minsta värdet på värdeaxeln"
type: docs
url: /sv/net/aspose.cells.charts/axis/minvalue/
---
## Axis.MinValue property

Anger det minsta värdet på värdeaxeln.

```csharp
public object MinValue { get; set; }
```

### Anmärkningar

Typen minValue kan endast vara double eller DateTime

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class AxisPropertyMinValueDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första kalkylbladet och lägg till exempeldata
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            worksheet.Cells["B1"].PutValue(40);
            worksheet.Cells["B2"].PutValue(50);
            worksheet.Cells["B3"].PutValue(60);

            // Lägg till ett diagram och ange dataintervall
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 5, 15, 15);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            chart.SetChartDataRange("A1:B3", false);

            // Konfigurera värdeaxelns egenskaper
            chart.ValueAxis.MinValue = 15;  // Setting minimum value
            chart.ValueAxis.MaxValue = 70;
            chart.ValueAxis.MajorUnit = 10;

            // Spara arbetsboken
            workbook.Save("AxisMinValueDemo.xlsx");

            Console.WriteLine("Chart created with MinValue set to 15.");
        }
    }
}
```

### Se även

* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


