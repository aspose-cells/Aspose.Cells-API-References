---
title: "TextureFill.IsTiling"
second_title: "Aspose.Cells för .NET API‑referens"
description: "TextureFill-egenskap. Anger om bilden ska tileas som textur"
type: docs
url: /sv/net/aspose.cells.drawing/texturefill/istiling/
---
## TextureFill.IsTiling property

Anger om bilden ska tileas som textur.

```csharp
public bool IsTiling { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class TextureFillPropertyIsTilingDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första arbetsbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till ett diagram
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Ange diagramdata
            chart.NSeries.Add("A1:B3", true);
            
            // Ställ in texturfyllning för diagramområdet
            chart.PlotArea.Area.FillFormat.Texture = TextureType.BlueTissuePaper;
            
            // Ställ in IsTiling-egenskapen
            chart.PlotArea.Area.FillFormat.TextureFill.IsTiling = true;
            
            // Verifiera och skriv ut IsTiling-värdet
            Console.WriteLine("IsTiling: " + chart.PlotArea.Area.FillFormat.TextureFill.IsTiling);
            
            // Spara arbetsboken
            workbook.Save("TextureFillIsTilingDemo.xlsx");
        }
    }
}
```

### Se även

* class [TextureFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


