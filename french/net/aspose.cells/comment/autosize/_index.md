---
title: "Comment.AutoSize"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Comment propriété. Indique si la taille du commentaire est ajustée automatiquement en fonction de son contenu. Remarque : dans certains cas particuliers, comme l'environnement Mac, ce paramètre peut ne pas prendre effet. Si ce paramètre ne prend pas effet, veuillez le remplacer par FitToTextSize"
type: docs
url: /fr/net/aspose.cells/comment/autosize/
---
## Comment.AutoSize property

Indique si la taille du commentaire est ajustée automatiquement en fonction de son contenu. Remarque : dans certains cas particuliers (comme l'environnement Mac), ce paramètre peut ne pas prendre effet. Si ce paramètre ne prend pas effet, veuillez le remplacer par FitToTextSize().

```csharp
public bool AutoSize { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CommentPropertyAutoSizeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter un commentaire à la cellule A1
            int commentIndex = worksheet.Comments.Add("A1");
            Comment comment = worksheet.Comments[commentIndex];
            comment.Note = "This is a sample comment that will auto-size to fit its content.";

            // Définir AutoSize sur true
            comment.AutoSize = true;

            // Enregistrez le classeur
            workbook.Save("CommentAutoSizeDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Comment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


