---
title: "TilePicOption.ScaleY"
second_title: "Aspose.Cells för .NET API‑referens"
description: "TilePicOption-egenskap. Hämtar eller anger Y‑skalan för mosaikbild"
type: docs
url: /sv/net/aspose.cells.drawing/tilepicoption/scaley/
---
## TilePicOption.ScaleY property

Hämtar eller anger Y‑skalan för kakelbilden.

```csharp
public double ScaleY { get; set; }
```

### Exempel

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class TilePicOptionPropertyScaleYDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till ett diagram
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 5, 15, 15);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Ställ in texturfyllning med bild
            chart.ChartArea.Area.FillFormat.FillType = FillType.Texture;
            byte[] imageData = File.ReadAllBytes("example.png");
            chart.ChartArea.Area.FillFormat.TextureFill.ImageData = imageData;
            
            // Konfigurera kakelalternativ med ScaleY
            chart.ChartArea.Area.FillFormat.TextureFill.TilePicOption = new TilePicOption();
            chart.ChartArea.Area.FillFormat.TextureFill.TilePicOption.ScaleX = 50;
            chart.ChartArea.Area.FillFormat.TextureFill.TilePicOption.ScaleY = 50;
            
            // Spara arbetsboken
            workbook.Save("TilePicOptionScaleYDemo.xlsx");
        }
    }
}
```

### Se även

* class [TilePicOption](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


