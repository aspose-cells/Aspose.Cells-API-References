---
title: "ImageOrPrintOptions.ImageType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ImageOrPrintOptions‑Eigenschaft. Gibt das Format der erzeugten Bilder zurück oder legt es fest. Standardwert PNG"
type: docs
url: /de/net/aspose.cells.rendering/imageorprintoptions/imagetype/
---
## ImageOrPrintOptions.ImageType property

Liest oder setzt das Format der erzeugten Bilder. Standardwert: PNG.

```csharp
public virtual ImageType ImageType { get; set; }
```

### Beispiele

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ImageOrPrintOptionsPropertyImageTypeDemo
    {
        public static void Run()
        {
            // Erstelle ein Beispielarbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Test SVG Image");

            // Setze HTML‑Speicheroptionen mit Bildtyp SVG
            HtmlSaveOptions options = new HtmlSaveOptions();
            options.ImageOptions.ImageType = ImageType.Svg;
            options.ExportActiveWorksheetOnly = true;

            // Speichere die Arbeitsmappe als HTML
            string outputPath = Path.Combine(Environment.GetFolderPath(Environment.SpecialFolder.Desktop), "output.html");
            workbook.Save(outputPath, options);

            Console.WriteLine("File saved with SVG images: " + outputPath);
        }
    }
}
```

### Siehe auch

* enum [ImageType](../../../aspose.cells.drawing/imagetype/)
* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


