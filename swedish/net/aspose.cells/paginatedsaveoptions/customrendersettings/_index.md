---
title: "PaginatedSaveOptions.CustomRenderSettings"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PaginatedSaveOptions egenskap. Hämtar eller anger anpassade inställningar under renderingen"
type: docs
url: /sv/net/aspose.cells/paginatedsaveoptions/customrendersettings/
---
## PaginatedSaveOptions.CustomRenderSettings property

Hämtar eller anger anpassade inställningar under rendering.

```csharp
public CustomRenderSettings CustomRenderSettings { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class PaginatedSaveOptionsPropertyCustomRenderSettingsDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till lite exempeldata
            worksheet.Cells["A1"].Value = "Custom Render Settings Demo";
            worksheet.Cells["A2"].Value = "This demonstrates CustomRenderSettings property";

            try
            {
                // Skapa PdfSaveOptions som ärver från PaginatedSaveOptions
                PdfSaveOptions saveOptions = new PdfSaveOptions();

                // Hämta det aktuella värdet för CustomRenderSettings
                CustomRenderSettings currentSettings = saveOptions.CustomRenderSettings;
                Console.WriteLine("Current CustomRenderSettings: " +
                    (currentSettings == null ? "null" : "CustomRenderSettings instance"));

                // Skapa och ange nya CustomRenderSettings
                CustomRenderSettings newSettings = new CustomRenderSettings();
                saveOptions.CustomRenderSettings = newSettings;

                // Verifiera att de nya inställningarna har tillämpats
                Console.WriteLine("New CustomRenderSettings set: " +
                    (saveOptions.CustomRenderSettings == newSettings ? "Success" : "Failed"));

                // Spara arbetsboken med de anpassade renderingsinställningarna
                workbook.Save("CustomRenderSettingsDemo.pdf", saveOptions);
                Console.WriteLine("Workbook saved with CustomRenderSettings");
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

* class [CustomRenderSettings](../../../aspose.cells.rendering/customrendersettings/)
* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


