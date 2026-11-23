---
title: "Comment.TextVerticalAlignment"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Comment. Obtient et définit le type d'alignement vertical du texte du commentaire"
type: docs
url: /fr/net/aspose.cells/comment/textverticalalignment/
---
## Comment.TextVerticalAlignment property

Obtient et définit le type d'alignement vertical du texte du commentaire.

```csharp
public TextAlignmentType TextVerticalAlignment { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CommentPropertyTextVerticalAlignmentDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            int commentIndex = worksheet.Comments.Add("B3");
            Comment comment = worksheet.Comments[commentIndex];
            comment.Note = "Sample comment text";

            // Définir l'alignement vertical sur Fill
            comment.TextVerticalAlignment = TextAlignmentType.Fill;
            Console.WriteLine("Vertical Alignment: " + comment.TextVerticalAlignment);

            // Modifier l'alignement vertical en Center si elle était Fill
            if (comment.TextVerticalAlignment == TextAlignmentType.Fill)
            {
                comment.TextVerticalAlignment = TextAlignmentType.Center;
                Console.WriteLine("Changed Vertical Alignment to: " + comment.TextVerticalAlignment);
            }
        }
    }
}
```

### Voir aussi

* enum [TextAlignmentType](../../textalignmenttype/)
* class [Comment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


