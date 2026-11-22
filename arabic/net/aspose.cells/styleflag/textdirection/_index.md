---
title: "StyleFlag.TextDirection"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية StyleFlag. سيتم تطبيق إعداد اتجاه النص"
type: docs
url: /ar/net/aspose.cells/styleflag/textdirection/
---
## StyleFlag.TextDirection property

سيتم تطبيق إعداد اتجاه النص.

```csharp
public bool TextDirection { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class StyleFlagPropertyTextDirectionDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // الوصول إلى الخلية A1 وتعيين بعض النص
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Sample Text with TextDirection");

            // إنشاء نمط وتحديد اتجاه النص
            Style style = workbook.CreateStyle();
            style.TextDirection = TextDirectionType.Context;

            // إنشاء علامة نمط وتمكين علامة TextDirection
            StyleFlag styleFlag = new StyleFlag();
            styleFlag.TextDirection = true;

            // تطبيق النمط على الخلية باستخدام علم النمط
            cell.SetStyle(style, styleFlag);

            // عرض اتجاه النص الحالي
            Console.WriteLine("Current TextDirection value: " + cell.GetStyle().TextDirection);

            // تغيير اتجاه النص وتطبيقه مرة أخرى
            style.TextDirection = TextDirectionType.LeftToRight;
            cell.SetStyle(style, styleFlag);

            Console.WriteLine("Current TextDirection value: " + cell.GetStyle().TextDirection);

            // احفظ المصنف
            workbook.Save("TextDirectionDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


