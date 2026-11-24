---
title: "FillFormat.GradientStyle"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "FillFormat-Eigenschaft. Gibt den Farbverlaufstil für die angegebene Füllung zurück"
type: docs
url: /de/net/aspose.cells.drawing/fillformat/gradientstyle/
---
## FillFormat.GradientStyle property

Gibt den Farbverlaufsstil für die angegebene Füllung zurück.

```csharp
public GradientStyleType GradientStyle { get; }
```

### Beispiele

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
            
            // Erstelle ein Diagramm und rufe dessen Diagrammbereich ab
            int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 5, 15, 15);
            Chart chart = sheet.Charts[chartIndex];
            ChartArea chartArea = chart.ChartArea;
            
            // Setze den Farbverlauf-Füllstil
            chartArea.Area.FillFormat.SetPresetColorGradient(GradientPresetType.CalmWater, GradientStyleType.Vertical, 2);
            
            // Demonstriere die Verwendung der GradientStyle-Eigenschaft
            Console.WriteLine("Gradient Style: " + chartArea.Area.FillFormat.GradientStyle);
            
            // Speichere die Arbeitsmappe
            workbook.Save("FillFormatPropertyGradientStyleDemo_out.xlsx");
        }
    }
}
```

### Siehe auch

* enum [GradientStyleType](../../gradientstyletype/)
* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


