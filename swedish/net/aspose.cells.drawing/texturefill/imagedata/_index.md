---
title: "TextureFill.ImageData"
second_title: "Aspose.Cells för .NET API‑referens"
description: "TextureFill-egenskap. Hämtar och anger bilddata för fyllningen"
type: docs
url: /sv/net/aspose.cells.drawing/texturefill/imagedata/
---
## TextureFill.ImageData property

Hämtar och anger bilddata för fyllningen.

```csharp
public byte[] ImageData { get; set; }
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
    public class TextureFillPropertyImageDataDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till ett diagram
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 5, 15, 15);
            Chart chart = worksheet.Charts[chartIndex];

            // Ange typ av texturfyllning
            chart.ChartArea.Area.FillFormat.FillType = FillType.Texture;

            // Läs in bilddata
            byte[] imageData = File.ReadAllBytes("texture.png");

            // Ange bilddata för texturfyllning
            chart.ChartArea.Area.FillFormat.TextureFill.ImageData = imageData;

            // Spara arbetsboken
            workbook.Save("TextureFillDemo.xlsx");
        }
    }
}
```

### Se även

* class [TextureFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


