---
title: "ImageOrPrintOptions.PageSavingCallback"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ImageOrPrintOptions-egenskap. Styr/indikera framsteg i processen för att spara sidor"
type: docs
url: /sv/net/aspose.cells.rendering/imageorprintoptions/pagesavingcallback/
---
## ImageOrPrintOptions.PageSavingCallback property

Styr/indikera framsteg för sidlagringsprocessen.

```csharp
public IPageSavingCallback PageSavingCallback { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Rendering;
    using System;

    public class ImageOrPrintOptionsPropertyPageSavingCallbackDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok och fyll i data
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata som sträcker sig över flera sidor
            worksheet.Cells["A1"].PutValue("PageSavingCallback Demonstration");
            for (int i = 1; i <= 50; i++)
            {
                worksheet.Cells[$"A{i + 1}"].PutValue($"Data Row {i}");
            }

            // Konfigurera sidinställningarna för att generera flera sidor
            PageSetup pageSetup = worksheet.PageSetup;
            pageSetup.PaperSize = PaperSizeType.PaperA4;
            pageSetup.Orientation = PageOrientationType.Portrait;
            pageSetup.FitToPagesWide = 1;
            pageSetup.FitToPagesTall = 0;

            // Initiera ImageOrPrintOptions
            ImageOrPrintOptions options = new ImageOrPrintOptions
            {
                ImageType = ImageType.Tiff,
                TiffCompression = TiffCompression.CompressionCCITT4
            };

            // Visa initialt callback-tillstånd
            Console.WriteLine($"Initial PageSavingCallback: {options.PageSavingCallback}");

            // Ange anpassad callback för sidsparning
            options.PageSavingCallback = new CustomPageSavingCallback();

            // Rendera kalkylblad till flersidig TIFF
            SheetRender renderer = new SheetRender(worksheet, options);
            renderer.ToTiff("output_with_callback.tiff");

            // Spara arbetsbok för referens
            workbook.Save("PageSavingCallbackDemo.xlsx");
        }

        private class CustomPageSavingCallback : IPageSavingCallback
        {
            public void PageStartSaving(PageStartSavingArgs args)
            {
                Console.WriteLine($"Processing page {args.PageIndex}");
                
                // Hoppa över första sidan (0-baserat index)
                if (args.PageIndex == 0)
                {
                    args.IsToOutput = false;
                    Console.WriteLine("Skipping first page");
                }
            }

            public void PageEndSaving(PageEndSavingArgs args)
            {
                Console.WriteLine($"Completed processing page {args.PageIndex}");
            }
        }
    }
}
```

### Se även

* interface [IPageSavingCallback](../../ipagesavingcallback/)
* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


