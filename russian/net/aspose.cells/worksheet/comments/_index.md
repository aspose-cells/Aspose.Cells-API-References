---
title: "Worksheet.Comments"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Worksheet. Возвращает коллекцию Comment"
type: docs
url: /ru/net/aspose.cells/worksheet/comments/
---
## Worksheet.Comments property

Возвращает коллекцию [`Comment`](../../comment/).

```csharp
public CommentCollection Comments { get; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyCommentsDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавьте комментарии в ячейки
            worksheet.Cells["A1"].PutValue("Cell A1");
            int commentIndexA1 = worksheet.Comments.Add("A1");
            worksheet.Comments[commentIndexA1].Note = "Note for A1";

            worksheet.Cells["B1"].PutValue("Cell B1");
            int commentIndexB1 = worksheet.Comments.Add("B1");
            worksheet.Comments[commentIndexB1].Note = "Note for B1";

            worksheet.Cells["C2"].PutValue("Cell C2");
            int commentIndexC2 = worksheet.Comments.Add("C2");
            worksheet.Comments[commentIndexC2].Note = "Note for C2";

            // Сохраните книгу
            workbook.Save("CommentsDemo.xlsx");
        }
    }
}
```

### См. также

* class [CommentCollection](../../commentcollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


