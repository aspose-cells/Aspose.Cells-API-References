---
title: "FillFormat.Pattern"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "FillFormat-Eigenschaft. Stellt ein Anzeigemuster für einen Bereich dar"
type: docs
url: /de/net/aspose.cells.drawing/fillformat/pattern/
---
## FillFormat.Pattern property

Stellt ein Anzeigemuster eines Bereichs dar.

```csharp
public FillPattern Pattern { get; set; }
```

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Fügen Sie Beispieldaten hinzu
            sheet.Cells["A1"].PutValue(50);
            sheet.Cells["A2"].PutValue(100);
            sheet.Cells["A3"].PutValue(150);

            // Füge ein Diagramm hinzu
            int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = sheet.Charts[chartIndex];
            
            // Diagrammdatenbereich festlegen
            chart.NSeries.Add("A1:A3", true);

            // Greife auf die erste Serie und deren ersten Punkt zu
            ChartPoint point = chart.NSeries[0].Points[0];
            
            // Füllmuster für den Bereich des Punktes festlegen
            point.Area.FillFormat.Pattern = FillPattern.DottedGrid;
            
            // Speichere die Arbeitsmappe
            workbook.Save("FillFormatPatternDemo.xlsx");
        }
    }
}
```

### Siehe auch

* enum [FillPattern](../../fillpattern/)
* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


