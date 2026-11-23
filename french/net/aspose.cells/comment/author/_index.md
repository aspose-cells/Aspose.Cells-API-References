---
title: "Comment.Author"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Comment. Obtient et définit le nom de l'auteur original du commentaire"
type: docs
url: /fr/net/aspose.cells/comment/author/
---
## Comment.Author property

Obtient et définit le nom de l'auteur original du commentaire

```csharp
public string Author { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CommentPropertyAuthorDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter un commentaire à la cellule A1
            int commentIndex = worksheet.Comments.Add("A1");
            Comment comment = worksheet.Comments[commentIndex];
            
            // Définir l'auteur du commentaire et la note
            comment.Author = "Carl.Yang";
            comment.Note = "This is a sample comment";

            // Afficher l'auteur du commentaire
            Console.WriteLine("Comment Author: " + comment.Author);
        }
    }
}
```

### Voir aussi

* class [Comment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


