---
title: "MsoFillFormatHelper.ImageData"
second_title: "Aspose.Cells för .NET API‑referens"
description: "MsoFillFormatHelper property. Hämtar och anger textur- och bildfyllnadsdata"
type: docs
url: /sv/net/aspose.cells.drawing/msofillformathelper/imagedata/
---
## MsoFillFormatHelper.ImageData property

Hämtar och anger textur‑ och bildfyllnadsdata.

```csharp
public byte[] ImageData { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;
    using System.IO;

    public class MsoFillFormatHelperPropertyImageDataDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok och hämta det första kalkylbladet
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en etikett för att göra exemplet meningsfullt
            worksheet.Cells["A1"].Value = "ImageData Property Demo";

            try
            {
                // Skapa en instans av MsoFillFormatHelper med hjälp av reflektion (ingen publik konstruktor)
                MsoFillFormatHelper fillHelper = (MsoFillFormatHelper)Activator.CreateInstance(
                    typeof(MsoFillFormatHelper), nonPublic: true);

                // Visa det aktuella värdet för ImageData‑egenskapen
                Console.WriteLine($"Current ImageData: {(fillHelper.ImageData == null ? "null" : $"Length: {fillHelper.ImageData.Length} bytes")}");

                // Ange ny bilddata (skapa en enkel 1x1‑pixel röd bild)
                byte[] imageData = new byte[] { 0x42, 0x4D, 0x3A, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x36, 0x00, 0x00, 0x00, 0x28, 0x00,
                                               0x00, 0x00, 0x01, 0x00, 0x00, 0x00, 0x01, 0x00, 0x00, 0x00, 0x01, 0x00, 0x18, 0x00, 0x00, 0x00,
                                               0x00, 0x00, 0x04, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00,
                                               0x00, 0x00, 0x00, 0x00, 0x00, 0xFF, 0x00, 0x00 };

                fillHelper.ImageData = imageData;
                Console.WriteLine($"Updated ImageData length: {fillHelper.ImageData.Length} bytes");

                // Demonstrera läsning av ImageData‑värdet
                byte[] currentImageData = fillHelper.ImageData;
                Console.WriteLine($"Current ImageData length: {currentImageData.Length} bytes");

                // Spara arbetsboken för att demonstrera en lyckad körning
                workbook.Save("ImageDataDemo.xlsx");

                Console.WriteLine("ImageData property demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during ImageData demo: {ex.Message}");
            }
        }
    }
}
```

### Se även

* class [MsoFillFormatHelper](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


