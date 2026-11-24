---
title: "Worksheet.Comments"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Worksheet‑Eigenschaft. Gibt die Comment‑Sammlung zurück"
type: docs
url: /de/net/aspose.cells/worksheet/comments/
---
## Worksheet.Comments property

Gibt die [`Comment`](../../comment/)‑Sammlung zurück.

```csharp
public CommentCollection Comments { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyCommentsDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Kommentare zu Zellen hinzufügen
            worksheet.Cells["A1"].PutValue("Cell A1");
            int commentIndexA1 = worksheet.Comments.Add("A1");
            worksheet.Comments[commentIndexA1].Note = "Note for A1";

            worksheet.Cells["B1"].PutValue("Cell B1");
            int commentIndexB1 = worksheet.Comments.Add("B1");
            worksheet.Comments[commentIndexB1].Note = "Note for B1";

            worksheet.Cells["C2"].PutValue("Cell C2");
            int commentIndexC2 = worksheet.Comments.Add("C2");
            worksheet.Comments[commentIndexC2].Note = "Note for C2";

            // Speichere die Arbeitsmappe
            workbook.Save("CommentsDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [CommentCollection](../../commentcollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


