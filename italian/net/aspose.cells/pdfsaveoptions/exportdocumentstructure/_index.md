---
title: "PdfSaveOptions.ExportDocumentStructure"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PdfSaveOptions. Indica se esportare la struttura del documento"
type: docs
url: /it/net/aspose.cells/pdfsaveoptions/exportdocumentstructure/
---
## PdfSaveOptions.ExportDocumentStructure property

Indica se esportare la struttura del documento.

```csharp
public bool ExportDocumentStructure { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PdfSaveOptionsPropertyExportDocumentStructureDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio al foglio di lavoro
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);

            // Crea le opzioni di salvataggio PDF
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            
            // Imposta ExportDocumentStructure su true per mantenere la struttura del documento
            pdfSaveOptions.ExportDocumentStructure = true;
            
            // Calcola le formule prima di salvare
            workbook.CalculateFormula();

            // Salva la cartella di lavoro in PDF con le opzioni specificate
            workbook.Save("output.pdf", pdfSaveOptions);

            Console.WriteLine("PDF saved with document structure exported.");
        }
    }
}
```

### Vedi anche

* class [PdfSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


