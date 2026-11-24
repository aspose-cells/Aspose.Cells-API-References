---
title: "PaginatedSaveOptions.PageCount"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PaginatedSaveOptions-Eigenschaft. Gibt die Anzahl der zu speichernden Seiten zurück oder legt sie fest"
type: docs
url: /de/net/aspose.cells/paginatedsaveoptions/pagecount/
---
## PaginatedSaveOptions.PageCount property

Liest oder legt die Anzahl der zu speichernden Seiten fest.

```csharp
public int PageCount { get; set; }
```

### Hinweise

Standard ist System.Int32.MaxValue, was bedeutet, dass alle Seiten gerendert werden..

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PaginatedSaveOptionsPropertyPageCountDemo
    {
        public static void Run()
        {
            // Eine Excel‑Datei öffnen
            Workbook wb = new Workbook("Book1.xlsx");
            
            // PDF-Speicheroptionen initialisieren
            PdfSaveOptions options = new PdfSaveOptions();
            
            // Auf das Drucken von nur 2 Seiten ab Seite 4 (0-basierter Index 3) einstellen
            options.PageIndex = 3;
            options.PageCount = 2;
            
            // Speichern Sie die PDF‑Datei
            wb.Save("output.pdf", options);
            
            Console.WriteLine("PDF saved with selected pages.");
        }
    }
}
```

### Siehe auch

* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


