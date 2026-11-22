---
title: "StyleFlag.FontScript"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية StyleFlag. سيتم تطبيق إعداد نص الخط"
type: docs
url: /ar/net/aspose.cells/styleflag/fontscript/
---
## StyleFlag.FontScript property

سيتم تطبيق إعداد نمط الخط.

```csharp
public bool FontScript { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class StyleFlagPropertyFontScriptDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // الوصول إلى الخلية A1 وتعيين بعض النص
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Sample Text");

            // إنشاء كائن نمط وتعيين نص الخط إلى نص سفلي
            Style style = workbook.CreateStyle();
            style.Font.IsSubscript = true;

            // إنشاء علم نمط وتمكين علم FontScript
            StyleFlag styleFlag = new StyleFlag();
            styleFlag.FontScript = true;

            // تطبيق النمط على الخلية باستخدام علم النمط
            cell.SetStyle(style, styleFlag);

            // عرض حالة نص الخط الحالية
            Console.WriteLine("Font is subscript: " + cell.GetStyle().Font.IsSubscript);

            // تغيير نص الخط إلى نص علوي
            style.Font.IsSubscript = false;
            style.Font.IsSuperscript = false;
            cell.SetStyle(style, styleFlag);

            // عرض حالة نص الخط المحدثة
            Console.WriteLine("Font is superscript: " + cell.GetStyle().Font.IsSuperscript);
            Console.WriteLine("Font is subscript: " + cell.GetStyle().Font.IsSubscript);

            // احفظ المصنف
            workbook.Save("StyleFlagPropertyFontScriptDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


