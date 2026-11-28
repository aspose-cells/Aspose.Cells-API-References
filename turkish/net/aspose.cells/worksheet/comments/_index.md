---
title: "Worksheet.Comments"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Worksheet özelliği. Yorum koleksiyonunu alır"
type: docs
url: /tr/net/aspose.cells/worksheet/comments/
---
## Worksheet.Comments property

Alır [`Comment`](../../comment/) koleksiyonunu.

```csharp
public CommentCollection Comments { get; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyCommentsDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Hücrelere yorum ekleyin
            worksheet.Cells["A1"].PutValue("Cell A1");
            int commentIndexA1 = worksheet.Comments.Add("A1");
            worksheet.Comments[commentIndexA1].Note = "Note for A1";

            worksheet.Cells["B1"].PutValue("Cell B1");
            int commentIndexB1 = worksheet.Comments.Add("B1");
            worksheet.Comments[commentIndexB1].Note = "Note for B1";

            worksheet.Cells["C2"].PutValue("Cell C2");
            int commentIndexC2 = worksheet.Comments.Add("C2");
            worksheet.Comments[commentIndexC2].Note = "Note for C2";

            // Çalışma kitabını kaydedin
            workbook.Save("CommentsDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [CommentCollection](../../commentcollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


