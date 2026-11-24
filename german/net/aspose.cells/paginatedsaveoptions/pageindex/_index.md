---
title: "PaginatedSaveOptions.PageIndex"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PaginatedSaveOptions-Eigenschaft. Gibt den nullbasierten Index der ersten zu speichernden Seite zurück oder legt ihn fest"
type: docs
url: /de/net/aspose.cells/paginatedsaveoptions/pageindex/
---
## PaginatedSaveOptions.PageIndex property

Liest oder legt den nullbasierten Index der ersten zu speichernden Seite fest.

```csharp
public int PageIndex { get; set; }
```

### Hinweise

Standard ist 0.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PaginatedSaveOptionsPropertyPageIndexDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch mit Beispieldaten
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            
            // Beispieldaten über mehrere Seiten hinzufügen
            for (int i = 0; i < 100; i++)
            {
                sheet.Cells[i, 0].Value = "Data " + (i + 1);
            }

            // PDF-Speicheroptionen festlegen
            PdfSaveOptions options = new PdfSaveOptions();
            
            // Auf das Drucken der Seiten 3‑4 (nullbasierter Index) einstellen
            options.PageIndex = 2;  // Third page (index 2)
            options.PageCount = 2; // Print 2 pages
            
            // PDF mit den ausgewählten Seiten speichern
            wb.Save("SelectedPages.pdf", options);
            
            Console.WriteLine("PDF with pages 3-4 created successfully.");
        }
    }
}
```

### Siehe auch

* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


