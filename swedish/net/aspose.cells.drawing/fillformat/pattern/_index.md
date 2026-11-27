---
title: "FillFormat.Pattern"
second_title: "Aspose.Cells för .NET API‑referens"
description: "FillFormat-egenskap. Representerar ett områdes visningsmönster"
type: docs
url: /sv/net/aspose.cells.drawing/fillformat/pattern/
---
## FillFormat.Pattern property

Representerar ett områdes displaymönster.

```csharp
public FillPattern Pattern { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class FillFormatPropertyPatternDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Lägg till exempeldata
            sheet.Cells["A1"].PutValue(50);
            sheet.Cells["A2"].PutValue(100);
            sheet.Cells["A3"].PutValue(150);

            // Lägg till ett diagram
            int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = sheet.Charts[chartIndex];
            
            // Ange diagrammets dataområde
            chart.NSeries.Add("A1:A3", true);

            // Få åtkomst till den första serien och dess första punkt
            ChartPoint point = chart.NSeries[0].Points[0];
            
            // Ställ in fyllningsmönster för punktens område
            point.Area.FillFormat.Pattern = FillPattern.DottedGrid;
            
            // Spara arbetsboken
            workbook.Save("FillFormatPatternDemo.xlsx");
        }
    }
}
```

### Se även

* enum [FillPattern](../../fillpattern/)
* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


