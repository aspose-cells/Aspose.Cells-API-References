---
title: "RenderingFont.Name"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "RenderingFont property. Gibt den Namen der Schriftart zurück"
type: docs
url: /de/net/aspose.cells.rendering/renderingfont/name/
---
## RenderingFont.Name property

Liest den Namen der Schriftart.

```csharp
public string Name { get; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class RenderingFontPropertyNameDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // PDF-Speicheroptionen erstellen
            PdfSaveOptions options = new PdfSaveOptions();

            // Erstelle die anfängliche Rendering-Schriftart mit "Arial"
            RenderingFont fontArial = new RenderingFont("Arial", 16);
            Console.WriteLine("Initial font name: " + fontArial.Name);

            // Wasserzeichen mit anfänglicher Schriftart erstellen
            RenderingWatermark watermark = new RenderingWatermark("Confidential", fontArial);
            watermark.Opacity = 0.5f;
            watermark.Rotation = 45;
            options.Watermark = watermark;

            // Speichern mit Wasserzeichen der anfänglichen Schriftart
            workbook.Save("WatermarkInitial.pdf", options);

            // Neue Rendering-Schriftart mit "Times New Roman" erstellen
            RenderingFont fontTimesNewRoman = new RenderingFont("Times New Roman", 16);
            Console.WriteLine("\nModified font name: " + fontTimesNewRoman.Name);

            // Wasserzeichen mit neuer Schriftart aktualisieren
            RenderingWatermark updatedWatermark = new RenderingWatermark("Confidential", fontTimesNewRoman);
            updatedWatermark.Opacity = 0.5f;
            updatedWatermark.Rotation = 45;
            options.Watermark = updatedWatermark;

            // Speichern mit modifiziertem Schriftart-Wasserzeichen
            workbook.Save("WatermarkModified.pdf", options);
        }
    }
}
```

### Siehe auch

* class [RenderingFont](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


