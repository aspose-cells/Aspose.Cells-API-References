---
title: "ImageOrPrintOptions.CustomQueryPageSettingsEventHandler"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ImageOrPrintOptions‑egenskap. Klienten kan kontrollera skrivarens sidinställningar när varje sida skrivs ut med denna EventHandler"
type: docs
url: /sv/net/aspose.cells.rendering/imageorprintoptions/customquerypagesettingseventhandler/
---
## ImageOrPrintOptions.CustomQueryPageSettingsEventHandler property

Klienten kan kontrollera sidinställningarna för skrivaren när varje sida skrivs ut med denna EventHandler

```csharp
public QueryPageSettingsEventHandler CustomQueryPageSettingsEventHandler { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class ImageOrPrintOptionsPropertyCustomQueryPageSettingsEventHandlerDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till lite exempeldata
            worksheet.Cells["A1"].Value = "Sample Data";
            worksheet.Cells["B1"].Value = "More Data";

            try
            {
                // Skapa en ImageOrPrintOptions-instans
                ImageOrPrintOptions options = new ImageOrPrintOptions();

                // Visa några av de tillgängliga egenskaperna
                Console.WriteLine("Current HorizontalResolution: " + options.HorizontalResolution);
                Console.WriteLine("Current VerticalResolution: " + options.VerticalResolution);
                Console.WriteLine("Current ImageType: " + options.ImageType);

                // Demonstrera att sätta några egenskaper
                options.HorizontalResolution = 300;
                options.VerticalResolution = 300;
                options.ImageType = Aspose.Cells.Drawing.ImageType.Png;

                // Verifiera att egenskaperna är satta
                Console.WriteLine("Updated HorizontalResolution: " + options.HorizontalResolution);
                Console.WriteLine("Updated VerticalResolution: " + options.VerticalResolution);
                Console.WriteLine("Updated ImageType: " + options.ImageType);

                // Skapa en SheetRender för att demonstrera rendering
                SheetRender renderer = new SheetRender(worksheet, options);

                // Spara arbetsboken
                workbook.Save("CustomQueryPageSettingsEventHandlerDemo.xlsx");

                Console.WriteLine("ImageOrPrintOptions demonstration completed");
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


