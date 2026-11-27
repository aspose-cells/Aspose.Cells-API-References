---
title: "Worksheet.Comments"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Worksheet-egenskap. Hämtar Comment-samlingen"
type: docs
url: /sv/net/aspose.cells/worksheet/comments/
---
## Worksheet.Comments property

Hämtar [`Comment`](../../comment/) samlingen.

```csharp
public CommentCollection Comments { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyCommentsDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till kommentarer till celler
            worksheet.Cells["A1"].PutValue("Cell A1");
            int commentIndexA1 = worksheet.Comments.Add("A1");
            worksheet.Comments[commentIndexA1].Note = "Note for A1";

            worksheet.Cells["B1"].PutValue("Cell B1");
            int commentIndexB1 = worksheet.Comments.Add("B1");
            worksheet.Comments[commentIndexB1].Note = "Note for B1";

            worksheet.Cells["C2"].PutValue("Cell C2");
            int commentIndexC2 = worksheet.Comments.Add("C2");
            worksheet.Comments[commentIndexC2].Note = "Note for C2";

            // Spara arbetsboken
            workbook.Save("CommentsDemo.xlsx");
        }
    }
}
```

### Se även

* class [CommentCollection](../../commentcollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


