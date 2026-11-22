---
title: "Validation.Value1"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Validation. تمثل القيمة الأولى المرتبطة بالتحقق من البيانات"
type: docs
url: /ar/net/aspose.cells/validation/value1/
---
## Validation.Value1 property

يمثل القيمة الأولى المرتبطة بالتحقق من البيانات.

```csharp
public object Value1 { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ValidationPropertyValue1Demo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء تحقق في الخلية A1
            Validation validation = worksheet.Cells["A1"].GetValidation();
            validation.Type = ValidationType.List;
            
            // تعيين خاصية Value1 بمصفوفة نصية
            validation.Value1 = new object[] { "Option1", "Option2", "Option3" };

            // الحصول على قيم التحقق وعرضها
            object[] values = validation.Value1 as object[];
            Console.WriteLine("Validation values in A1:");
            foreach (object value in values)
            {
                Console.WriteLine(value.ToString());
            }

            // إنشاء تحقق آخر في الخلية B1 بقيم مختلفة
            Validation validation2 = worksheet.Cells["B1"].GetValidation();
            validation2.Type = ValidationType.List;
            validation2.Value1 = new object[] { "Yes", "No", "Maybe" };

            // الحصول على قيم التحقق الثانية وعرضها
            object[] values2 = validation2.Value1 as object[];
            Console.WriteLine("\nValidation values in B1:");
            foreach (object value in values2)
            {
                Console.WriteLine(value.ToString());
            }
        }
    }
}
```

### انظر أيضًا

* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


