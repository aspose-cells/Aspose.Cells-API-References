---
title: "PaginatedSaveOptions.OutputBlankPageWhenNothingToPrint"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PaginatedSaveOptions-Eigenschaft. Gibt an, ob eine leere Seite ausgegeben werden soll, wenn nichts zu drucken ist"
type: docs
url: /de/net/aspose.cells/paginatedsaveoptions/outputblankpagewhennothingtoprint/
---
## PaginatedSaveOptions.OutputBlankPageWhenNothingToPrint property

Gibt an, ob eine leere Seite ausgegeben werden soll, wenn nichts zu drucken ist.

```csharp
public bool OutputBlankPageWhenNothingToPrint { get; set; }
```

### Hinweise

Standard ist true.

### Beispiele

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PaginatedSaveOptionsPropertyOutputBlankPageWhenNothingToPrintDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Ein Arbeitsblatt hinzufügen und ausblenden (simuliert, dass nichts zu drucken ist)
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.IsVisible = false;

            // PDF‑Speicheroptionen festlegen mit OutputBlankPageWhenNothingToPrint = false
            PdfSaveOptions options = new PdfSaveOptions
            {
                OutputBlankPageWhenNothingToPrint = false
            };

            // Als PDF speichern – es sollte keine leere Seite erzeugt werden
            string outputPath = Path.Combine(Environment.GetFolderPath(Environment.SpecialFolder.Desktop), "OutputNoBlankPage.pdf");
            workbook.Save(outputPath, options);

            // Option auf true ändern
            options.OutputBlankPageWhenNothingToPrint = true;

            // Erneut speichern – es sollte eine leere Seite erzeugt werden
            outputPath = Path.Combine(Environment.GetFolderPath(Environment.SpecialFolder.Desktop), "OutputWithBlankPage.pdf");
            workbook.Save(outputPath, options);
        }
    }
}
```

### Siehe auch

* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


