---
title: "PaginatedSaveOptions.CheckFontCompatibility"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété PaginatedSaveOptions. Indique s'il faut vérifier la compatibilité des polices pour chaque caractère du texte"
type: docs
url: /fr/net/aspose.cells/paginatedsaveoptions/checkfontcompatibility/
---
## PaginatedSaveOptions.CheckFontCompatibility property

Indique s'il faut vérifier la compatibilité des polices pour chaque caractère du texte.

```csharp
public bool CheckFontCompatibility { get; set; }
```

### Remarques

La valeur par défaut est true. Désactiver cette propriété peut offrir de meilleures performances. Mais lorsque la police par défaut ou spécifiée du texte/caractère ne peut pas être utilisée pour le rendre, des caractères illisibles (comme des blocs) peuvent apparaître dans le PDF généré. Dans une telle situation, l'utilisateur doit conserver cette propriété à true afin qu'une police alternative puisse être recherchée et utilisée pour rendre le texte à la place ;

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PaginatedSaveOptionsPropertyCheckFontCompatibilityDemo
    {
        public static void Run()
        {
            // Créez un nouveau classeur avec des données d'exemple
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Font Compatibility Test");

            // Créez des options d'enregistrement paginées
            PdfSaveOptions saveOptions = new PdfSaveOptions();
            
            // Démontrez la propriété CheckFontCompatibility
            saveOptions.CheckFontCompatibility = false; // Disable font compatibility checking
            
            // Définissez les autres propriétés requises
            saveOptions.DefaultFont = "Arial";
            saveOptions.CheckWorkbookDefaultFont = true;

            // Enregistrez le document avec les options spécifiées
            workbook.Save("PaginatedSaveOptions_CheckFontCompatibility.pdf", saveOptions);
            
            Console.WriteLine("Document saved with CheckFontCompatibility = false");
        }
    }
}
```

### Voir aussi

* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


