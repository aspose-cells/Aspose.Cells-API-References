---
title: "PaginatedSaveOptions.IgnoreError"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PaginatedSaveOptions-Eigenschaft. Gibt an, ob Sie den Fehler beim Rendern ausblenden müssen. Der Fehler kann ein Fehler beim Rendern von Formen, Bildern, Diagrammen usw. sein"
type: docs
url: /de/net/aspose.cells/paginatedsaveoptions/ignoreerror/
---
## PaginatedSaveOptions.IgnoreError property

Gibt an, ob Sie den Fehler beim Rendern ausblenden müssen. Der Fehler kann ein Fehler bei Formen, Bildern, Diagramm‑Rendern usw. sein.

```csharp
public bool IgnoreError { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PaginatedSaveOptionsPropertyIgnoreErrorDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch mit Beispieldaten
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Einige Beispieldaten mit potenziellen Formatierungsfehlern hinzufügen
            worksheet.Cells["A1"].PutValue("Sample Data");
            worksheet.Cells["A2"].PutValue(123);
            worksheet.Cells["A3"].PutValue(DateTime.Now);
            
            // PDF-Speicheroptionen erstellen
            PdfSaveOptions options = new PdfSaveOptions();
            
            // IgnoreError auf true setzen, um alle Konvertierungsfehler zu überspringen
            options.IgnoreError = true;
            
            // Speichern Sie die Arbeitsmappe als PDF
            workbook.Save("PaginatedSaveWithIgnoreError.pdf", options);
            
            Console.WriteLine("PDF saved with IgnoreError enabled.");
        }
    }
}
```

### Siehe auch

* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


