---
title: "Comment.HeightInch"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Comment propriété. Représente la hauteur du commentaire en unités de pouces"
type: docs
url: /fr/net/aspose.cells/comment/heightinch/
---
## Comment.HeightInch property

Représente la hauteur du commentaire, en pouces.

```csharp
public double HeightInch { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CommentPropertyHeightInchDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            int commentIndex = worksheet.Comments.Add("A1");
            Comment comment = worksheet.Comments[commentIndex];
            
            comment.HeightInch = 1.5;
            Console.WriteLine("Comment height set to: " + comment.HeightInch + " inches");
        }
    }
}
```

### Voir aussi

* class [Comment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


