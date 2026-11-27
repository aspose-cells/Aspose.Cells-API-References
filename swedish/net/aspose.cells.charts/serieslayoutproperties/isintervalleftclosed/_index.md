---
title: "SeriesLayoutProperties.IsIntervalLeftClosed"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SeriesLayoutProperties-egenskap. Anger om intervallet är stängt på vänster sida"
type: docs
url: /sv/net/aspose.cells.charts/serieslayoutproperties/isintervalleftclosed/
---
## SeriesLayoutProperties.IsIntervalLeftClosed property

Anger om intervallet är stängt på vänster sida.

```csharp
public bool IsIntervalLeftClosed { get; set; }
```

### Anmärkningar

Endast för ParetoLine-diagram.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesLayoutPropertiesPropertyIsIntervalLeftClosedDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            worksheet.Cells["B1"].PutValue(15);
            worksheet.Cells["B2"].PutValue(25);
            worksheet.Cells["B3"].PutValue(35);

            // Skapa diagram
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            int seriesIndex = chart.NSeries.Add("A1:B3", true);
            Aspose.Cells.Charts.Series series = chart.NSeries[seriesIndex];

            // Ställ in egenskapen IsIntervalLeftClosed
            series.LayoutProperties.IsIntervalLeftClosed = true;

            // Spara arbetsbok
            workbook.Save("SeriesLayoutPropertiesIsIntervalLeftClosedDemo.xlsx");
        }
    }
}
```

### Se även

* class [SeriesLayoutProperties](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


