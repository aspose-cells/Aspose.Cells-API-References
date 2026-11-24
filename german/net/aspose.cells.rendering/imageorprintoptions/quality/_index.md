---
title: "ImageOrPrintOptions.Quality"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ImageOrPrintOptions-Eigenschaft. Gibt einen Wert zurück oder legt ihn fest, der die Qualität der erzeugten Bilder bestimmt und nur beim Speichern von Seiten im JPEG-Format angewendet wird. Der Standardwert ist 100"
type: docs
url: /de/net/aspose.cells.rendering/imageorprintoptions/quality/
---
## ImageOrPrintOptions.Quality property

Ruft den Wert ab oder legt ihn fest, der die Qualität der erzeugten Bilder bestimmt und nur beim Speichern von Seiten im `Jpeg`‑Format angewendet wird. Der Standardwert ist 100

```csharp
public int Quality { get; set; }
```

### Hinweise

Wirkt nur beim Speichern als JPEG. Der Wert muss zwischen 0 und 100 liegen. Der Standardwert ist 100.

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class ImageOrPrintOptionsPropertyQualityDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie Beispieldaten hinzu
            worksheet.Cells["A1"].PutValue("Sample Text");
            worksheet.Cells["B2"].PutValue(123.45);
            worksheet.Cells["C3"].PutValue(DateTime.Now);

            // Bildoptionen mit unterschiedlichen Qualitätseinstellungen erstellen
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.ImageType = Aspose.Cells.Drawing.ImageType.Jpeg;
            options.Quality = 100; // Highest quality

            // Arbeitsblatt mit hoher Qualität in ein Bild rendern
            SheetRender renderer = new SheetRender(worksheet, options);
            renderer.ToImage(0, "HighQualityOutput.jpg");

            // Qualität ändern, um den Unterschied zu demonstrieren
            options.Quality = 50; // Medium quality
            renderer.ToImage(0, "MediumQualityOutput.jpg");

            options.Quality = 10; // Low quality
            renderer.ToImage(0, "LowQualityOutput.jpg");
        }
    }
}
```

### Siehe auch

* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


