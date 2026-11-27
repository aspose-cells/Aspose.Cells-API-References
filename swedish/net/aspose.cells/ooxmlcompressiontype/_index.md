---
title: "Enum OoxmlCompressionType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.OoxmlCompressionType enum. Ooxml-komprimeringstypen"
type: docs
url: /sv/net/aspose.cells/ooxmlcompressiontype/
---
## OoxmlCompressionType enumeration

Ooxml-komprimeringstypen

```csharp
public enum OoxmlCompressionType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| Level1 | `1` | Den snabbaste men minst effektiva komprimeringen. |
| Level2 | `2` | Lite långsammare, men bättre, än nivå 1. |
| Level3 | `3` | Lite långsammare, men bättre, än nivå 2. |
| Level4 | `4` | Lite långsammare, men bättre, än nivå 3. |
| Level5 | `5` | Lite långsammare än nivå 4, men med bättre komprimering. |
| Level6 | `6` | En bra balans mellan hastighet och komprimeringseffektivitet. |
| Level7 | `7` | Ganska bra komprimering! |
| Level8 | `8` | Bättre komprimering än Level7! |
| Level9 | `9` | Den "bästa" komprimeringen, där bästa betyder största minskning i storlek på den inkommande dataströmmen. Detta är också den långsammaste komprimeringen. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class OoxmlCompressionTypeDemo
    {
        public static void OoxmlCompressionTypeExample()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till lite data i kalkylbladet
            worksheet.Cells["A1"].PutValue("Sample Data");
            worksheet.Cells["A2"].PutValue(123);
            worksheet.Cells["A3"].PutValue(456);

            // Skapa OoxmlSaveOptions och ställ in komprimeringstypen
            OoxmlSaveOptions saveOptions = new OoxmlSaveOptions();
            saveOptions.CompressionType = OoxmlCompressionType.Level6; // A good balance of speed and compression efficiency

            // Spara arbetsboken med den angivna komprimeringstypen
            workbook.Save("OoxmlCompressionTypeExample.xlsx", saveOptions);

            Console.WriteLine("Workbook saved with OoxmlCompressionType.Level6 compression.");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


