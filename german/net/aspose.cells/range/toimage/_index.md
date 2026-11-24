---
title: "Range.ToImage"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Range-Methode. Konvertiert den Bereich in ein Bild"
type: docs
url: /de/net/aspose.cells/range/toimage/
---
## Range.ToImage method

Konvertiert den Bereich in ein Bild.

```csharp
public byte[] ToImage(ImageOrPrintOptions options)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Optionen | ImageOrPrintOptions | Die Optionen zum Konvertieren dieses Bereichs in ein Bild |

### Beispiele

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class RangeMethodToImageWithImageOrPrintOptionsDemo
    {
        public static void Run()
        {
            // Arbeitsmappe aus einer Beispiel-Excel-Datei erstellen
            Workbook workbook = new Workbook("example.xlsx");
            
            // Erste Arbeitsblatt und dessen Zellen abrufen
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;
            
            // Bereich A1:J25 erstellen
            Aspose.Cells.Range range = cells.CreateRange("A1:J25");
            
            // Bildoptionen erstellen
            ImageOrPrintOptions options = new ImageOrPrintOptions()
            {
                ImageType = Aspose.Cells.Drawing.ImageType.Png,
                HorizontalResolution = 300,
                VerticalResolution = 300
            };
            
            // Bereich in ein Bild konvertieren
            byte[] imageData = range.ToImage(options);
            
            // Bild in Datei speichern
            File.WriteAllBytes("range_output.png", imageData);
        }
    }
}
```

### Siehe auch

* class [ImageOrPrintOptions](../../../aspose.cells.rendering/imageorprintoptions/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


