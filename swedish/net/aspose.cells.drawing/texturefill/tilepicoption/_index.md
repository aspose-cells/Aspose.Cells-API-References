---
title: "TextureFill.TilePicOption"
second_title: "Aspose.Cells för .NET API‑referens"
description: "TextureFill-egenskap. Hämtar eller anger alternativ för mosaikbild"
type: docs
url: /sv/net/aspose.cells.drawing/texturefill/tilepicoption/
---
## TextureFill.TilePicOption property

Hämtar eller anger alternativ för tile-bild.

```csharp
public TilePicOption TilePicOption { get; set; }
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
    public class TextureFillPropertyTilePicOptionDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till ett diagram
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 5, 15, 15);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];

            // Ställ in texturfyllning med bild
            chart.ChartArea.Area.FillFormat.FillType = FillType.Texture;
            byte[] imageData = File.ReadAllBytes("texture.png");
            chart.ChartArea.Area.FillFormat.TextureFill.ImageData = imageData;

            // Konfigurera mosaikalternativ
            chart.ChartArea.Area.FillFormat.TextureFill.TilePicOption = new TilePicOption();
            chart.ChartArea.Area.FillFormat.TextureFill.TilePicOption.ScaleX = 50;
            chart.ChartArea.Area.FillFormat.TextureFill.TilePicOption.ScaleY = 50;
            chart.ChartArea.Area.FillFormat.TextureFill.TilePicOption.OffsetX = 10;
            chart.ChartArea.Area.FillFormat.TextureFill.TilePicOption.OffsetY = 10;

            // Spara arbetsboken
            workbook.Save("TextureFillDemo.xlsx");
        }
    }
}
```

### Se även

* class [TilePicOption](../../tilepicoption/)
* class [TextureFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


