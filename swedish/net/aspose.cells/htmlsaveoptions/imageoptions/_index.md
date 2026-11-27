---
title: "HtmlSaveOptions.ImageOptions"
second_title: "Aspose.Cells för .NET API‑referens"
description: "HtmlSaveOptions egenskap. Hämta ImageOrPrintOptions‑objektet innan export"
type: docs
url: /sv/net/aspose.cells/htmlsaveoptions/imageoptions/
---
## HtmlSaveOptions.ImageOptions property

Hämta ImageOrPrintOptions-objektet innan export

```csharp
public ImageOrPrintOptions ImageOptions { get; }
```

### Exempel

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Rendering;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyImageOptionsDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok med exempeldata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample HTML Export");
            
            // Ställ in HTML‑sparalternativ
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.ExportImagesAsBase64 = true;
            
            // Konfigurera bildalternativ
            ImageOrPrintOptions imageOptions = saveOptions.ImageOptions;
            imageOptions.ImageType = ImageType.Svg;
            imageOptions.HorizontalResolution = 300;
            imageOptions.VerticalResolution = 300;
            
            // Spara arbetsboken med HTML-alternativ
            string outputPath = "output.html";
            workbook.Save(outputPath, saveOptions);
            
            Console.WriteLine("HTML file saved with SVG images.");
        }
    }
}
```

### Se även

* class [ImageOrPrintOptions](../../../aspose.cells.rendering/imageorprintoptions/)
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


