---
title: "Comment.Row"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Comment. Obtient l'indice de ligne du commentaire"
type: docs
url: /fr/net/aspose.cells/comment/row/
---
## Comment.Row property

Obtient l'index de ligne du commentaire.

```csharp
public int Row { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CommentPropertyRowDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter un commentaire à la cellule A1
            int commentIndex = worksheet.Comments.Add("A1");
            Comment comment1 = worksheet.Comments[commentIndex];
            comment1.Note = "This is a sample comment";

            // Obtenir et afficher l'indice de ligne de la cellule commentée
            int row = comment1.Row;
            Console.WriteLine("The comment is in row: " + row);

            // Ajouter un autre commentaire à la cellule B3
            commentIndex = worksheet.Comments.Add("B3");
            Comment comment2 = worksheet.Comments[commentIndex];
            comment2.Note = "Another comment";

            // Afficher l'indice de ligne du deuxième commentaire
            Console.WriteLine("Second comment is in row: " + comment2.Row);
        }
    }
}
```

### Voir aussi

* class [Comment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


