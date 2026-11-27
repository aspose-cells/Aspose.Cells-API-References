---
title: "RenderingWatermark.Font"
second_title: "Aspose.Cells för .NET API‑referens"
description: "RenderingWatermark-egenskap. Hämtar teckensnittet för vattenstämpeln"
type: docs
url: /sv/net/aspose.cells.rendering/renderingwatermark/font/
---
## RenderingWatermark.Font property

Hämtar teckensnittet för vattenstämpeln.

```csharp
public RenderingFont Font { get; }
```

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Skapa ett rendering font och ange initiala egenskaper
            RenderingFont font = new RenderingFont("Arial", 24);
            
            // Skapa en textvattenstämpel med rendering font
            RenderingWatermark watermark = new RenderingWatermark("CONFIDENTIAL", font);
            
            // Visa initiala teckensnittsegenskaper
            Console.WriteLine("Initial Font Name: " + watermark.Font.Name);
            Console.WriteLine("Initial Font Size: " + watermark.Font.Size);
            Console.WriteLine("Initial Bold Status: " + watermark.Font.Bold);
            
            // Ändra teckensnittsegenskaper via RenderingFont-referensen
            font.Bold = true;
            
            // Visa uppdaterade teckensnittsegenskaper från vattenstämpeln
            Console.WriteLine("\nUpdated Font Name: " + watermark.Font.Name);
            Console.WriteLine("Updated Font Size: " + watermark.Font.Size);
            Console.WriteLine("Updated Bold Status: " + watermark.Font.Bold);
            
            // Konfigurera vattenstämpelns visningsegenskaper
            watermark.Opacity = 0.5f;
            watermark.Rotation = 45;
            watermark.IsBackground = true;
            
            // Skapa PDF-sparaalternativ och tilldela vattenstämpel
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            pdfSaveOptions.Watermark = watermark;
            
            // Spara arbetsbok med vattenmärkt PDF för att visa teckensnittsförändringar
            workbook.Save("RenderingWatermarkFontDemo.pdf", pdfSaveOptions);
        }
    }
}
```

### Se även

* class [RenderingFont](../../renderingfont/)
* class [RenderingWatermark](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


