---
title: "Énumération PdfOptimizationType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.Rendering.PdfOptimizationType enum. Spécifie un type d'optimisation"
type: docs
url: /fr/net/aspose.cells.rendering/pdfoptimizationtype/
---
## PdfOptimizationType enumeration

Spécifie un type d'optimisation.

```csharp
public enum PdfOptimizationType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| Standard | `0` | Qualité d'impression élevée |
| MinimumSize | `1` | La taille du fichier est plus importante que la qualité d'impression |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class PdfOptimizationTypeDemo
    {
        public static void PdfOptimizationTypeExample()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Hello World");

            // Créez PdfSaveOptions et définissez le type d'optimisation
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            pdfSaveOptions.OptimizationType = PdfOptimizationType.MinimumSize;

            // Enregistrez le classeur au format PDF avec le type d'optimisation spécifié
            workbook.Save("OptimizedOutput.pdf", pdfSaveOptions);

            Console.WriteLine("PDF saved with optimization type: MinimumSize");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


