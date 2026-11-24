---
title: "ImageOrPrintOptions.Transparent"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ImageOrPrintOptions‑Eigenschaft. Gibt an, ob der Hintergrund des erzeugten Bildes transparent sein soll"
type: docs
url: /de/net/aspose.cells.rendering/imageorprintoptions/transparent/
---
## ImageOrPrintOptions.Transparent property

Gibt an, ob der Hintergrund des erzeugten Bildes transparent sein soll.

```csharp
public bool Transparent { get; set; }
```

### Hinweise

Der Standardwert ist false. Das bedeutet, dass der Hintergrund der erzeugten Bilder weiß ist.

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class ImageOrPrintOptionsPropertyTransparentDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch mit Beispieldaten
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Transparent Image Demo");
            
            // HTML‑Speicheroptionen mit transparentem PNG‑Bild festlegen
            HtmlSaveOptions options = new HtmlSaveOptions();
            options.ImageOptions.ImageType = Aspose.Cells.Drawing.ImageType.Png;
            options.ImageOptions.Transparent = true;
            options.ExportImagesAsBase64 = true;

            // Arbeitsmappe mit transparenten Bildoptionen speichern
            workbook.Save("output.html", options);
            
            Console.WriteLine("HTML with transparent images saved successfully.");
        }
    }
}
```

### Siehe auch

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


