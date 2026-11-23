---
title: "PaginatedSaveOptions.OutputBlankPageWhenNothingToPrint"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PaginatedSaveOptions. Indique s'il faut générer une page blanche lorsqu'il n'y a rien à imprimer"
type: docs
url: /fr/net/aspose.cells/paginatedsaveoptions/outputblankpagewhennothingtoprint/
---
## PaginatedSaveOptions.OutputBlankPageWhenNothingToPrint property

Indique s'il faut générer une page blanche lorsqu'il n'y a rien à imprimer.

```csharp
public bool OutputBlankPageWhenNothingToPrint { get; set; }
```

### Remarques

La valeur par défaut est vraie.

### Exemples

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
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Ajoutez une feuille de calcul et masquez‑la (simulant l'absence d'impression)
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.IsVisible = false;

            // Définissez les options d'enregistrement PDF avec OutputBlankPageWhenNothingToPrint = false
            PdfSaveOptions options = new PdfSaveOptions
            {
                OutputBlankPageWhenNothingToPrint = false
            };

            // Enregistrez en PDF - aucune page blanche ne doit être générée
            string outputPath = Path.Combine(Environment.GetFolderPath(Environment.SpecialFolder.Desktop), "OutputNoBlankPage.pdf");
            workbook.Save(outputPath, options);

            // Modifiez l'option à vrai
            options.OutputBlankPageWhenNothingToPrint = true;

            // Enregistrer à nouveau - une page vierge doit être générée
            outputPath = Path.Combine(Environment.GetFolderPath(Environment.SpecialFolder.Desktop), "OutputWithBlankPage.pdf");
            workbook.Save(outputPath, options);
        }
    }
}
```

### Voir aussi

* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


