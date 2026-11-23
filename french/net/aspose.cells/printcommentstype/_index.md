---
title: "Enum PrintCommentsType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.PrintCommentsType enum. Représente la façon dont les commentaires sont imprimés avec la feuille"
type: docs
url: /fr/net/aspose.cells/printcommentstype/
---
## PrintCommentsType enumeration

Représente la façon dont les commentaires sont imprimés avec la feuille.

```csharp
public enum PrintCommentsType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| PrintInPlace | `0` | Représente l'impression des commentaires tels qu'affichés sur la feuille. |
| PrintNoComments | `1` | Représente le fait de ne pas imprimer les commentaires. |
| PrintSheetEnd | `2` | Représente l'impression des commentaires à la fin de la feuille. |
| PrintWithThreadedComments | `3` | Représente l'impression des commentaires tels qu'affichés sur la feuille, y compris les commentaires en fil. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class PrintCommentsTypeDemo
    {
        public static void PrintCommentsTypeExample()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez quelques commentaires à la feuille de calcul
            int commentIndex = worksheet.Comments.Add("A1");
            Comment comment = worksheet.Comments[commentIndex];
            comment.Note = "This is a comment.";

            commentIndex = worksheet.Comments.Add("B2");
            comment = worksheet.Comments[commentIndex];
            comment.Note = "This is another comment.";

            // Définissez le type d'impression des commentaires dans la configuration de la page
            PageSetup pageSetup = worksheet.PageSetup;
            pageSetup.PrintComments = PrintCommentsType.PrintSheetEnd;

            // Enregistrer le classeur dans un fichier
            workbook.Save("PrintCommentsTypeExample.xlsx");

            Console.WriteLine("Workbook saved successfully with comments printed at the end of the sheet.");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


