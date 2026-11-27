---
title: "MarkdownSaveOptions.ImageOptions"
second_title: "Aspose.Cells för .NET API‑referens"
description: "MarkdownSaveOptions egenskap. Hämta ImageOrPrintOptions-objektet innan export"
type: docs
url: /sv/net/aspose.cells/markdownsaveoptions/imageoptions/
---
## MarkdownSaveOptions.ImageOptions property

Hämta ImageOrPrintOptions-objektet innan export

```csharp
public ImageOrPrintOptions ImageOptions { get; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class MarkdownSaveOptionsPropertyImageOptionsDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Skapa ett exempelark
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till data för att göra exemplet meningsfullt
            worksheet.Cells["A1"].Value = "Sample Data";
            worksheet.Cells["A2"].Value = "Image Options Demo";

            try
            {
                // Skapa en instans av MarkdownSaveOptions
                MarkdownSaveOptions saveOptions = new MarkdownSaveOptions();

                // Åtkomst till ImageOptions-egenskap (skrivskyddad)
                ImageOrPrintOptions imageOptions = saveOptions.ImageOptions;

                // Visa de aktuella värdena för ImageOptions-egenskaperna
                Console.WriteLine("ImageOptions properties:");
                Console.WriteLine($"HorizontalResolution: {imageOptions.HorizontalResolution}");
                Console.WriteLine($"VerticalResolution: {imageOptions.VerticalResolution}");
                Console.WriteLine($"ImageType: {imageOptions.ImageType}");
                Console.WriteLine($"Quality: {imageOptions.Quality}");
                Console.WriteLine($"Transparent: {imageOptions.Transparent}");

                // Spara arbetsboken med de aktuella alternativen
                workbook.Save("ImageOptionsDemo.md", saveOptions);

                Console.WriteLine("Markdown file saved successfully with ImageOptions demonstrated.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Se även

* class [ImageOrPrintOptions](../../../aspose.cells.rendering/imageorprintoptions/)
* class [MarkdownSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


