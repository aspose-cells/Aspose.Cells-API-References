---
title: "Enum PrintCommentsType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "Aspose.Cells.PrintCommentsType enum. يمثل الطريقة التي يتم بها طباعة التعليقات مع الورقة"
type: docs
url: /ar/net/aspose.cells/printcommentstype/
---
## PrintCommentsType enumeration

يمثل طريقة طباعة التعليقات مع الورقة.

```csharp
public enum PrintCommentsType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| PrintInPlace | `0` | يمثل طباعة التعليقات كما هي معروضة على الورقة. |
| PrintNoComments | `1` | يمثل عدم طباعة التعليقات. |
| PrintSheetEnd | `2` | يمثل طباعة التعليقات في نهاية الورقة. |
| PrintWithThreadedComments | `3` | يمثل طباعة التعليقات كما هي معروضة على الورقة بما في ذلك التعليقات المتسلسلة. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class PrintCommentsTypeDemo
    {
        public static void PrintCommentsTypeExample()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بعض التعليقات إلى ورقة العمل
            int commentIndex = worksheet.Comments.Add("A1");
            Comment comment = worksheet.Comments[commentIndex];
            comment.Note = "This is a comment.";

            commentIndex = worksheet.Comments.Add("B2");
            comment = worksheet.Comments[commentIndex];
            comment.Note = "This is another comment.";

            // حدد نوع طباعة التعليقات في إعداد الصفحة
            PageSetup pageSetup = worksheet.PageSetup;
            pageSetup.PrintComments = PrintCommentsType.PrintSheetEnd;

            // حفظ المصنف إلى ملف
            workbook.Save("PrintCommentsTypeExample.xlsx");

            Console.WriteLine("Workbook saved successfully with comments printed at the end of the sheet.");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


