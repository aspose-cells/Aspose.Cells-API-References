---
title: "Enum OoxmlCompressionType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.OoxmlCompressionType Enum. Der Ooxml-Kompressionstyp"
type: docs
url: /de/net/aspose.cells/ooxmlcompressiontype/
---
## OoxmlCompressionType enumeration

Der Ooxml-Kompressionstyp

```csharp
public enum OoxmlCompressionType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| Level1 | `1` | Die schnellste, aber am wenigsten effektive Kompression. |
| Level2 | `2` | Etwas langsamer, aber besser als Stufe 1. |
| Level3 | `3` | Etwas langsamer, aber besser als Stufe 2. |
| Level4 | `4` | Etwas langsamer, aber besser als Stufe 3. |
| Level5 | `5` | Etwas langsamer als Stufe 4, aber mit besserer Kompression. |
| Level6 | `6` | Ein gutes Gleichgewicht zwischen Geschwindigkeit und Kompressionseffizienz. |
| Level7 | `7` | Ziemlich gute Kompression! |
| Level8 | `8` | Bessere Kompression als Stufe 7! |
| Level9 | `9` | Die "beste" Kompression, wobei "beste" die größte Reduzierung der Größe des Eingabedatenstroms bedeutet. Dies ist auch die langsamste Kompression. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class OoxmlCompressionTypeDemo
    {
        public static void OoxmlCompressionTypeExample()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge dem Arbeitsblatt einige Daten hinzu
            worksheet.Cells["A1"].PutValue("Sample Data");
            worksheet.Cells["A2"].PutValue(123);
            worksheet.Cells["A3"].PutValue(456);

            // Erstelle OoxmlSaveOptions und setze den Kompressionstyp
            OoxmlSaveOptions saveOptions = new OoxmlSaveOptions();
            saveOptions.CompressionType = OoxmlCompressionType.Level6; // A good balance of speed and compression efficiency

            // Speichere die Arbeitsmappe mit dem angegebenen Kompressionstyp
            workbook.Save("OoxmlCompressionTypeExample.xlsx", saveOptions);

            Console.WriteLine("Workbook saved with OoxmlCompressionType.Level6 compression.");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


