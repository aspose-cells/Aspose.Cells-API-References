---
title: "Workbook.Colors"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Workbook. تُرجع الألوان في لوحة الألوان لجدول البيانات"
type: docs
url: /ar/net/aspose.cells/workbook/colors/
---
## Workbook.Colors property

يرجع الألوان في لوحة الألوان للجدول الإلكتروني.

```csharp
public Color[] Colors { get; }
```

### ملاحظات

لوحة الألوان تحتوي على 56 مدخلًا، كل منها ممثل بقيمة RGB.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class WorkbookPropertyColorsDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();

            // الوصول إلى لوحة الألوان الافتراضية
            Color[] colors = workbook.Colors;

            // تعديل بعض الألوان في لوحة الألوان
            colors[0] = System.Drawing.Color.Red;      // Modify first color to Red
            colors[1] = System.Drawing.Color.Green;    // Modify second color to Green
            colors[2] = System.Drawing.Color.Blue;    // Modify third color to Blue

            // إنشاء ورقة عمل وإضافة بعض البيانات
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Color Demo");
            
            // تطبيق الألوان المعدلة على الخلايا
            Style style1 = workbook.CreateStyle();
            style1.ForegroundColor = colors[0];
            style1.Pattern = BackgroundType.Solid;
            worksheet.Cells["A2"].SetStyle(style1);
            
            Style style2 = workbook.CreateStyle();
            style2.ForegroundColor = colors[1];
            style2.Pattern = BackgroundType.Solid;
            worksheet.Cells["B2"].SetStyle(style2);
            
            Style style3 = workbook.CreateStyle();
            style3.ForegroundColor = colors[2];
            style3.Pattern = BackgroundType.Solid;
            worksheet.Cells["C2"].SetStyle(style3);

            // احفظ المصنف
            workbook.Save("WorkbookColorsDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


