---
title: "ImageOrPrintOptions.CustomRenderSettings"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ImageOrPrintOptions-egenskap. Hämtar eller anger anpassade inställningar under rendering"
type: docs
url: /sv/net/aspose.cells.rendering/imageorprintoptions/customrendersettings/
---
## ImageOrPrintOptions.CustomRenderSettings property

Hämtar eller anger anpassade inställningar under rendering.

```csharp
public CustomRenderSettings CustomRenderSettings { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using System;
    using Aspose.Cells;
    using Aspose.Cells.Rendering;

    public class ImageOrPrintOptionsPropertyCustomRenderSettingsDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok med några exempeldata
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            sheet.Cells["A1"].PutValue("Demo for CustomRenderSettings");
            sheet.Cells["B2"].PutValue(12345);
            sheet.Cells["C3"].PutValue(DateTime.Now);

            try
            {
                // Initiera ImageOrPrintOptions
                ImageOrPrintOptions options = new ImageOrPrintOptions();

                // Åtkomst till CustomRenderSettings-egenskapen (skrivskyddad) och visa dess aktuella tillstånd
                var customRenderSettings = options.CustomRenderSettings;
                Console.WriteLine("CustomRenderSettings instance: " +
                                  (customRenderSettings != null ? customRenderSettings.GetType().FullName : "null"));

                // Visa eventuellt att alternativen fortfarande fungerar för rendering
                options.ImageType = Aspose.Cells.Drawing.ImageType.Png;
                SheetRender renderer = new SheetRender(sheet, options);
                renderer.ToImage(0, "CustomRenderSettingsDemo.png");

                Console.WriteLine("Image rendered successfully.");
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

* class [CustomRenderSettings](../../customrendersettings/)
* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


