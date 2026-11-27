---
title: "ImageOrPrintOptions.ImageType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ImageOrPrintOptions-egenskap. Hämtar eller anger formatet för de genererade bilderna. standardvärde PNG"
type: docs
url: /sv/net/aspose.cells.rendering/imageorprintoptions/imagetype/
---
## ImageOrPrintOptions.ImageType property

Hämtar eller anger formatet för de genererade bilderna. standardvärde: PNG.

```csharp
public virtual ImageType ImageType { get; set; }
```

### Exempel

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ImageOrPrintOptionsPropertyImageTypeDemo
    {
        public static void Run()
        {
            // Skapa en exempelarbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Test SVG Image");

            // Ange HTML-spara-alternativ med SVG-bildtyp
            HtmlSaveOptions options = new HtmlSaveOptions();
            options.ImageOptions.ImageType = ImageType.Svg;
            options.ExportActiveWorksheetOnly = true;

            // Spara arbetsboken som HTML
            string outputPath = Path.Combine(Environment.GetFolderPath(Environment.SpecialFolder.Desktop), "output.html");
            workbook.Save(outputPath, options);

            Console.WriteLine("File saved with SVG images: " + outputPath);
        }
    }
}
```

### Se även

* enum [ImageType](../../../aspose.cells.drawing/imagetype/)
* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


