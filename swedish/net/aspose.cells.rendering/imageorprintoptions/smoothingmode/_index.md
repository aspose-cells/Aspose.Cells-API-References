---
title: "ImageOrPrintOptions.SmoothingMode"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ImageOrPrintOptions-egenskap. Anger om jämnings-antialiasing tillämpas på linjer och kurvor samt kanterna på fyllda områden. Standardvärdet är SmoothingMode.None"
type: docs
url: /sv/net/aspose.cells.rendering/imageorprintoptions/smoothingmode/
---
## ImageOrPrintOptions.SmoothingMode property

Anger om utjämning (kantutjämning) tillämpas på linjer och kurvor samt kanterna på fyllda områden. Standardvärdet är SmoothingMode.None

```csharp
public SmoothingMode SmoothingMode { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;
    using System.IO;

    public class ImageOrPrintOptionsPropertySmoothingModeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till lite exempeldata
            worksheet.Cells["A1"].Value = "ImageOrPrintOptions Demo";
            worksheet.Cells["A2"].Value = "Sample Data";

            try
            {
                // Skapa en ImageOrPrintOptions-instans
                ImageOrPrintOptions options = new ImageOrPrintOptions();

                // Visa några av de tillgängliga egenskaperna
                Console.WriteLine("HorizontalResolution: " + options.HorizontalResolution);
                Console.WriteLine("VerticalResolution: " + options.VerticalResolution);
                Console.WriteLine("ImageType: " + options.ImageType);

                // Skapa en SheetRender för att demonstrera egenskapen
                SheetRender renderer = new SheetRender(worksheet, options);

                // Rendera till en minnesström för att demonstrera funktionaliteten
                MemoryStream stream = new MemoryStream();
                renderer.ToImage(0, stream);

                Console.WriteLine("Sheet rendered successfully");
                Console.WriteLine("Image size: " + stream.Length + " bytes");

                // Spara arbetsboken
                workbook.Save("ImageOrPrintOptionsDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
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


