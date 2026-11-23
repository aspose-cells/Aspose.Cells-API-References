---
title: "Comment.Width"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Comment propriété. Représente la largeur du commentaire en unités de pixels"
type: docs
url: /fr/net/aspose.cells/comment/width/
---
## Comment.Width property

Représente la largeur du commentaire, en pixels.

```csharp
public int Width { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CommentPropertyWidthDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter un commentaire à la cellule A1
            int commentIndex = worksheet.Comments.Add("A1");
            Comment comment = worksheet.Comments[commentIndex];
            
            // Définir les propriétés du commentaire
            comment.Note = "This is a sample comment";
            comment.Width = 200; // Setting the width of the comment box
            comment.Height = 50;
            
            // Enregistrez le classeur
            workbook.Save("CommentWidthDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Comment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


