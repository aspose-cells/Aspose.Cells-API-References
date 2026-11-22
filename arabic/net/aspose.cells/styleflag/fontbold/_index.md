---
title: "StyleFlag.FontBold"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية StyleFlag. سيتم تطبيق إعداد الخط العريض"
type: docs
url: /ar/net/aspose.cells/styleflag/fontbold/
---
## StyleFlag.FontBold property

سيتم تطبيق إعداد الخط العريض.

```csharp
public bool FontBold { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StyleFlagPropertyFontBoldDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء نمط عريض
            Style boldStyle = workbook.CreateStyle();
            boldStyle.Font.IsBold = true;

            // تطبيق النمط العريض على الصف 2 باستخدام StyleFlag لخاصية FontBold فقط
            worksheet.Cells.ApplyRowStyle(1, boldStyle, new StyleFlag { FontBold = true });

            // وضع قيمة في الخلية لتوضيح النمط
            worksheet.Cells[1, 0].PutValue("Bold Text");

            // احفظ المصنف
            workbook.Save("output.xlsx");

            Console.WriteLine("FontBold property demo completed successfully.");
        }
    }
}
```

### انظر أيضًا

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


