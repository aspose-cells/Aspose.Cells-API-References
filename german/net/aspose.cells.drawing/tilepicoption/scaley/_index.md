---
title: "TilePicOption.ScaleY"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "TilePicOption-Eigenschaft. Liest oder setzt die Y‑Skalierung für das Kachelbild"
type: docs
url: /de/net/aspose.cells.drawing/tilepicoption/scaley/
---
## TilePicOption.ScaleY property

Liest oder setzt die Y‑Skalierung für das Kachelbild.

```csharp
public double ScaleY { get; set; }
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
    public class TilePicOptionPropertyScaleYDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Füge ein Diagramm hinzu
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 5, 15, 15);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Setze Texturfüllung mit Bild
            chart.ChartArea.Area.FillFormat.FillType = FillType.Texture;
            byte[] imageData = File.ReadAllBytes("example.png");
            chart.ChartArea.Area.FillFormat.TextureFill.ImageData = imageData;
            
            // Konfiguriere Kacheloptionen mit ScaleY
            chart.ChartArea.Area.FillFormat.TextureFill.TilePicOption = new TilePicOption();
            chart.ChartArea.Area.FillFormat.TextureFill.TilePicOption.ScaleX = 50;
            chart.ChartArea.Area.FillFormat.TextureFill.TilePicOption.ScaleY = 50;
            
            // Speichere die Arbeitsmappe
            workbook.Save("TilePicOptionScaleYDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [TilePicOption](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


