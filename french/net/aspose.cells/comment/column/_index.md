---
title: "Comment.Column"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Comment propriété. Obtient l'index de colonne du commentaire"
type: docs
url: /fr/net/aspose.cells/comment/column/
---
## Comment.Column property

Obtient l'index de colonne du commentaire.

```csharp
public int Column { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CommentPropertyColumnDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter un commentaire à la cellule B5 (index de colonne 1)
            int commentRow = 4;
            int commentColumn = 1;
            Comment comment = worksheet.Comments[worksheet.Comments.Add(commentRow, commentColumn)];

            // Définir le texte du commentaire
            comment.Note = "This is a sample comment";

            // Démontrez l’utilisation de la propriété Column
            Console.WriteLine("Comment is in column: " + comment.Column);

            // Vérifier que l'index de colonne correspond à l'endroit où nous l'avons placé
            if (comment.Column == commentColumn)
            {
                Console.WriteLine("Column property correctly returns the comment's column index");
            }
        }
    }
}
```

### Voir aussi

* class [Comment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


