---
title: "PaginatedSaveOptions.TextCrossType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PaginatedSaveOptions. Obtient ou définit le type d'affichage du texte lorsque la largeur du texte est supérieure à la largeur de la cellule"
type: docs
url: /fr/net/aspose.cells/paginatedsaveoptions/textcrosstype/
---
## PaginatedSaveOptions.TextCrossType property

Obtient ou définit le type d'affichage du texte lorsque la largeur du texte dépasse la largeur de la cellule.

```csharp
public TextCrossType TextCrossType { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class PaginatedSaveOptionsPropertyTextCrossTypeDemo
    {
        public static void Run()
        {
            // Créez un nouveau classeur avec des données d'exemple
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Définissez un texte long qui dépassera les limites de la cellule
            worksheet.Cells["A1"].PutValue("This is a long text that will cross cell boundaries");
            worksheet.Cells["B1"].PutValue("Another cell content");
            
            // Définissez la largeur de la colonne pour que le texte traverse les cellules
            worksheet.Cells.SetColumnWidth(0, 5);
            
            // Créez les options d'enregistrement PDF
            PdfSaveOptions options = new PdfSaveOptions();
            
            // Démontrez TextCrossType en le définissant sur CrossKeep
            options.TextCrossType = TextCrossType.CrossKeep;
            
            // Enregistrez le classeur au format PDF
            workbook.Save("TextCrossTypeDemo.pdf", options);
            
            Console.WriteLine("PDF saved with TextCrossType.CrossKeep setting");
        }
    }
}
```

### Voir aussi

* enum [TextCrossType](../../textcrosstype/)
* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


