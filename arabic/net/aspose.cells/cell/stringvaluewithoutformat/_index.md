---
title: "Cell.StringValueWithoutFormat"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية الخلية. تحصل على قيمة الخلية كسلسلة نصية دون أي تنسيق"
type: docs
url: /ar/net/aspose.cells/cell/stringvaluewithoutformat/
---
## Cell.StringValueWithoutFormat property

يحصل على قيمة الخلية كسلسلة نصية دون أي تنسيق.

```csharp
[Obsolete("Use GetStringValue(CellValueFormatStrategy) with CellValueFormatStrategy.None instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public string StringValueWithoutFormat { get; }
```

### ملاحظات

ملاحظة: هذه الطريقة أصبحت الآن مهجورة. بدلاً من ذلك، يجب على المستخدم الحصول على كائن القيمة وتنسيقه وفقًا لنوع القيمة والمتطلبات المحددة. سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ ديسمبر 2020. تُعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellPropertyStringValueWithoutFormatDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();

            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة أنواع مختلفة من البيانات لتوضيح StringValueWithoutFormat
            worksheet.Cells["A1"].PutValue("Plain Text");
            worksheet.Cells["A2"].PutValue(12345);
            worksheet.Cells["A3"].PutValue(3.14159);
            worksheet.Cells["A4"].PutValue(DateTime.Now);

            // تطبيق تنسيق الأرقام على بعض الخلايا
            Style style = worksheet.Cells["A2"].GetStyle();
            style.Number = 3; // Currency format
            worksheet.Cells["A2"].SetStyle(style);

            style = worksheet.Cells["A3"].GetStyle();
            style.Number = 9; // Percentage format
            worksheet.Cells["A3"].SetStyle(style);

            try
            {
                // عرض StringValueWithoutFormat لكل خلية
                Console.WriteLine("A1 StringValueWithoutFormat: " + worksheet.Cells["A1"].StringValueWithoutFormat);
                Console.WriteLine("A2 StringValueWithoutFormat: " + worksheet.Cells["A2"].StringValueWithoutFormat);
                Console.WriteLine("A3 StringValueWithoutFormat: " + worksheet.Cells["A3"].StringValueWithoutFormat);
                Console.WriteLine("A4 StringValueWithoutFormat: " + worksheet.Cells["A4"].StringValueWithoutFormat);

                // قارن مع StringValue المنسق
                Console.WriteLine("\nComparison with formatted values:");
                Console.WriteLine("A2 StringValue (formatted): " + worksheet.Cells["A2"].StringValue);
                Console.WriteLine("A3 StringValue (formatted): " + worksheet.Cells["A3"].StringValue);

                // احفظ المصنف
                workbook.Save("StringValueWithoutFormatDemo.xlsx");
                Console.WriteLine("\nWorkbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


