---
title: "StyleFlag.QuotePrefix"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية StyleFlag. سيتم تطبيق إعداد إخفاء الصيغة"
type: docs
url: /ar/net/aspose.cells/styleflag/quoteprefix/
---
## StyleFlag.QuotePrefix property

سيتم تطبيق إعداد إخفاء الصيغة.

```csharp
public bool QuotePrefix { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class StyleFlagPropertyQuotePrefixDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // الوصول إلى الخلية A1 وتعيين قيمة تبدو كرقم ولكن يجب معالجتها كنص
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("123456");

            // إنشاء نمط وتعيين QuotePrefix إلى true
            Style style = workbook.CreateStyle();
            style.QuotePrefix = true;

            // إنشاء علم نمط وتمكين علم QuotePrefix
            StyleFlag flag = new StyleFlag();
            flag.QuotePrefix = true;

            // تطبيق النمط على الخلية باستخدام SetStyle بدلاً من ApplyStyle
            cell.SetStyle(style, flag);

            // عرض قيمة QuotePrefix الحالية
            Console.WriteLine("Current QuotePrefix value: " + cell.GetStyle().QuotePrefix);

            // حفظ المصنف لرؤية التأثير (سيتم معالجة القيمة كنص في Excel)
            workbook.Save("PropertyQuotePrefixDemo.xlsx");

            // الآن لنقم بتغيير QuotePrefix إلى false ونرى الفرق
            style.QuotePrefix = false;
            cell.SetStyle(style, flag);

            Console.WriteLine("Current QuotePrefix value: " + cell.GetStyle().QuotePrefix);
            // احفظ مرة أخرى باسم مختلف للمقارنة
            workbook.Save("PropertyQuotePrefixDemo_WithoutPrefix.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


