---
title: "PdfSaveOptions.Compliance"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "PdfSaveOptions property. Obtient ou définit le niveau de conformité aux normes PDF pour les documents de sortie"
type: docs
url: /fr/net/aspose.cells/pdfsaveoptions/compliance/
---
## PdfSaveOptions.Compliance property

Obtient ou définit le niveau de conformité aux normes PDF pour les documents de sortie.

```csharp
public PdfCompliance Compliance { get; set; }
```

### Remarques

La valeur par défaut est Pdf17.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class PdfSaveOptionsPropertyComplianceDemo
    {
        public static void Run()
        {
            // Créer un classeur d'exemple avec des données de test
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Test PDF Compliance");

            // Définir les options d'enregistrement PDF avec la conformité PDF/A-1b
            PdfSaveOptions options = new PdfSaveOptions
            {
                Compliance = PdfCompliance.PdfA1b
            };

            // Enregistrez le classeur au format PDF avec les paramètres de conformité
            workbook.Save("output.pdf", options);
            
            Console.WriteLine("PDF saved with PDF/A-1b compliance.");
        }
    }
}
```

### Voir aussi

* enum [PdfCompliance](../../../aspose.cells.rendering/pdfcompliance/)
* class [PdfSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


