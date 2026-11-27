---
title: "Series.Has3DEffect"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Series‑egenskap. Sant om serien har ett tredimensionellt utseende"
type: docs
url: /sv/net/aspose.cells.charts/series/has3deffect/
---
## Series.Has3DEffect property

Sant om serien har ett tredimensionellt utseende.

```csharp
public bool Has3DEffect { get; set; }
```

### Anmärkningar

Gäller endast för Bubble‑ eller Bubble3D‑diagram.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertyHas3DEffectDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

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

            // Lägg till ett diagram
            int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Lägg till serie
            int seriesIndex = chart.NSeries.Add("A1:B3", true);
            chart.NSeries.CategoryData = "C1:C3";
            
            // Hämta serien och ange 3D‑effekt
            Series series = chart.NSeries[seriesIndex];
            series.Has3DEffect = true;
            series.Bar3DShapeType = Bar3DShapeType.Cylinder;

            // Spara arbetsboken
            workbook.Save("Series3DEffectDemo.xlsx");
        }
    }
}
```

### Se även

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


