---
title: "Range.ToImage"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Range-metoden. Konverterar området till bild"
type: docs
url: /sv/net/aspose.cells/range/toimage/
---
## Range.ToImage method

Konverterar området till en bild.

```csharp
public byte[] ToImage(ImageOrPrintOptions options)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| alternativ | ImageOrPrintOptions | Alternativen för att konvertera detta område till bild |

### Exempel

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
            // Skapa arbetsbok från exempel‑Excel‑fil
            Workbook workbook = new Workbook("example.xlsx");
            
            // Hämta det första kalkylbladet och dess celler
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;
            
            // Skapa området A1:J25
            Aspose.Cells.Range range = cells.CreateRange("A1:J25");
            
            // Skapa bildalternativ
            ImageOrPrintOptions options = new ImageOrPrintOptions()
            {
                ImageType = Aspose.Cells.Drawing.ImageType.Png,
                HorizontalResolution = 300,
                VerticalResolution = 300
            };
            
            // Konvertera området till bild
            byte[] imageData = range.ToImage(options);
            
            // Spara bilden till fil
            File.WriteAllBytes("range_output.png", imageData);
        }
    }
}
```

### Se även

* class [ImageOrPrintOptions](../../../aspose.cells.rendering/imageorprintoptions/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


