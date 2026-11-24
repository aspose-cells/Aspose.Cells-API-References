---
title: "PdfSaveOptions.ExportDocumentStructure"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PdfSaveOptions-Eigenschaft. Gibt an, ob die Dokumentstruktur exportiert werden soll."
type: docs
url: /de/net/aspose.cells/pdfsaveoptions/exportdocumentstructure/
---
## PdfSaveOptions.ExportDocumentStructure property

Gibt an, ob die Dokumentstruktur exportiert werden soll.

```csharp
public bool ExportDocumentStructure { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PdfSaveOptionsPropertyExportDocumentStructureDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten zum Arbeitsblatt hinzufügen
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);

            // PDF-Speicheroptionen erstellen
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            
            // Setze ExportDocumentStructure auf true, um die Dokumentstruktur beizubehalten.
            pdfSaveOptions.ExportDocumentStructure = true;
            
            // Formeln vor dem Speichern berechnen.
            workbook.CalculateFormula();

            // Speichern Sie die Arbeitsmappe als PDF mit den angegebenen Optionen.
            workbook.Save("output.pdf", pdfSaveOptions);

            Console.WriteLine("PDF saved with document structure exported.");
        }
    }
}
```

### Siehe auch

* class [PdfSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


