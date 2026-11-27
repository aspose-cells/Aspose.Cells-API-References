---
title: "ImageOrPrintOptions.Transparent"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ImageOrPrintOptions-egenskap. Anger om bakgrunden för den genererade bilden ska vara transparent"
type: docs
url: /sv/net/aspose.cells.rendering/imageorprintoptions/transparent/
---
## ImageOrPrintOptions.Transparent property

Anger om bakgrunden på den genererade bilden ska vara transparent.

```csharp
public bool Transparent { get; set; }
```

### Anmärkningar

Standardvärdet är false. Det betyder att bakgrunden för de genererade bilderna är vit.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class ImageOrPrintOptionsPropertyTransparentDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok med exempeldata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Transparent Image Demo");
            
            // Ställ in HTML-sparalternativ med transparent PNG-bild
            HtmlSaveOptions options = new HtmlSaveOptions();
            options.ImageOptions.ImageType = Aspose.Cells.Drawing.ImageType.Png;
            options.ImageOptions.Transparent = true;
            options.ExportImagesAsBase64 = true;

            // Spara arbetsboken med transparenta bildalternativ
            workbook.Save("output.html", options);
            
            Console.WriteLine("HTML with transparent images saved successfully.");
        }
    }
}
```

### Se även

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


