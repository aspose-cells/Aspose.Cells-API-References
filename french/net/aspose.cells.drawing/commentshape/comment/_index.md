---
title: "CommentShape.Comment"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété CommentShape. Obtient l'objet commentaire"
type: docs
url: /fr/net/aspose.cells.drawing/commentshape/comment/
---
## CommentShape.Comment property

Obtient l'objet commentaire.

```csharp
public Comment Comment { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class CommentShapePropertyCommentDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter un commentaire à la cellule A1
            int commentIndex = worksheet.Comments.Add("A1");
            Comment comment = worksheet.Comments[commentIndex];
            comment.Note = "This is a sample comment";
            
            // Obtenir la forme de commentaire et démontrer la propriété Comment
            CommentShape commentShape = worksheet.Comments[commentIndex].CommentShape;
            Comment retrievedComment = commentShape.Comment;
            
            // Afficher le texte du commentaire
            Console.WriteLine("Comment Text: " + retrievedComment.Note);
        }
    }
}
```

### Voir aussi

* class [Comment](../../../aspose.cells/comment/)
* class [CommentShape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


