---
title: "ImageOrPrintOptions.CustomPrintPageEventHandler"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ImageOrPrintOptions‑egenskap. Klienten kan specialutskrift till skrivare när varje sida skrivs ut med denna EventHandler"
type: docs
url: /sv/net/aspose.cells.rendering/imageorprintoptions/customprintpageeventhandler/
---
## ImageOrPrintOptions.CustomPrintPageEventHandler property

Klienten kan särskilt skicka utskrift till skrivaren när varje sida skrivs ut med denna EventHandler

```csharp
public PrintPageEventHandler CustomPrintPageEventHandler { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class ImageOrPrintOptionsPropertyCustomPrintPageEventHandlerDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till lite exempeldata
            worksheet.Cells["A1"].Value = "Sample Data for Printing";
            worksheet.Cells["A2"].Value = "This demonstrates printing options";

            try
            {
                // Skapa en ImageOrPrintOptions-instans
                ImageOrPrintOptions options = new ImageOrPrintOptions();

                // Konfigurera utskriftsalternativ
                options.PrintWithStatusDialog = true;
                options.HorizontalResolution = 300;
                options.VerticalResolution = 300;

                // Visa aktuella utskriftsalternativ
                Console.WriteLine($"PrintWithStatusDialog: {options.PrintWithStatusDialog}");
                Console.WriteLine($"HorizontalResolution: {options.HorizontalResolution}");
                Console.WriteLine($"VerticalResolution: {options.VerticalResolution}");

                // Skapa en SheetRender för att demonstrera utskrift
                SheetRender sheetRender = new SheetRender(worksheet, options);

                // Rendera till bild för att demonstrera utskrift
                sheetRender.ToImage(0, "output.png");
                Console.WriteLine("Rendering completed successfully.");
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


