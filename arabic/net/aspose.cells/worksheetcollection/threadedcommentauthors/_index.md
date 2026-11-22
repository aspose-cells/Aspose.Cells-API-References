---
title: "WorksheetCollection.ThreadedCommentAuthors"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية WorksheetCollection. تحصل على قائمة مؤلفي التعليقات المتسلسلة"
type: docs
url: /ar/net/aspose.cells/worksheetcollection/threadedcommentauthors/
---
## WorksheetCollection.ThreadedCommentAuthors property

يحصل على قائمة مؤلفي التعليقات المتسلسلة.

```csharp
public ThreadedCommentAuthorCollection ThreadedCommentAuthors { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionPropertyThreadedCommentAuthorsDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف مؤلف تعليق متسلسل
            int authorIndex = workbook.Worksheets.ThreadedCommentAuthors.Add("Demo Author", "demo", "DA");

            // احصل على المؤلف الذي أضفناه للتو
            ThreadedCommentAuthor author = workbook.Worksheets.ThreadedCommentAuthors[authorIndex];

            // أضف تعليقات متسلسلة إلى الخلية C2
            AddThreadedComment(worksheet, "C2", "First comment", author);
            AddThreadedComment(worksheet, "C2", "Second comment", author);
            AddThreadedComment(worksheet, "C2", "Third comment", author);

            // احفظ المصنف
            workbook.Save("ThreadedCommentsDemo.xlsx");
        }

        private static void AddThreadedComment(Worksheet worksheet, string cellName, string text, ThreadedCommentAuthor author)
        {
            // احصل على الخلية التي نريد إضافة التعليق إليها
            Cell cell = worksheet.Cells[cellName];
            
            // أضف تعليقًا متسلسلًا (يرجع void، وليس ThreadedComment)
            worksheet.Comments.AddThreadedComment(cellName, text, author);
        }
    }
}
```

### انظر أيضًا

* class [ThreadedCommentAuthorCollection](../../threadedcommentauthorcollection/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


