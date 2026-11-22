---
title: "التعداد CellValueFormatStrategy"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "التعداد Aspose.Cells.CellValueFormatStrategy. يحدد كيفية تطبيق النمط لقيمة الخلية"
type: docs
url: /ar/net/aspose.cells/cellvalueformatstrategy/
---
## CellValueFormatStrategy enumeration

يحدد كيفية تطبيق النمط على قيمة الخلية.

```csharp
public enum CellValueFormatStrategy
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| None | `0` | غير مُنسَّق. |
| CellStyle | `1` | مُنسَّق فقط باستخدام النمط الأصلي للخلية. |
| DisplayStyle | `2` | مُنسَّق باستخدام النمط المعروض للخلية. |
| DisplayString | `3` | يحصل على السلسلة المعروضة في MS Excel. الاختلاف الرئيسي عن DisplayStyle هو أن هذا الخيار يأخذ أيضًا في الاعتبار تأثير عرض العمود. إذا كان عرض العمود صغيرًا جدًا لعرض السلسلة المُنسَّقة بالكامل، قد يُظهر "#"، كما يحدث في MS Excel. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellValueFormatStrategyDemo
    {
        public static void CellValueFormatStrategyExample()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بعض البيانات النموذجية إلى ورقة العمل
            worksheet.Cells["A1"].PutValue("Date");
            worksheet.Cells["A2"].PutValue(DateTime.Now);
            worksheet.Cells["B1"].PutValue("Number");
            worksheet.Cells["B2"].PutValue(12345.6789);
            worksheet.Cells["C1"].PutValue("Text");
            worksheet.Cells["C2"].PutValue("Hello World");

            // تطبيق استراتيجيات CellValueFormatStrategy المختلفة لعرض تأثيراتها.
            // None: غير مُنسَّق
            string valueNone = worksheet.Cells["A2"].GetStringValue(CellValueFormatStrategy.None);
            Console.WriteLine($"None: {valueNone}");

            // CellStyle: مُنسَّق فقط باستخدام النمط الأصلي للخلية
            string valueCellStyle = worksheet.Cells["A2"].GetStringValue(CellValueFormatStrategy.CellStyle);
            Console.WriteLine($"CellStyle: {valueCellStyle}");

            // DisplayStyle: مُنسَّق باستخدام النمط المعروض للخلية
            string valueDisplayStyle = worksheet.Cells["A2"].GetStringValue(CellValueFormatStrategy.DisplayStyle);
            Console.WriteLine($"DisplayStyle: {valueDisplayStyle}");

            // DisplayString: يحصل على السلسلة المعروضة في MS Excel
            string valueDisplayString = worksheet.Cells["A2"].GetStringValue(CellValueFormatStrategy.DisplayString);
            Console.WriteLine($"DisplayString: {valueDisplayString}");

            // حفظ المصنف إلى ملف
            workbook.Save("CellValueFormatStrategyExample.xlsx");
            workbook.Save("CellValueFormatStrategyExample.pdf");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


