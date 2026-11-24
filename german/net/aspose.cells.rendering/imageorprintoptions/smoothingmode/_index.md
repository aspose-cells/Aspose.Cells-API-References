---
title: "ImageOrPrintOptions.SmoothingMode"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ImageOrPrintOptions-Eigenschaft. Gibt an, ob Glättungs-Antialiasing auf Linien und Kurven sowie die Kanten gefüllter Bereiche angewendet wird. Der Standardwert ist SmoothingMode.None"
type: docs
url: /de/net/aspose.cells.rendering/imageorprintoptions/smoothingmode/
---
## ImageOrPrintOptions.SmoothingMode property

Gibt an, ob Glättung (Antialiasing) auf Linien, Kurven und die Kanten gefüllter Bereiche angewendet wird. Der Standardwert ist SmoothingMode.None

```csharp
public SmoothingMode SmoothingMode { get; set; }
```

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie einige Beispieldaten hinzu
            worksheet.Cells["A1"].Value = "ImageOrPrintOptions Demo";
            worksheet.Cells["A2"].Value = "Sample Data";

            try
            {
                // Erstelle eine ImageOrPrintOptions-Instanz
                ImageOrPrintOptions options = new ImageOrPrintOptions();

                // Zeige einige der verfügbaren Eigenschaften an
                Console.WriteLine("HorizontalResolution: " + options.HorizontalResolution);
                Console.WriteLine("VerticalResolution: " + options.VerticalResolution);
                Console.WriteLine("ImageType: " + options.ImageType);

                // Erstellen Sie ein SheetRender, um die Eigenschaft zu demonstrieren
                SheetRender renderer = new SheetRender(worksheet, options);

                // Rendern Sie in einen MemoryStream, um die Funktionalität zu demonstrieren
                MemoryStream stream = new MemoryStream();
                renderer.ToImage(0, stream);

                Console.WriteLine("Sheet rendered successfully");
                Console.WriteLine("Image size: " + stream.Length + " bytes");

                // Speichere die Arbeitsmappe
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

### Siehe auch

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


