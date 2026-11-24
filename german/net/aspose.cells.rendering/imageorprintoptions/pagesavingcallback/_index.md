---
title: "ImageOrPrintOptions.PageSavingCallback"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ImageOrPrintOptions-Eigenschaft. Steuert/zeigt den Fortschritt des Seiten‑Speichervorgangs an"
type: docs
url: /de/net/aspose.cells.rendering/imageorprintoptions/pagesavingcallback/
---
## ImageOrPrintOptions.PageSavingCallback property

Steuern/Anzeigen des Fortschritts des Seiten‑Speichervorgangs.

```csharp
public IPageSavingCallback PageSavingCallback { get; set; }
```

### Beispiele

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
            // Erstellen Sie eine neue Arbeitsmappe und füllen Sie Daten ein.
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Füge Beispieldaten hinzu, die sich über mehrere Seiten erstrecken
            worksheet.Cells["A1"].PutValue("PageSavingCallback Demonstration");
            for (int i = 1; i <= 50; i++)
            {
                worksheet.Cells[$"A{i + 1}"].PutValue($"Data Row {i}");
            }

            // Konfiguriere die Seiteneinrichtung, um mehrere Seiten zu erzeugen
            PageSetup pageSetup = worksheet.PageSetup;
            pageSetup.PaperSize = PaperSizeType.PaperA4;
            pageSetup.Orientation = PageOrientationType.Portrait;
            pageSetup.FitToPagesWide = 1;
            pageSetup.FitToPagesTall = 0;

            // Initialisiere ImageOrPrintOptions
            ImageOrPrintOptions options = new ImageOrPrintOptions
            {
                ImageType = ImageType.Tiff,
                TiffCompression = TiffCompression.CompressionCCITT4
            };

            // Zeige den anfänglichen Callback‑Zustand an
            Console.WriteLine($"Initial PageSavingCallback: {options.PageSavingCallback}");

            // Setze benutzerdefinierten Seiten‑Speicher‑Callback
            options.PageSavingCallback = new CustomPageSavingCallback();

            // Render das Arbeitsblatt zu einem mehrseitigen TIFF
            SheetRender renderer = new SheetRender(worksheet, options);
            renderer.ToTiff("output_with_callback.tiff");

            // Arbeitsmappe zum Referenzieren speichern
            workbook.Save("PageSavingCallbackDemo.xlsx");
        }

        private class CustomPageSavingCallback : IPageSavingCallback
        {
            public void PageStartSaving(PageStartSavingArgs args)
            {
                Console.WriteLine($"Processing page {args.PageIndex}");
                
                // Überspringe die erste Seite (Index ab 0)
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

### Siehe auch

* interface [IPageSavingCallback](../../ipagesavingcallback/)
* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


