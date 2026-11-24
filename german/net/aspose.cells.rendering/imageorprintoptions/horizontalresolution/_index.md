---
title: "ImageOrPrintOptions.HorizontalResolution"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ImageOrPrintOptions Eigenschaft. Gibt die horizontale Auflösung für erzeugte Bilder in DPI zurück oder legt sie fest"
type: docs
url: /de/net/aspose.cells.rendering/imageorprintoptions/horizontalresolution/
---
## ImageOrPrintOptions.HorizontalResolution property

Ruft die horizontale Auflösung für erzeugte Bilder ab oder legt sie fest, in Punkten pro Zoll.

```csharp
public int HorizontalResolution { get; set; }
```

### Hinweise

Der Standardwert ist 96.

Einstellung von `HorizontalResolution` und [`VerticalResolution`](../verticalresolution/) beeinflusst die Breite und Höhe des Ausgabebildes in Pixeln.

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ImageOrPrintOptionsPropertyHorizontalResolutionDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch mit Beispieldaten
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample Text for Image Rendering");

            // Initialisiere ImageOrPrintOptions
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.ImageType = ImageType.Png;
            
            // Setze horizontale und vertikale Auflösung
            options.HorizontalResolution = 192;
            options.VerticalResolution = 192;

            // Render das Arbeitsblatt als Bild mit angegebener Auflösung
            SheetRender renderer = new SheetRender(worksheet, options);
            renderer.ToImage(0, "WorksheetImage_192dpi.png");

            // Unterschiedliche Auflösungen demonstrieren
            options.HorizontalResolution = 300;
            options.VerticalResolution = 300;
            renderer = new SheetRender(worksheet, options);
            renderer.ToImage(0, "WorksheetImage_300dpi.png");
        }
    }
}
```

### Siehe auch

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


