---
title: "PaginatedSaveOptions.TextCrossType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PaginatedSaveOptions‑Eigenschaft. Gibt den Anzeigetexttyp zurück oder legt ihn fest, wenn die Textbreite größer als die Zellenbreite ist."
type: docs
url: /de/net/aspose.cells/paginatedsaveoptions/textcrosstype/
---
## PaginatedSaveOptions.TextCrossType property

Liest oder legt den Anzeigetexttyp fest, wenn die Textbreite größer als die Zellenbreite ist.

```csharp
public TextCrossType TextCrossType { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class PaginatedSaveOptionsPropertyTextCrossTypeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch mit Beispieldaten
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Langen Text festlegen, der Zellen­grenzen überschreitet
            worksheet.Cells["A1"].PutValue("This is a long text that will cross cell boundaries");
            worksheet.Cells["B1"].PutValue("Another cell content");
            
            // Spaltenbreite festlegen, damit Text Zellen überschreitet
            worksheet.Cells.SetColumnWidth(0, 5);
            
            // PDF-Speicheroptionen erstellen
            PdfSaveOptions options = new PdfSaveOptions();
            
            // Demonstrieren Sie TextCrossType, indem Sie es auf CrossKeep setzen
            options.TextCrossType = TextCrossType.CrossKeep;
            
            // Speichern Sie die Arbeitsmappe als PDF
            workbook.Save("TextCrossTypeDemo.pdf", options);
            
            Console.WriteLine("PDF saved with TextCrossType.CrossKeep setting");
        }
    }
}
```

### Siehe auch

* enum [TextCrossType](../../textcrosstype/)
* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


