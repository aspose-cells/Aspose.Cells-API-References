---
title: "Enum TiffCompression"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Rendering.TiffCompression enum. Gibt an, welchen Kompressionstyp beim Speichern von Bildern in einer TIFF‑Datei angewendet werden soll."
type: docs
url: /de/net/aspose.cells.rendering/tiffcompression/
---
## TiffCompression enumeration

Gibt an, welchen Kompressionstyp beim Speichern von Bildern in einer TIFF-Datei anzuwenden ist.

```csharp
public enum TiffCompression
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| CompressionNone | `0` | Gibt keine Kompression an. |
| CompressionRle | `1` | Gibt das RLE‑Kompressionsverfahren an. |
| CompressionLZW | `2` | Gibt das LZW‑Kompressionsverfahren an. |
| CompressionCCITT3 | `3` | Gibt das CCITT3‑Kompressionsverfahren an. |
| CompressionCCITT4 | `4` | Gibt das CCITT4‑Kompressionsverfahren an. |

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class RenderingClassTiffCompressionDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch mit Beispieldaten
            Workbook wb = new Workbook();
            Worksheet ws = wb.Worksheets[0];
            ws.Cells["A1"].PutValue("TIFF Compression Test");
            ws.Cells["A2"].PutValue(DateTime.Now.ToString());

            // Lege Bildoptionen fest
            ImageOrPrintOptions imgOpt = new ImageOrPrintOptions();
            imgOpt.HorizontalResolution = 300;
            imgOpt.VerticalResolution = 300;
            imgOpt.ImageType = ImageType.Tiff;

            // Testen Sie verschiedene Kompressionstypen
            string outputPath = "output_compression_";

            // LZW-Kompression
            imgOpt.TiffCompression = TiffCompression.CompressionLZW;
            new WorkbookRender(wb, imgOpt).ToImage(outputPath + "LZW.tiff");

            // CCITT3-Kompression
            imgOpt.TiffCompression = TiffCompression.CompressionCCITT3;
            new WorkbookRender(wb, imgOpt).ToImage(outputPath + "CCITT3.tiff");

            // CCITT4-Kompression
            imgOpt.TiffCompression = TiffCompression.CompressionCCITT4;
            new WorkbookRender(wb, imgOpt).ToImage(outputPath + "CCITT4.tiff");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


