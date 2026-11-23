---
title: "Comment.WidthInch"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Comment propriété. Représente la largeur du commentaire en unités de pouces"
type: docs
url: /fr/net/aspose.cells/comment/widthinch/
---
## Comment.WidthInch property

Représente la largeur du commentaire, en pouces.

```csharp
public double WidthInch { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CommentPropertyWidthInchDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            int commentIndex = worksheet.Comments.Add("A1");
            Comment comment = worksheet.Comments[commentIndex];
            comment.Note = "Sample comment";
            
            comment.WidthInch = 1.5;
            
            Console.WriteLine("Comment width set to: " + comment.WidthInch + " inches");
        }
    }
}
```

### Voir aussi

* class [Comment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


