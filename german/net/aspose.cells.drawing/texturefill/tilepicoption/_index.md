---
title: "TextureFill.TilePicOption"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "TextureFill-Eigenschaft. Ruft die Kachelbildoption ab oder legt sie fest"
type: docs
url: /de/net/aspose.cells.drawing/texturefill/tilepicoption/
---
## TextureFill.TilePicOption property

Liest oder setzt die Kachelbildoption.

```csharp
public TilePicOption TilePicOption { get; set; }
```

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge ein Diagramm hinzu
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 5, 15, 15);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];

            // Setze Texturfüllung mit Bild
            chart.ChartArea.Area.FillFormat.FillType = FillType.Texture;
            byte[] imageData = File.ReadAllBytes("texture.png");
            chart.ChartArea.Area.FillFormat.TextureFill.ImageData = imageData;

            // Kacheloptionen konfigurieren
            chart.ChartArea.Area.FillFormat.TextureFill.TilePicOption = new TilePicOption();
            chart.ChartArea.Area.FillFormat.TextureFill.TilePicOption.ScaleX = 50;
            chart.ChartArea.Area.FillFormat.TextureFill.TilePicOption.ScaleY = 50;
            chart.ChartArea.Area.FillFormat.TextureFill.TilePicOption.OffsetX = 10;
            chart.ChartArea.Area.FillFormat.TextureFill.TilePicOption.OffsetY = 10;

            // Speichere die Arbeitsmappe
            workbook.Save("TextureFillDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [TilePicOption](../../tilepicoption/)
* class [TextureFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


