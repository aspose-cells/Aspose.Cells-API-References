---
title: "PaginatedSaveOptions.OnePagePerSheet"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PaginatedSaveOptions‑Eigenschaft. Wenn OnePagePerSheet true ist, wird der gesamte Inhalt eines Blatts nur auf einer Seite im Ergebnis ausgegeben. Die Papiergröße der Seiten­einrichtung ist dann ungültig, während die anderen Einstellungen der Seiten­einrichtung weiterhin wirksam bleiben"
type: docs
url: /de/net/aspose.cells/paginatedsaveoptions/onepagepersheet/
---
## PaginatedSaveOptions.OnePagePerSheet property

Ist OnePagePerSheet true, wird der gesamte Inhalt eines Blatts im Ergebnis nur auf einer Seite ausgegeben. Die Papiergröße der Seiten­einstellungen wird ungültig, während die anderen Einstellungen der Seiten­einstellungen weiterhin wirksam bleiben.

```csharp
public bool OnePagePerSheet { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PaginatedSaveOptionsPropertyOnePagePerSheetDemo
    {
        public static void Run()
        {
            // Erstelle eine Beispielarbeitsmappe mit Testdaten
            Workbook workbook = new Workbook();
            Worksheet sheet1 = workbook.Worksheets[0];
            Worksheet sheet2 = workbook.Worksheets.Add("Sheet2");
            
            // Einige Beispieldaten zu beiden Blättern hinzufügen
            for (int i = 0; i < 10; i++)
            {
                sheet1.Cells[i, 0].Value = $"Sheet1 Data {i + 1}";
                sheet2.Cells[i, 0].Value = $"Sheet2 Data {i + 1}";
            }

            // PDF‑Speicheroptionen mit OnePagePerSheet festlegen
            PdfSaveOptions options = new PdfSaveOptions();
            options.OnePagePerSheet = true;

            // Arbeitsmappe als PDF speichern
            workbook.Save("output.pdf", options);
        }
    }
}
```

### Siehe auch

* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


