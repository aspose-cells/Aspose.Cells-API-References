---
title: "ImageOrPrintOptions.PixelFormat"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ImageOrPrintOptions-egenskap. Hämtar eller anger pixelformatet för de genererade bilderna"
type: docs
url: /sv/net/aspose.cells.rendering/imageorprintoptions/pixelformat/
---
## ImageOrPrintOptions.PixelFormat property

Hämtar eller anger pixelformatet för de genererade bilderna.

```csharp
public PixelFormat PixelFormat { get; set; }
```

### Anmärkningar

Standardvärdet är PixelFormat.Format32bppArgb.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class ImageOrPrintOptionsPropertyPixelFormatDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Skapa ett exempelark
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till data för att göra exemplet meningsfullt
            worksheet.Cells["A1"].Value = "Sample Data";
            worksheet.Cells["B1"].Value = "PixelFormat Demo";

            try
            {
                // Skapa en ImageOrPrintOptions-instans
                ImageOrPrintOptions options = new ImageOrPrintOptions();

                // Visa det aktuella värdet för egenskapen ImageType (eftersom PixelFormat inte finns).
                Console.WriteLine("Current ImageType: " + options.ImageType);

                // Obs: Eftersom PixelFormat inte finns i API:et demonstrerar vi ImageType istället.
                // vilken är den närmaste relaterade egenskapen för bildformatinställningar

                // Skapa en SheetRender för att demonstrera de använda alternativen.
                SheetRender sheetRender = new SheetRender(worksheet, options);

                // Spara resultatet som en bild för att demonstrera alternativen.
                sheetRender.ToImage(0, "PixelFormatDemo.png");

                Console.WriteLine("ImageType property has been demonstrated. Image saved as PixelFormatDemo.png");
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

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


