---
title: "Validation.GetListValue"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Validation. الحصول على القيمة لقائمة التحقق للخلية المحددة"
type: docs
url: /ar/net/aspose.cells/validation/getlistvalue/
---
## Validation.GetListValue method

احصل على القيمة لقائمة التحقق للخلية المحددة.

```csharp
public object GetListValue(int row, int column)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| صف | Int32 | فهرس الصف. |
| عمود | Int32 | فهرس العمود. |

### قيمة الإرجاع

القيمة لإنتاج قائمة هذا التحقق للخلية المحددة. إذا كانت القائمة تشير إلى نطاق، فستكون القيمة المرتجعة كائنًا [`ReferredArea`](../../referredarea/); وإلا قد تكون القيمة المرتجعة null أو object[] أو كائنًا بسيطًا.

### ملاحظات

فقط للتحقق الذي يكون نوعه List وتم تطبيقه على الخلية المعطاة، وإلا سيتم إرجاع null.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ValidationMethodGetListValueWithInt32Int32Demo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بيانات عينة للتحقق
            worksheet.Cells["A1"].PutValue("Apple");
            worksheet.Cells["A2"].PutValue("Banana");
            worksheet.Cells["A3"].PutValue("Cherry");
            worksheet.Cells["A4"].PutValue("Date");

            // إنشاء تحقق للخلية B1
            Validation validation = worksheet.Cells["B1"].GetValidation();
            validation.Type = ValidationType.List;
            validation.Formula1 = "A1:A4";

            // اختبار GetListValue بمعلمات مختلفة
            Console.WriteLine("List values:");
            for (int i = 0; i < 4; i++)
            {
                object value = validation.GetListValue(i, 0);
                Console.WriteLine($"Index {i}: {value}");
            }

            // تغيير إلى قيم مفصولة بفواصل
            validation.Formula1 = "Red,Green,Blue";
            Console.WriteLine("\nComma-separated values:");
            for (int i = 0; i < 3; i++)
            {
                object[] values = (object[])validation.GetListValue(i, 0);
                Console.WriteLine($"Index {i}: {string.Join(", ", values)}");
            }

            // تغيير إلى قيمة واحدة
            validation.Formula1 = "SingleValue";
            Console.WriteLine("\nSingle value:");
            object singleValue = validation.GetListValue(0, 0);
            Console.WriteLine($"Value: {singleValue}");
        }
    }
}
```

### انظر أيضًا

* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


