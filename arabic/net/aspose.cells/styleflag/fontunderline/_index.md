---
title: "StyleFlag.FontUnderline"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية StyleFlag. سيتم تطبيق إعداد تسطير الخط"
type: docs
url: /ar/net/aspose.cells/styleflag/fontunderline/
---
## StyleFlag.FontUnderline property

سيتم تطبيق إعداد تسطير الخط.

```csharp
public bool FontUnderline { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class StyleFlagPropertyFontUnderlineDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // الوصول إلى الخلية A1 وتعيين بعض النص
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Sample Text with Underline");

            // إنشاء كائن نمط وتعيين تسطير الخط
            Style style = workbook.CreateStyle();
            style.Font.Underline = FontUnderlineType.Single;

            // إنشاء علم نمط وتمكين علم تسطير الخط
            StyleFlag styleFlag = new StyleFlag();
            styleFlag.FontUnderline = true;

            // تطبيق النمط على الخلية باستخدام علم النمط
            cell.SetStyle(style, styleFlag);

            // عرض حالة التسطير الحالية
            Console.WriteLine("Current FontUnderline status: " + cell.GetStyle().Font.Underline);

            // تغيير نوع التسطير إلى مزدوج
            style.Font.Underline = FontUnderlineType.Double;
            cell.SetStyle(style, styleFlag);

            Console.WriteLine("Current FontUnderline status: " + cell.GetStyle().Font.Underline);

            // احفظ المصنف
            workbook.Save("FontUnderlineDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


