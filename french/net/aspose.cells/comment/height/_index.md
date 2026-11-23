---
title: "Comment.Height"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Comment. Représente la hauteur du commentaire en pixels"
type: docs
url: /fr/net/aspose.cells/comment/height/
---
## Comment.Height property

Représente la hauteur du commentaire, en pixels.

```csharp
public int Height { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CommentPropertyHeightDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            int commentIndex = worksheet.Comments.Add("A1");
            Comment comment = worksheet.Comments[commentIndex];
            comment.Note = "Sample comment";
            
            // Démontrer la propriété Height
            comment.Height = 100;
            
            Console.WriteLine("Comment height set to: " + comment.Height);
        }
    }
}
```

### Voir aussi

* class [Comment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


