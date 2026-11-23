---
title: "PaginatedSaveOptions.PageIndex"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PaginatedSaveOptions. Obtient ou définit l'index de base 0 de la première page à enregistrer"
type: docs
url: /fr/net/aspose.cells/paginatedsaveoptions/pageindex/
---
## PaginatedSaveOptions.PageIndex property

Obtient ou définit l'index basé sur zéro de la première page à enregistrer.

```csharp
public int PageIndex { get; set; }
```

### Remarques

La valeur par défaut est 0.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PaginatedSaveOptionsPropertyPageIndexDemo
    {
        public static void Run()
        {
            // Créez un nouveau classeur avec des données d'exemple
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            
            // Ajoutez des données d'exemple sur plusieurs pages
            for (int i = 0; i < 100; i++)
            {
                sheet.Cells[i, 0].Value = "Data " + (i + 1);
            }

            // Définissez les options d'enregistrement PDF
            PdfSaveOptions options = new PdfSaveOptions();
            
            // Définissez l'impression des pages 3-4 (index à base 0)
            options.PageIndex = 2;  // Third page (index 2)
            options.PageCount = 2; // Print 2 pages
            
            // Enregistrez le PDF avec les pages sélectionnées
            wb.Save("SelectedPages.pdf", options);
            
            Console.WriteLine("PDF with pages 3-4 created successfully.");
        }
    }
}
```

### Voir aussi

* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


