---
title: "Validation.GetValue"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Validation. احصل على قيمة التحقق في الخلية المحددة"
type: docs
url: /ar/net/aspose.cells/validation/getvalue/
---
## Validation.GetValue method

احصل على قيمة التحقق على الخلية المحددة.

```csharp
public object GetValue(int row, int column, bool isValue1)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| صف | Int32 | فهرس الصف. |
| عمود | Int32 | فهرس العمود. |
| isValue1 | منطقي | يشير إلى ما إذا كان يتم الحصول على القيمة الأولى. |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ValidationMethodGetValueWithInt32Int32BooleanDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إضافة بيانات نموذجية والتحقق
            worksheet.Cells["A1"].PutValue("Select Item:");
            worksheet.Cells["B1"].PutValue("Item 1");
            worksheet.Cells["B2"].PutValue("Item 2");
            
            // إنشاء تحقق للخلية B1
            Validation validation = worksheet.Cells["B1"].GetValidation();
            validation.Type = ValidationType.List;
            validation.Formula1 = "A1:B2";
            
            // احصل على القيمة باستخدام طريقة GetValue مع الصف والعمود وتحويل القيم الرقمية إلى تاريخ
            object value = validation.GetValue(0, 1, false);
            
            // أخرج النتيجة.
            Console.WriteLine("Validation value: " + value.ToString());
        }
    }
}
```

### انظر أيضًا

* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


