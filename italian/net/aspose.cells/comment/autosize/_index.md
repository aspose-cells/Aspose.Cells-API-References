---
title: "Comment.AutoSize"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Comment. Indica se la dimensione del commento viene regolata automaticamente in base al suo contenuto. Nota: in alcuni casi speciali, come l'ambiente Mac, questa impostazione potrebbe non avere effetto. Se questa impostazione non ha effetto, sostituirla con FitToTextSize"
type: docs
url: /it/net/aspose.cells/comment/autosize/
---
## Comment.AutoSize property

Indica se la dimensione del commento viene regolata automaticamente in base al suo contenuto. Nota: in alcuni casi speciali (come l'ambiente Mac), questa impostazione potrebbe non avere effetto. Se questa impostazione non ha effetto, si prega di sostituirla con FitToTextSize().

```csharp
public bool AutoSize { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CommentPropertyAutoSizeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi un commento alla cella A1
            int commentIndex = worksheet.Comments.Add("A1");
            Comment comment = worksheet.Comments[commentIndex];
            comment.Note = "This is a sample comment that will auto-size to fit its content.";

            // Imposta AutoSize su true
            comment.AutoSize = true;

            // Salva la cartella di lavoro
            workbook.Save("CommentAutoSizeDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Comment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


