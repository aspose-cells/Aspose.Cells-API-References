---
title: "Comment.TextOrientationType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Comment. Obtient et définit le type d'orientation du texte du commentaire"
type: docs
url: /fr/net/aspose.cells/comment/textorientationtype/
---
## Comment.TextOrientationType property

Obtient et définit le type d'orientation du texte du commentaire.

```csharp
public TextOrientationType TextOrientationType { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CommentPropertyTextOrientationTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter un commentaire à la cellule A1
            int commentIndex = worksheet.Comments.Add("A1");
            Comment comment = worksheet.Comments[commentIndex];
            comment.Note = "Sample comment text";

            // Définissez l'orientation initiale sur NoRotation
            comment.TextOrientationType = TextOrientationType.NoRotation;
            Console.WriteLine("Initial orientation: " + comment.TextOrientationType);

            // Modifier l'orientation en TopToBottom si elle est actuellement NoRotation
            if (comment.TextOrientationType == TextOrientationType.NoRotation)
            {
                comment.TextOrientationType = TextOrientationType.TopToBottom;
                Console.WriteLine("Changed orientation to: " + comment.TextOrientationType);
            }

            // Enregistrez le classeur
            workbook.Save("CommentOrientationDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [TextOrientationType](../../textorientationtype/)
* class [Comment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


