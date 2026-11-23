---
title: "PdfSaveOptions.ExportDocumentStructure"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PdfSaveOptions. Indique si l’on doit exporter la structure du document"
type: docs
url: /fr/net/aspose.cells/pdfsaveoptions/exportdocumentstructure/
---
## PdfSaveOptions.ExportDocumentStructure property

Indique s'il faut exporter la structure du document.

```csharp
public bool ExportDocumentStructure { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PdfSaveOptionsPropertyExportDocumentStructureDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple à la feuille de calcul
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);

            // Créez les options d'enregistrement PDF
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            
            // Définissez ExportDocumentStructure sur true pour conserver la structure du document
            pdfSaveOptions.ExportDocumentStructure = true;
            
            // Calculer les formules avant l’enregistrement
            workbook.CalculateFormula();

            // Enregistrez le classeur au format PDF avec les options spécifiées
            workbook.Save("output.pdf", pdfSaveOptions);

            Console.WriteLine("PDF saved with document structure exported.");
        }
    }
}
```

### Voir aussi

* class [PdfSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


