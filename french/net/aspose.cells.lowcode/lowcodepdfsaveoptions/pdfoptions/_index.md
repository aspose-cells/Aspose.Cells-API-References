---
title: "LowCodePdfSaveOptions.PdfOptions"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété LowCodePdfSaveOptions. Les options pour enregistrer le fichier PDF"
type: docs
url: /fr/net/aspose.cells.lowcode/lowcodepdfsaveoptions/pdfoptions/
---
## LowCodePdfSaveOptions.PdfOptions property

Les options pour enregistrer le fichier PDF.

```csharp
public PdfSaveOptions PdfOptions { get; set; }
```

### Exemples

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Rendering;
using Aspose.Cells.LowCode;

namespace AsposeCellsExamples
{
    public class LowCodePdfSaveOptionsPropertyPdfOptionsDemo
    {
        public static void Run()
        {
            // Créer un classeur d'exemple
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("PDF Options Demo");

            // Créer des options d'enregistrement PDF avec des paramètres personnalisés
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions
            {
                Compliance = PdfCompliance.PdfA1b,
                OnePagePerSheet = true
            };

            // Créer des options d'enregistrement PDF low code et assigner les options PDF
            LowCodePdfSaveOptions lowCodePdfSaveOptions = new LowCodePdfSaveOptions
            {
                OutputFile = "output.pdf",
                PdfOptions = pdfSaveOptions
            };

            // Enregistrer en utilisant les options low code
            workbook.Save(lowCodePdfSaveOptions.OutputFile, lowCodePdfSaveOptions.PdfOptions);

            Console.WriteLine("PDF saved with custom options.");
        }
    }
}
```

### Voir aussi

* class [PdfSaveOptions](../../../aspose.cells/pdfsaveoptions/)
* class [LowCodePdfSaveOptions](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


