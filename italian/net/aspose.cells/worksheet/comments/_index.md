---
title: "Worksheet.Comments"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Worksheet. Restituisce la collezione Comment"
type: docs
url: /it/net/aspose.cells/worksheet/comments/
---
## Worksheet.Comments property

Restituisce la collezione [`Comment`](../../comment/).

```csharp
public CommentCollection Comments { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyCommentsDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi commenti alle celle
            worksheet.Cells["A1"].PutValue("Cell A1");
            int commentIndexA1 = worksheet.Comments.Add("A1");
            worksheet.Comments[commentIndexA1].Note = "Note for A1";

            worksheet.Cells["B1"].PutValue("Cell B1");
            int commentIndexB1 = worksheet.Comments.Add("B1");
            worksheet.Comments[commentIndexB1].Note = "Note for B1";

            worksheet.Cells["C2"].PutValue("Cell C2");
            int commentIndexC2 = worksheet.Comments.Add("C2");
            worksheet.Comments[commentIndexC2].Note = "Note for C2";

            // Salva la cartella di lavoro
            workbook.Save("CommentsDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [CommentCollection](../../commentcollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


