---
title: "PdfSaveOptions.OptimizationType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PdfSaveOptions. Obtient et définit le type d'optimisation du pdf"
type: docs
url: /fr/net/aspose.cells/pdfsaveoptions/optimizationtype/
---
## PdfSaveOptions.OptimizationType property

Obtient et définit le type d'optimisation du pdf.

```csharp
public PdfOptimizationType OptimizationType { get; set; }
```

### Remarques

La valeur par défaut est Standard

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class PdfSaveOptionsPropertyOptimizationTypeDemo
    {
        public static void Run()
        {
            // Créez un nouveau classeur avec des données d'exemple
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Aspose.Cells PDF Optimization Example");

            // Créez les options d'enregistrement PDF
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            
            // Démontrer la propriété OptimizationType
            pdfSaveOptions.OptimizationType = PdfOptimizationType.MinimumSize;

            // Enregistrer le classeur avec les paramètres d'optimisation
            workbook.Save("OptimizedPdf.pdf", pdfSaveOptions);
        }
    }
}
```

### Voir aussi

* enum [PdfOptimizationType](../../../aspose.cells.rendering/pdfoptimizationtype/)
* class [PdfSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


