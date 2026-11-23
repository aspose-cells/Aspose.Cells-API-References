---
title: "Comment.WidthCM"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Comment propriété. Représente la largeur du commentaire en unités de centimètres"
type: docs
url: /fr/net/aspose.cells/comment/widthcm/
---
## Comment.WidthCM property

Représente la largeur du commentaire, en centimètres.

```csharp
public double WidthCM { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CommentPropertyWidthCMDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            int commentIndex = worksheet.Comments.Add("A1");
            Comment comment = worksheet.Comments[commentIndex];
            comment.Note = "Sample comment";
            comment.WidthCM = 5.0;

            Console.WriteLine($"Comment width set to: {comment.WidthCM} cm");
        }
    }
}
```

### Voir aussi

* class [Comment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


