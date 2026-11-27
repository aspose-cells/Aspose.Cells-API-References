---
title: "ImageOrPrintOptions.PageCount"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ImageOrPrintOptions-egenskap. Hämtar eller anger antalet sidor som ska sparas"
type: docs
url: /sv/net/aspose.cells.rendering/imageorprintoptions/pagecount/
---
## ImageOrPrintOptions.PageCount property

Hämtar eller anger antalet sidor som ska sparas.

```csharp
public int PageCount { get; set; }
```

### Anmärkningar

Standard är System.Int32.MaxValue vilket betyder att alla sidor kommer att renderas.

### Exempel

```csharp
using System;
using System.IO;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class ImageOrPrintOptionsPropertyPageCountDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok med exempeldata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata i kalkylbladet
            worksheet.Cells["A1"].PutValue("Page 1 Data");
            worksheet.Cells["A2"].PutValue("Sample Content");
            worksheet.Cells["A3"].PutValue("Demo for PageCount");
            
            // Ställ in utskriftsområde och sidinställningar
            worksheet.PageSetup.PrintArea = "A1:A3";
            worksheet.PageSetup.LeftMargin = 0;
            worksheet.PageSetup.RightMargin = 0;
            worksheet.PageSetup.TopMargin = 0;
            worksheet.PageSetup.BottomMargin = 0;

            // Skapa bild- eller utskriftsalternativ
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.OnePagePerSheet = true;
            options.ImageType = Aspose.Cells.Drawing.ImageType.Png; // Fully qualified namespace AsposeCellsExamples = 1; // Demonstrating PageCount property
            options.OnlyArea = true;

            // Rendera kalkylbladet till bild
            SheetRender renderer = new SheetRender(worksheet, options);
            using (MemoryStream stream = new MemoryStream())
            {
                renderer.ToImage(0, stream);
                
                // Spara bilden till fil
                string outputPath = "output.png";
                File.WriteAllBytes(outputPath, stream.ToArray());
                Console.WriteLine($"Output saved to: {outputPath}");
            }
        }
    }
}
```

### Se även

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


