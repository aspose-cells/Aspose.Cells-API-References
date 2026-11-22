---
title: "CommentCollection.Item"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية CommentCollection. تجلب عنصر Comment عند الفهرس المحدد"
type: docs
url: /ar/net/aspose.cells/commentcollection/item/
---
## CommentCollection indexer (1 of 3)

يجلب عنصر [`Comment`](../../comment/) عند الفهرس المحدد.

```csharp
public Comment this[int index] { get; }
```

| معامل | الوصف |
| --- | --- |
| فهرس | الفهرس الذي يبدأ من الصفر للعنصر. |

### قيمة الإرجاع

العنصر عند الفهرس المحدد.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CommentCollectionPropertyItemDemo1
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف تعليقات إلى الخلايا
            int commentIndex1 = worksheet.Comments.Add("A1");
            int commentIndex2 = worksheet.Comments.Add("B2");
            
            // الوصول إلى التعليقات باستخدام خاصية Item
            Comment comment1 = worksheet.Comments[commentIndex1];
            Comment comment2 = worksheet.Comments[commentIndex2];
            
            // تعيين ملاحظات التعليق
            comment1.Note = "First comment";
            comment2.Note = "Second comment";
            
            // تعديل أول تعليق باستخدام خاصية Item
            worksheet.Comments[0].Note = "Updated first comment";
            
            // الوصول إلى التعليق وتعديله مباشرةً من المجموعة
            Comment comment3 = worksheet.Comments[1];
            comment3.Note = "Updated second comment";
            
            // احفظ المصنف
            workbook.Save("CommentsDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Comment](../../comment/)
* class [CommentCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## CommentCollection indexer (2 of 3)

يجلب عنصر [`Comment`](../../comment/) عند الخلية المحددة.

```csharp
public Comment this[string cellName] { get; }
```

| معامل | الوصف |
| --- | --- |
| cellName | اسم الخلية. |

### قيمة الإرجاع

العنصر عند الخلية المحددة.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CommentCollectionPropertyItemDemo2
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف تعليقات إلى الخلايا باستخدام مراجع الخلايا
            int comment1Index = worksheet.Comments.Add(0, 0); // A1
            worksheet.Comments[comment1Index].Note = "First comment";
            
            int comment2Index = worksheet.Comments.Add(1, 1); // B2
            worksheet.Comments[comment2Index].Note = "Second comment";
            
            int comment3Index = worksheet.Comments.Add(2, 2); // C3
            worksheet.Comments[comment3Index].Note = "Third comment";

            // الوصول إلى التعليقات باستخدام خاصية Item مع مراجع الخلايا
            CommentCollection comments = worksheet.Comments;
            Comment comment1 = comments["A1"];
            Comment comment2 = comments["B2"];
            Comment comment3 = comments["C3"];

            // تعديل ملاحظات التعليق
            comment1.Note = "Updated first note";
            comment2.Note = "Updated second note";
            comment3.Note = "Updated third note";

            // احفظ المصنف
            workbook.Save("CommentsDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Comment](../../comment/)
* class [CommentCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## CommentCollection indexer (3 of 3)

يحصل على عنصر [`Comment`](../../comment/) في فهرس الصف المحدد وفهرس العمود المحدد.

```csharp
public Comment this[int row, int column] { get; }
```

| معامل | الوصف |
| --- | --- |
| صف | فهرس الصف. |
| عمود | فهرس العمود. |

### قيمة الإرجاع

العنصر عند الخلية المحددة.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CommentCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف تعليقات إلى الخلايا باستخدام مراجع الخلايا
            int comment1Index = worksheet.Comments.Add("A1");
            worksheet.Comments[comment1Index].Note = "First comment";

            int comment2Index = worksheet.Comments.Add("B2");
            worksheet.Comments[comment2Index].Note = "Second comment";

            int comment3Index = worksheet.Comments.Add("C3");
            worksheet.Comments[comment3Index].Note = "Third comment";

            // الوصول إلى التعليقات باستخدام خاصية Item مع فهارس الصف/العمود
            CommentCollection comments = worksheet.Comments;
            Comment comment1 = comments[0, 0];
            comment1.Note = "Updated first comment";

            Comment comment2 = comments[1, 1];
            comment2.Note = "Updated second comment";

            // احفظ المصنف
            workbook.Save("CommentsDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Comment](../../comment/)
* class [CommentCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


