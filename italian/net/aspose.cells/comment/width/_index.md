---
title: "Comment.Width"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Comment. Rappresenta la larghezza del commento in unità di pixel"
type: docs
url: /it/net/aspose.cells/comment/width/
---
## Comment.Width property

Rappresenta la larghezza del commento, in unità di pixel.

```csharp
public int Width { get; set; }
```

### Esempi

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

            // Aggiungi un commento alla cella A1
            int commentIndex = worksheet.Comments.Add("A1");
            Comment comment = worksheet.Comments[commentIndex];
            
            // Imposta le proprietà del commento
            comment.Note = "This is a sample comment";
            comment.Width = 200; // Setting the width of the comment box
            comment.Height = 50;
            
            // Salva la cartella di lavoro
            workbook.Save("CommentWidthDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Comment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


