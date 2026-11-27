---
title: "TilePicOption.ScaleX"
second_title: "Aspose.Cells för .NET API‑referens"
description: "TilePicOption-egenskap. Hämtar eller anger X-skalan för kaklad bild"
type: docs
url: /sv/net/aspose.cells.drawing/tilepicoption/scalex/
---
## TilePicOption.ScaleX property

Hämtar eller anger X‑skalan för kakelbilden.

```csharp
public double ScaleX { get; set; }
```

### Exempel

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class TilePicOptionPropertyScaleXDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata och skapa ett diagram
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:A3", true);

            // Ställ in texturfyllning med bild
            string imagePath = Path.Combine(Environment.GetFolderPath(Environment.SpecialFolder.Desktop), "texture.png");
            byte[] imageData = File.ReadAllBytes(imagePath);
            
            chart.ChartArea.Area.FillFormat.FillType = FillType.Texture;
            chart.ChartArea.Area.FillFormat.TextureFill.ImageData = imageData;
            chart.ChartArea.Area.FillFormat.TextureFill.TilePicOption = new TilePicOption();
            
            // Demonstrera ScaleX-egenskapen
            chart.ChartArea.Area.FillFormat.TextureFill.TilePicOption.ScaleX = 50; // 50% horizontal scaling
            chart.ChartArea.Area.FillFormat.TextureFill.TilePicOption.ScaleY = 75; // 75% vertical scaling

            // Spara arbetsboken
            workbook.Save(Path.Combine(Environment.GetFolderPath(Environment.SpecialFolder.Desktop), "ScaleXDemo.xlsx"));
        }
    }
}
```

### Se även

* class [TilePicOption](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


