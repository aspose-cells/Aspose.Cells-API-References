---
title: "FillFormat.GradientStyle"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà FillFormat. Restituisce lo stile di gradiente per il riempimento specificato"
type: docs
url: /it/net/aspose.cells.drawing/fillformat/gradientstyle/
---
## FillFormat.GradientStyle property

Restituisce lo stile del gradiente per il riempimento specificato.

```csharp
public GradientStyleType GradientStyle { get; }
```

### Esempi

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
            
            // Crea un grafico e ottieni la sua area del grafico
            int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 5, 15, 15);
            Chart chart = sheet.Charts[chartIndex];
            ChartArea chartArea = chart.ChartArea;
            
            // Imposta lo stile di riempimento a gradiente
            chartArea.Area.FillFormat.SetPresetColorGradient(GradientPresetType.CalmWater, GradientStyleType.Vertical, 2);
            
            // Dimostra l'uso della proprietà GradientStyle
            Console.WriteLine("Gradient Style: " + chartArea.Area.FillFormat.GradientStyle);
            
            // Salva la cartella di lavoro
            workbook.Save("FillFormatPropertyGradientStyleDemo_out.xlsx");
        }
    }
}
```

### Vedi anche

* enum [GradientStyleType](../../gradientstyletype/)
* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


