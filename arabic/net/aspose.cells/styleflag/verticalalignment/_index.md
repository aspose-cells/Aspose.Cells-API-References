---
title: "StyleFlag.VerticalAlignment"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية StyleFlag. سيتم تطبيق إعداد المحاذاة العمودية"
type: docs
url: /ar/net/aspose.cells/styleflag/verticalalignment/
---
## StyleFlag.VerticalAlignment property

سيتم تطبيق إعداد المحاذاة العمودية.

```csharp
public bool VerticalAlignment { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class StyleFlagPropertyVerticalAlignmentDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // إنشاء نمط مع محاذاة عمودية
            Style style = workbook.CreateStyle();
            style.VerticalAlignment = TextAlignmentType.Center;
            style.HorizontalAlignment = TextAlignmentType.Center;
            style.Font.Color = Color.Blue;

            // إنشاء علم نمط لتطبيق المحاذاة العمودية ولون الخط فقط
            StyleFlag styleFlag = new StyleFlag();
            styleFlag.VerticalAlignment = true;
            styleFlag.FontColor = true;

            // تطبيق النمط على الصف الأول باستخدام علم النمط
            Row row = sheet.Cells.Rows[0];
            row.ApplyStyle(style, styleFlag);

            // تعيين بعض النصوص في الخلايا لرؤية التأثير
            sheet.Cells["A1"].PutValue("Vertically Centered");
            sheet.Cells["B1"].PutValue("Blue Text");

            // احفظ المصنف
            workbook.Save("VerticalAlignmentDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


