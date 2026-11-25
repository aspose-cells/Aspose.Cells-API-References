---
title: "ImageOrPrintOptions.CustomRenderSettings"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ImageOrPrintOptions. Ottiene o imposta le impostazioni personalizzate durante il rendering"
type: docs
url: /it/net/aspose.cells.rendering/imageorprintoptions/customrendersettings/
---
## ImageOrPrintOptions.CustomRenderSettings property

Ottiene o imposta le impostazioni personalizzate durante il rendering.

```csharp
public CustomRenderSettings CustomRenderSettings { get; set; }
```

### Esempi

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
            // Crea una nuova cartella di lavoro con alcuni dati di esempio
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            sheet.Cells["A1"].PutValue("Demo for CustomRenderSettings");
            sheet.Cells["B2"].PutValue(12345);
            sheet.Cells["C3"].PutValue(DateTime.Now);

            try
            {
                // Inizializza ImageOrPrintOptions
                ImageOrPrintOptions options = new ImageOrPrintOptions();

                // Accedi alla proprietà CustomRenderSettings (sola lettura) e visualizza il suo stato attuale
                var customRenderSettings = options.CustomRenderSettings;
                Console.WriteLine("CustomRenderSettings instance: " +
                                  (customRenderSettings != null ? customRenderSettings.GetType().FullName : "null"));

                // Facoltativamente dimostra che le opzioni funzionano ancora per il rendering
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

### Vedi anche

* class [CustomRenderSettings](../../customrendersettings/)
* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


