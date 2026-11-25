---
title: "Comment.IsVisible"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Comment. Rappresenta se il commento è visibile o meno"
type: docs
url: /it/net/aspose.cells/comment/isvisible/
---
## Comment.IsVisible property

Rappresenta se il commento è visibile o meno.

```csharp
public bool IsVisible { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CommentPropertyIsVisibleDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi un commento alla cella A1
            int commentIndex = worksheet.Comments.Add("A1");
            Comment comment = worksheet.Comments[commentIndex];
            comment.Note = "This is a test comment";

            // Imposta il commento come visibile
            comment.IsVisible = true;

            // Verifica se il commento è visibile
            if (comment.IsVisible)
            {
                Console.WriteLine("The comment is visible");
            }

            // Salva la cartella di lavoro
            workbook.Save("CommentVisibilityDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Comment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


