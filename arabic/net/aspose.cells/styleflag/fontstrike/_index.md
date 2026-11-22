---
title: "StyleFlag.FontStrike"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية StyleFlag. سيتم تطبيق إعداد شطب الخط"
type: docs
url: /ar/net/aspose.cells/styleflag/fontstrike/
---
## StyleFlag.FontStrike property

سيتم تطبيق إعداد شطب الخط.

```csharp
public bool FontStrike { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class StyleFlagPropertyFontStrikeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // الوصول إلى الخلية A1 وتعيين بعض النص
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Sample Text");

            // إنشاء كائن نمط وتعيين FontStrike إلى true
            Style style = workbook.CreateStyle();
            style.Font.IsStrikeout = true;

            // إنشاء علامة نمط وتمكين علامة FontStrike
            StyleFlag styleFlag = new StyleFlag();
            styleFlag.FontStrike = true;

            // تطبيق النمط على الخلية باستخدام علم النمط
            cell.SetStyle(style, styleFlag);

            // عرض حالة FontStrike الحالية
            Console.WriteLine("FontStrike applied: " + cell.GetStyle().Font.IsStrikeout);

            // إنشاء خلية أخرى لتوضيح نص غير مشطوب
            Cell cell2 = worksheet.Cells["A2"];
            cell2.PutValue("Normal Text");
            styleFlag.FontStrike = false;

            cell2.SetStyle(style, styleFlag);
            Console.WriteLine("FontStrike applied: " + cell2.GetStyle().Font.IsStrikeout);

            // حفظ المصنف لرؤية التأثيرات
            workbook.Save("PropertyFontStrikeDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


