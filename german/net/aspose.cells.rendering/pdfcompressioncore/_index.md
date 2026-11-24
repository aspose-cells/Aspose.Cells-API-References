---
title: "Enum PdfCompressionCore"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Rendering.PdfCompressionCore enum. Gibt einen Kompressionstyp an, der auf alle Inhalte der PDF-Datei außer Bildern angewendet wird."
type: docs
url: /de/net/aspose.cells.rendering/pdfcompressioncore/
---
## PdfCompressionCore enumeration

Gibt einen Kompressionstyp an, der auf alle Inhalte der PDF‑Datei außer Bildern angewendet wird.

```csharp
public enum PdfCompressionCore
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| None | `0` | Keine |
| Rle | `1` | Rle |
| Lzw | `2` | Lzw |
| Flate | `3` | Flate |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class PdfCompressionCoreDemo
    {
        public static void PdfCompressionCoreExample()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Hello Aspose!");

            // Erstellen Sie PdfSaveOptions und setzen Sie die PdfCompressionCore
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            pdfSaveOptions.PdfCompression = PdfCompressionCore.Flate; // Setting the compression type to Flate

            // Speichern Sie die Arbeitsmappe als PDF-Datei mit der angegebenen Kompression
            workbook.Save("PdfCompressionCoreExample.pdf", pdfSaveOptions);

            Console.WriteLine("PDF file saved with specified compression.");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


