---
title: "PatternFill.Pattern"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PatternFill-egenskap. Hämtar eller anger fyllningsmönstertyp"
type: docs
url: /sv/net/aspose.cells.drawing/patternfill/pattern/
---
## PatternFill.Pattern property

Hämtar eller anger fyllningsmönster-typen

```csharp
public FillPattern Pattern { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class PatternFillPropertyPatternDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första arbetsbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till ett diagram
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Lägg till exempeldata för diagrammet
            worksheet.Cells["A1"].PutValue("Item");
            worksheet.Cells["A2"].PutValue("Product A");
            worksheet.Cells["A3"].PutValue("Product B");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(200);
            
            // Ange diagrammets dataområde
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";
            
            // Ange fyllningsmönster för den första serien
            chart.NSeries[0].Area.FillFormat.FillType = FillType.Pattern;
            chart.NSeries[0].Area.FillFormat.PatternFill.Pattern = FillPattern.WideDownwardDiagonal;
            
            // Spara arbetsboken
            workbook.Save("PatternFillDemo.xlsx");
        }
    }
}
```

### Se även

* enum [FillPattern](../../fillpattern/)
* class [PatternFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


