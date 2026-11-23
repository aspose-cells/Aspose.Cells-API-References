---
title: "PaginatedSaveOptions.PageCount"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PaginatedSaveOptions. Obtient ou définit le nombre de pages à enregistrer"
type: docs
url: /fr/net/aspose.cells/paginatedsaveoptions/pagecount/
---
## PaginatedSaveOptions.PageCount property

Obtient ou définit le nombre de pages à enregistrer.

```csharp
public int PageCount { get; set; }
```

### Remarques

Par défaut, c'est System.Int32.MaxValue, ce qui signifie que toutes les pages seront rendues..

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PaginatedSaveOptionsPropertyPageCountDemo
    {
        public static void Run()
        {
            // Ouvrez un fichier Excel
            Workbook wb = new Workbook("Book1.xlsx");
            
            // Initialisez les options d'enregistrement PDF
            PdfSaveOptions options = new PdfSaveOptions();
            
            // Définissez l'impression sur seulement 2 pages à partir de la page 4 (indice basé sur 0 = 3)
            options.PageIndex = 3;
            options.PageCount = 2;
            
            // Enregistrer le fichier PDF
            wb.Save("output.pdf", options);
            
            Console.WriteLine("PDF saved with selected pages.");
        }
    }
}
```

### Voir aussi

* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


