---
title: "Font.IsSubscript"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Font. الحصول على أو تعيين قيمة تشير إلى ما إذا كان الخط فرعيًا"
type: docs
url: /ar/net/aspose.cells/font/issubscript/
---
## Font.IsSubscript property

يحصل على أو يضبط قيمة تشير إلى ما إذا كان الخط منخفضًا.

```csharp
public bool IsSubscript { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FontPropertyIsSubscriptDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء نمط بنص فرعي
            Style subscriptStyle = workbook.CreateStyle();
            subscriptStyle.Font.IsSubscript = true;

            // إنشاء نمط بنص مرتفع للمقارنة
            Style superscriptStyle = workbook.CreateStyle();
            superscriptStyle.Font.IsSuperscript = true;

            // تطبيق الأنماط على الخلايا
            worksheet.Cells["A1"].PutValue("Subscript Text");
            worksheet.Cells["A1"].SetStyle(subscriptStyle);

            worksheet.Cells["A2"].PutValue("Superscript Text");
            worksheet.Cells["A2"].SetStyle(superscriptStyle);

            // تحقق وعرض الأنماط
            Console.WriteLine("A1 IsSubscript: " + worksheet.Cells["A1"].GetStyle().Font.IsSubscript);
            Console.WriteLine("A1 IsSuperscript: " + worksheet.Cells["A1"].GetStyle().Font.IsSuperscript);
            Console.WriteLine("A2 IsSubscript: " + worksheet.Cells["A2"].GetStyle().Font.IsSubscript);
            Console.WriteLine("A2 IsSuperscript: " + worksheet.Cells["A2"].GetStyle().Font.IsSuperscript);

            // احفظ المصنف
            workbook.Save("FontPropertyIsSubscriptDemo.ods");
        }
    }
}
```

### انظر أيضًا

* class [Font](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


