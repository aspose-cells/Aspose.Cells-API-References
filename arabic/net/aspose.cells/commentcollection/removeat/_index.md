---
title: "CommentCollection.RemoveAt"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة CommentCollection. يزيل التعليق للخلية المحددة"
type: docs
url: /ar/net/aspose.cells/commentcollection/removeat/
---
## RemoveAt(string) {#removeat_2}

يزيل التعليق الخاص بالخلية المحددة.

```csharp
public void RemoveAt(string cellName)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| cellName | String | اسم الخلية التي تحتوي على تعليق. |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CommentCollectionMethodRemoveAtWithStringDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // أضف تعليقات إلى الخلايا باستخدام أسماء الخلايا
            int commentIndex1 = worksheet.Comments.Add("A1");
            worksheet.Comments[commentIndex1].Note = "Comment in A1";
            
            int commentIndex2 = worksheet.Comments.Add("B2");
            worksheet.Comments[commentIndex2].Note = "Comment in B2";
            
            int commentIndex3 = worksheet.Comments.Add("C3");
            worksheet.Comments[commentIndex3].Note = "Comment in C3";
            
            // إزالة التعليق في الخلية B2 باستخدام RemoveAt مع معامل نصي
            worksheet.Comments.RemoveAt("B2");
            
            // احفظ المصنف
            workbook.Save("CommentsDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [CommentCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## RemoveAt(int, int) {#removeat_1}

يزيل التعليق الخاص بالخلية المحددة.

```csharp
public void RemoveAt(int row, int column)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| صف | Int32 | فهرس الصف. |
| عمود | Int32 | فهرس العمود. |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CommentCollectionMethodRemoveAtWithInt32Int32Demo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // أضف تعليقات إلى الخلايا باستخدام مراجع الخلايا
            int comment1Index = worksheet.Comments.Add("A1");
            worksheet.Comments[comment1Index].Note = "First comment";
            
            int comment2Index = worksheet.Comments.Add("B2");
            worksheet.Comments[comment2Index].Note = "Second comment";
            
            int comment3Index = worksheet.Comments.Add("C3");
            worksheet.Comments[comment3Index].Note = "Third comment";
            
            // إزالة التعليق في الصف 1، العمود 1 (B2)
            worksheet.Comments.RemoveAt(1, 1);
            
            // احفظ المصنف
            workbook.Save("output.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [CommentCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


