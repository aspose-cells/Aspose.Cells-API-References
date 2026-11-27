---
title: "ImageOrPrintOptions.OutputBlankPageWhenNothingToPrint"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ImageOrPrintOptions-egenskap. Anger om en tom sida ska skrivas ut när det inte finns något att skriva ut"
type: docs
url: /sv/net/aspose.cells.rendering/imageorprintoptions/outputblankpagewhennothingtoprint/
---
## ImageOrPrintOptions.OutputBlankPageWhenNothingToPrint property

Anger om en tom sida ska skrivas ut när det inte finns något att skriva ut.

```csharp
public bool OutputBlankPageWhenNothingToPrint { get; set; }
```

### Anmärkningar

Standard är falskt.

### Exempel

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class ImageOrPrintOptionsPropertyOutputBlankPageWhenNothingToPrintDemo
    {
        public static void Run()
        {
            // Skapa en ny tom arbetsbok
            Workbook workbook = new Workbook();
            
            // Öppna det första kalkylbladet som är tomt
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ställ in bild- eller utskriftsalternativ
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.ImageType = Aspose.Cells.Drawing.ImageType.Png;
            options.OnePagePerSheet = true;
            
            // Demonstrera OutputBlankPageWhenNothingToPrint-egenskapen
            options.OutputBlankPageWhenNothingToPrint = true;
            
            // Rendera bladet
            SheetRender renderer = new SheetRender(worksheet, options);
            
            // Utskriften kommer fortfarande att producera en tom sida på grund av egenskapsinställningen
            Console.WriteLine("Page count with OutputBlankPageWhenNothingToPrint=true: " + renderer.PageCount);
            
            // Spara den första sidan till minnesström
            MemoryStream stream = new MemoryStream();
            renderer.ToImage(0, stream);
            Console.WriteLine("Image data length: " + stream.ToArray().Length);
            
            // Ställ nu in egenskapen till falskt
            options.OutputBlankPageWhenNothingToPrint = false;
            SheetRender renderer2 = new SheetRender(worksheet, options);
            
            // Utskriften kommer nu att ha noll sidor
            Console.WriteLine("Page count with OutputBlankPageWhenNothingToPrint=false: " + renderer2.PageCount);
        }
    }
}
```

### Se även

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


