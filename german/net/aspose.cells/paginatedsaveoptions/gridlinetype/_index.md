---
title: "PaginatedSaveOptions.GridlineType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PaginatedSaveOptions-Eigenschaft. Gibt den Gitterlinientyp zurück oder legt ihn fest"
type: docs
url: /de/net/aspose.cells/paginatedsaveoptions/gridlinetype/
---
## PaginatedSaveOptions.GridlineType property

Liest oder legt den Typ der Gitternetzlinien fest.

```csharp
public GridlineType GridlineType { get; set; }
```

### Hinweise

Standard ist der gepunktete Typ.

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class PaginatedSaveOptionsPropertyGridlineTypeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Beispieldaten hinzufügen und Gitterlinien aktivieren
            worksheet.Cells["A1"].PutValue("GridlineType Demo");
            worksheet.Cells["B2"].PutValue(1);
            worksheet.Cells["C3"].PutValue(2);
            worksheet.Cells["D4"].PutValue(3);
            worksheet.IsGridlinesVisible = true;

            // PDF-Speicheroptionen erstellen
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            
            // GridlineType‑Eigenschaft demonstrieren
            pdfSaveOptions.GridlineType = GridlineType.Dotted;

            // Arbeitsmappe mit Gitterlinien speichern
            workbook.Save("GridlineTypeDemo.pdf", pdfSaveOptions);
        }
    }
}
```

### Siehe auch

* enum [GridlineType](../../gridlinetype/)
* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


