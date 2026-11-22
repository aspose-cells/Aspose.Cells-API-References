---
title: "ThreadedCommentAuthorCollection.Add"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة ThreadedCommentAuthorCollection. يضيف شخصًا واحدًا لتعليق الخيط"
type: docs
url: /ar/net/aspose.cells/threadedcommentauthorcollection/add/
---
## ThreadedCommentAuthorCollection.Add method

يضيف شخصًا واحدًا لتعليق السلسلة.

```csharp
public int Add(string name, string userId, string providerId)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| name | String | اسم الشخص. |
| userId | String |  |
| providerId | String | معرف الموفر |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ThreadedCommentAuthorCollectionMethodAddWithStringStringStringDemo
    {
        public static void Run()
        {
            // إنشاء مصنف
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف مؤلف تعليق متسلسل
            int authorIndex = workbook.Worksheets.ThreadedCommentAuthors.Add("Test Author", "testuser", "TA");

            // احصل على المؤلف المضاف
            ThreadedCommentAuthor author = workbook.Worksheets.ThreadedCommentAuthors[authorIndex];

            // أضف تعليقات خيطية باستخدام المؤلف
            worksheet.Comments.AddThreadedComment("C2", "First comment", author);
            worksheet.Comments.AddThreadedComment("C2", "Second comment", author);

            // احفظ المصنف
            workbook.Save("ThreadedCommentsExample.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ThreadedCommentAuthorCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


