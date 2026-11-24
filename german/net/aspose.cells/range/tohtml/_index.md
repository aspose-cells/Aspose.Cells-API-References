---
title: "Range.ToHtml"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Range-Methode. Konvertiere den Bereich zu HTML"
type: docs
url: /de/net/aspose.cells/range/tohtml/
---
## Range.ToHtml method

Konvertiert den Bereich zu HTML.

```csharp
public byte[] ToHtml(HtmlSaveOptions saveOptions)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| saveOptions | HtmlSaveOptions | Optionen zum Konvertieren des Bereichs zu HTML. |

### Beispiele

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangeMethodToHtmlWithHtmlSaveOptionsDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine Arbeitsmappe mit Beispieldaten
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Fülle einige Daten im Bereich A1:J25
            for (int i = 0; i < 25; i++)
            {
                for (int j = 0; j < 10; j++)
                {
                    worksheet.Cells[i, j].Value = $"Cell {i+1},{j+1}";
                }
            }

            // Erstelle einen Bereich mit vollständig qualifiziertem Typnamen
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1:J25");
            
            // HTML‑Speicheroptionen erstellen
            HtmlSaveOptions options = new HtmlSaveOptions();
            options.ExportImagesAsBase64 = true;
            
            // Konvertiere den Bereich zu HTML
            byte[] htmlData = range.ToHtml(options);
            
            // Speichere HTML in eine Datei
            File.WriteAllBytes("output.html", htmlData);
        }
    }
}
```

### Siehe auch

* class [HtmlSaveOptions](../../htmlsaveoptions/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


