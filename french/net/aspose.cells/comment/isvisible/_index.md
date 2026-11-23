---
title: "Comment.IsVisible"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Comment. Représente si le commentaire est visible ou non"
type: docs
url: /fr/net/aspose.cells/comment/isvisible/
---
## Comment.IsVisible property

Indique si le commentaire est visible ou non.

```csharp
public bool IsVisible { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CommentPropertyIsVisibleDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter un commentaire à la cellule A1
            int commentIndex = worksheet.Comments.Add("A1");
            Comment comment = worksheet.Comments[commentIndex];
            comment.Note = "This is a test comment";

            // Définir le commentaire comme visible
            comment.IsVisible = true;

            // Vérifier si le commentaire est visible
            if (comment.IsVisible)
            {
                Console.WriteLine("The comment is visible");
            }

            // Enregistrez le classeur
            workbook.Save("CommentVisibilityDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Comment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


