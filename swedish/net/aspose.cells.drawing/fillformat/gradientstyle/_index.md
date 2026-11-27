---
title: "FillFormat.GradientStyle"
second_title: "Aspose.Cells för .NET API‑referens"
description: "FillFormat-egenskap. Returnerar gradientstilen för den angivna fyllningen"
type: docs
url: /sv/net/aspose.cells.drawing/fillformat/gradientstyle/
---
## FillFormat.GradientStyle property

Returnerar gradientstilen för den angivna fyllningen.

```csharp
public GradientStyleType GradientStyle { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class FillFormatPropertyGradientStyleDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Skapa ett diagram och hämta dess diagramområde
            int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 5, 15, 15);
            Chart chart = sheet.Charts[chartIndex];
            ChartArea chartArea = chart.ChartArea;
            
            // Ställ in gradientfyllningsstil
            chartArea.Area.FillFormat.SetPresetColorGradient(GradientPresetType.CalmWater, GradientStyleType.Vertical, 2);
            
            // Visa hur GradientStyle-egenskapen används
            Console.WriteLine("Gradient Style: " + chartArea.Area.FillFormat.GradientStyle);
            
            // Spara arbetsboken
            workbook.Save("FillFormatPropertyGradientStyleDemo_out.xlsx");
        }
    }
}
```

### Se även

* enum [GradientStyleType](../../gradientstyletype/)
* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


