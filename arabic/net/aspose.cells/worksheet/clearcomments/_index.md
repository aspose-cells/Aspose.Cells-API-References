---
title: "Worksheet.ClearComments"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Worksheet. يمسح جميع التعليقات في جدول البيانات المصمم"
type: docs
url: /ar/net/aspose.cells/worksheet/clearcomments/
---
## Worksheet.ClearComments method

يمسح جميع التعليقات في جدول البيانات المصمم.

```csharp
public void ClearComments()
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodClearCommentsDemo
    {
        public static void Run()
        {
            // إنشاء مصنف
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إضافة تعليقات نموذجية إلى الخلايا باستخدام مراجع الخلايا
            int comment1 = worksheet.Comments.Add("A1");
            worksheet.Comments[comment1].Note = "This is comment 1";
            
            int comment2 = worksheet.Comments.Add("B3");
            worksheet.Comments[comment2].Note = "This is comment 2";
            
            int comment3 = worksheet.Comments.Add("C5");
            worksheet.Comments[comment3].Note = "This is comment 3";

            // عرض عدد التعليقات قبل المسح
            Console.WriteLine($"Comments count before ClearComments(): {worksheet.Comments.Count}");

            // مسح جميع التعليقات من ورقة العمل
            worksheet.ClearComments();

            // عرض عدد التعليقات بعد المسح
            Console.WriteLine($"Comments count after ClearComments(): {worksheet.Comments.Count}");

            // احفظ المصنف
            workbook.Save("ClearCommentsDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### انظر أيضًا

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


