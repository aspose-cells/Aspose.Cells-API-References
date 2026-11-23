---
title: "PaginatedSaveOptions.IgnoreError"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PaginatedSaveOptions. Indique si vous devez masquer l'erreur lors du rendu. L'erreur peut être une erreur de rendu de forme, d'image, de graphique, etc."
type: docs
url: /fr/net/aspose.cells/paginatedsaveoptions/ignoreerror/
---
## PaginatedSaveOptions.IgnoreError property

Indique si vous devez masquer l'erreur lors du rendu. L'erreur peut provenir du rendu de formes, d'images, de graphiques, etc.

```csharp
public bool IgnoreError { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PaginatedSaveOptionsPropertyIgnoreErrorDemo
    {
        public static void Run()
        {
            // Créez un nouveau classeur avec des données d'exemple
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajoutez des données d'exemple avec d'éventuelles erreurs de formatage
            worksheet.Cells["A1"].PutValue("Sample Data");
            worksheet.Cells["A2"].PutValue(123);
            worksheet.Cells["A3"].PutValue(DateTime.Now);
            
            // Créez les options d'enregistrement PDF
            PdfSaveOptions options = new PdfSaveOptions();
            
            // Définissez IgnoreError sur true pour ignorer toutes les erreurs de conversion
            options.IgnoreError = true;
            
            // Enregistrez le classeur au format PDF
            workbook.Save("PaginatedSaveWithIgnoreError.pdf", options);
            
            Console.WriteLine("PDF saved with IgnoreError enabled.");
        }
    }
}
```

### Voir aussi

* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


