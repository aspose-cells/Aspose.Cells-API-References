---
title: "RenderingWatermark.Font"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "RenderingWatermark-Eigenschaft. Gibt die Schriftart des Wasserzeichens zurück."
type: docs
url: /de/net/aspose.cells.rendering/renderingwatermark/font/
---
## RenderingWatermark.Font property

Liest die Schriftart des Wasserzeichens.

```csharp
public RenderingFont Font { get; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class RenderingWatermarkPropertyFontDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Erstellen Sie eine Rendering-Schriftart und setzen Sie die Anfangseigenschaften.
            RenderingFont font = new RenderingFont("Arial", 24);
            
            // Erstellen Sie ein Textwasserzeichen mit der Rendering-Schriftart.
            RenderingWatermark watermark = new RenderingWatermark("CONFIDENTIAL", font);
            
            // Anzeigen der anfänglichen Schriftarteigenschaften.
            Console.WriteLine("Initial Font Name: " + watermark.Font.Name);
            Console.WriteLine("Initial Font Size: " + watermark.Font.Size);
            Console.WriteLine("Initial Bold Status: " + watermark.Font.Bold);
            
            // Ändern Sie die Schriftarteigenschaften über die RenderingFont-Referenz.
            font.Bold = true;
            
            // Anzeigen der aktualisierten Schriftarteigenschaften des Wasserzeichens.
            Console.WriteLine("\nUpdated Font Name: " + watermark.Font.Name);
            Console.WriteLine("Updated Font Size: " + watermark.Font.Size);
            Console.WriteLine("Updated Bold Status: " + watermark.Font.Bold);
            
            // Konfigurieren Sie die Anzeigeeigenschaften des Wasserzeichens.
            watermark.Opacity = 0.5f;
            watermark.Rotation = 45;
            watermark.IsBackground = true;
            
            // Erstellen Sie PDF-Speicheroptionen und weisen Sie das Wasserzeichen zu.
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            pdfSaveOptions.Watermark = watermark;
            
            // Speichern Sie die Arbeitsmappe mit einem wassergezeichneten PDF, um Schriftänderungen zu zeigen.
            workbook.Save("RenderingWatermarkFontDemo.pdf", pdfSaveOptions);
        }
    }
}
```

### Siehe auch

* class [RenderingFont](../../renderingfont/)
* class [RenderingWatermark](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


