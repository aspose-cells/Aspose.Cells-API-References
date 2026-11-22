---
title: "Name.Comment"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Name. تحصل وتعيّن تعليق الاسم. ينطبق فقط على Excel 2007 أو الإصدارات الأحدث"
type: docs
url: /ar/net/aspose.cells/name/comment/
---
## Name.Comment property

يحصل على تعليق الاسم ويضبطه. ينطبق فقط على Excel 2007 أو الإصدارات الأحدث.

```csharp
public string Comment { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class NamePropertyCommentDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // أضف نطاقًا مسمىً مع تعليق
            int index = workbook.Worksheets.Names.Add("TestRange");
            Name namedRange = workbook.Worksheets.Names[index];
            namedRange.RefersTo = "=Sheet1!$A$1:$B$2";
            namedRange.Comment = "This is a test named range";
            
            // احفظ المصنف
            workbook.Save("NamedRangeWithComment.xlsx");
            
            // حمّل المصنف المحفوظ للتحقق من التعليق
            Workbook loadedWorkbook = new Workbook("NamedRangeWithComment.xlsx");
            Name loadedNamedRange = loadedWorkbook.Worksheets.Names[0];
            
            // أخرج التعليق لإظهار الوظيفة
            Console.WriteLine("Named Range Comment: " + loadedNamedRange.Comment);
        }
    }
}
```

### انظر أيضًا

* class [Name](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


