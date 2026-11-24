---
title: "Enum PrintingPageType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.PrintingPageType Enum. Gibt an, welche Seiten nicht gedruckt werden."
type: docs
url: /de/net/aspose.cells/printingpagetype/
---
## PrintingPageType enumeration

Gibt an, welche Seiten nicht gedruckt werden.

```csharp
public enum PrintingPageType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| Default | `0` | Druckt alle Seiten. |
| IgnoreBlank | `1` | Drucken Sie die Seiten nicht, auf denen die Zellen leer sind. |
| IgnoreStyle | `2` | Drucken Sie die Seiten nicht, die nur Formatierungen enthalten. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class PrintingPageTypeDemo
    {
        public static void PrintingPageTypeExample()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füllen Sie einige Daten im Arbeitsblatt ein
            worksheet.Cells["A1"].PutValue("Hello");
            worksheet.Cells["A2"].PutValue("World");
            worksheet.Cells["A3"].PutValue("!");

            // Erstellen Sie PdfSaveOptions.
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();

            // Setzen Sie den PrintingPageType auf IgnoreBlank.
            pdfSaveOptions.PrintingPageType = PrintingPageType.IgnoreBlank;

            // Speichern Sie die Arbeitsmappe als PDF mit den angegebenen Optionen.
            workbook.Save("output_ignore_blank_page.pdf", pdfSaveOptions);

            // Setzen Sie den PrintingPageType auf IgnoreStyle.
            pdfSaveOptions.PrintingPageType = PrintingPageType.IgnoreStyle;

            // Speichern Sie die Arbeitsmappe als PDF mit den angegebenen Optionen.
            workbook.Save("output_ignore_blank_and_style_page.pdf", pdfSaveOptions);

            // Setzen Sie den PrintingPageType auf Default.
            pdfSaveOptions.PrintingPageType = PrintingPageType.Default;

            // Speichern Sie die Arbeitsmappe als PDF mit den angegebenen Optionen.
            workbook.Save("output_default_page.pdf", pdfSaveOptions);

            return;
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


