---
title: "Comment.Font"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Comment. Obtient la police du commentaire"
type: docs
url: /fr/net/aspose.cells/comment/font/
---
## Comment.Font property

Obtient la police du commentaire.

```csharp
public Font Font { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CommentPropertyFontDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter un commentaire à la cellule A1
            int commentIndex = worksheet.Comments.Add("A1");
            Comment comment = worksheet.Comments[commentIndex];
            comment.Note = "Sample comment";

            // Accéder et modifier les propriétés de police du commentaire
            Aspose.Cells.Font font = comment.Font;
            font.Size = 12;
            font.Name = "Arial";
            font.Color = System.Drawing.Color.Red;
            font.IsBold = true;

            // Enregistrez le classeur
            workbook.Save("CommentFontDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Font](../../font/)
* class [Comment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


