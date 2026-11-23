---
title: "PaginatedSaveOptions.CheckWorkbookDefaultFont"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PaginatedSaveOptions. Lorsque les caractères dans l'Excel sont Unicode et ne sont pas définis avec la police correcte dans le style de cellule, ils peuvent apparaître sous forme de blocs dans le pdfimage. Réglez ceci sur true pour essayer d'utiliser la police par défaut du classeur afin d'afficher ces caractères en premier."
type: docs
url: /fr/net/aspose.cells/paginatedsaveoptions/checkworkbookdefaultfont/
---
## PaginatedSaveOptions.CheckWorkbookDefaultFont property

Lorsque les caractères dans le fichier Excel sont Unicode et ne sont pas définis avec la police correcte dans le style de cellule, ils peuvent apparaître sous forme de blocs dans le PDF, l'image. Réglez ceci sur true pour essayer d'utiliser la police par défaut du classeur afin d'afficher ces caractères en premier.

```csharp
public bool CheckWorkbookDefaultFont { get; set; }
```

### Remarques

La valeur par défaut est vraie.

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PaginatedSaveOptionsPropertyCheckWorkbookDefaultFontDemo
    {
        public static void Run()
        {
            // Créer un classeur d'exemple
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue("Test Content");
            
            // Configurer les options d'enregistrement PDF
            PdfSaveOptions saveOptions = new PdfSaveOptions();
            saveOptions.CheckWorkbookDefaultFont = false;
            
            // Enregistrer en PDF
            workbook.Save("output.pdf", saveOptions);
            
            Console.WriteLine("PDF saved with CheckWorkbookDefaultFont set to false");
        }
    }
}
```

### Voir aussi

* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


