---
title: "Enum PdfFontEncoding"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Rendering.PdfFontEncoding-Enum. Stellt die eingebettete PDF-Schriftkodierung dar"
type: docs
url: /de/net/aspose.cells.rendering/pdffontencoding/
---
## PdfFontEncoding enumeration

Stellt die PDF-eingebettete Schriftkodierung dar.

```csharp
public enum PdfFontEncoding
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| Identity | `0` | Stellt die Verwendung der Identity-H-Kodierung für alle eingebetteten Schriften im PDF dar. |
| AnsiPrefer | `1` | Stellt die bevorzugte Verwendung von WinAnsiEncoding für TrueType-Schriften mit Zeichen 32‑127 dar; andernfalls wird die Identity-H-Kodierung für eingebettete Schriften im PDF verwendet. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class PdfFontEncodingDemo
    {
        public static void PdfFontEncodingExample()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Hello, Aspose!");

            // PdfSaveOptions erstellen und die FontEncoding‑Eigenschaft festlegen
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            pdfSaveOptions.FontEncoding = PdfFontEncoding.AnsiPrefer;

            // Speichern Sie die Arbeitsmappe als PDF-Datei
            workbook.Save("PdfFontEncodingExample.pdf", pdfSaveOptions);

            Console.WriteLine("PDF file created successfully with specified font encoding.");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


