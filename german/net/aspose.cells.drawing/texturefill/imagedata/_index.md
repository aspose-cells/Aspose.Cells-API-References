---
title: "TextureFill.ImageData"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "TextureFill-Eigenschaft. Ruft die Bilddaten der Füllung ab oder legt sie fest"
type: docs
url: /de/net/aspose.cells.drawing/texturefill/imagedata/
---
## TextureFill.ImageData property

Liest und setzt die Bilddaten der Füllung.

```csharp
public byte[] ImageData { get; set; }
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
    public class TextureFillPropertyImageDataDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge ein Diagramm hinzu
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 5, 15, 15);
            Chart chart = worksheet.Charts[chartIndex];

            // Texturfülltyp festlegen
            chart.ChartArea.Area.FillFormat.FillType = FillType.Texture;

            // Bilddaten laden
            byte[] imageData = File.ReadAllBytes("texture.png");

            // Bilddaten für die Texturfüllung festlegen
            chart.ChartArea.Area.FillFormat.TextureFill.ImageData = imageData;

            // Speichere die Arbeitsmappe
            workbook.Save("TextureFillDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [TextureFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


