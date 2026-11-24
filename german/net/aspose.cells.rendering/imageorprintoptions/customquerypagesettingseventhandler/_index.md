---
title: "ImageOrPrintOptions.CustomQueryPageSettingsEventHandler"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ImageOrPrintOptions-Eigenschaft. Der Client kann die Seiteneinstellungen des Druckers für jede zu druckende Seite über diesen EventHandler steuern"
type: docs
url: /de/net/aspose.cells.rendering/imageorprintoptions/customquerypagesettingseventhandler/
---
## ImageOrPrintOptions.CustomQueryPageSettingsEventHandler property

Der Client kann die Seiteneinstellungen des Druckers steuern, wenn jede Seite mit diesem EventHandler gedruckt wird.

```csharp
public QueryPageSettingsEventHandler CustomQueryPageSettingsEventHandler { get; set; }
```

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie einige Beispieldaten hinzu
            worksheet.Cells["A1"].Value = "Sample Data";
            worksheet.Cells["B1"].Value = "More Data";

            try
            {
                // Erstelle eine ImageOrPrintOptions-Instanz
                ImageOrPrintOptions options = new ImageOrPrintOptions();

                // Zeige einige der verfügbaren Eigenschaften an
                Console.WriteLine("Current HorizontalResolution: " + options.HorizontalResolution);
                Console.WriteLine("Current VerticalResolution: " + options.VerticalResolution);
                Console.WriteLine("Current ImageType: " + options.ImageType);

                // Demonstriere das Festlegen einiger Eigenschaften
                options.HorizontalResolution = 300;
                options.VerticalResolution = 300;
                options.ImageType = Aspose.Cells.Drawing.ImageType.Png;

                // Verifiziere, dass die Eigenschaften gesetzt sind
                Console.WriteLine("Updated HorizontalResolution: " + options.HorizontalResolution);
                Console.WriteLine("Updated VerticalResolution: " + options.VerticalResolution);
                Console.WriteLine("Updated ImageType: " + options.ImageType);

                // Erstelle ein SheetRender, um das Rendern zu demonstrieren
                SheetRender renderer = new SheetRender(worksheet, options);

                // Speichere die Arbeitsmappe
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

### Siehe auch

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


