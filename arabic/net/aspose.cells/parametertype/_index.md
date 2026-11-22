---
title: "تعداد ParameterType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "تعداد Aspose.Cells.ParameterType. يمثل جميع أنواع المعلمات أو نوع قيمة الإرجاع للدالة"
type: docs
url: /ar/net/aspose.cells/parametertype/
---
## ParameterType enumeration

يمثل نوع جميع المعلمات أو نوع قيمة الإرجاع للدالة.

```csharp
public enum ParameterType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| Reference | `0` |  |
| Value | `1` |  |
| Array | `2` |  |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ParameterTypeDemo
    {
        public static void ParameterTypeExample()
        {
            // إنشاء مصنف وورقة عمل لتوضيح الاستخدام
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // مثال على استخدام تعداد ParameterType في دالة صيغة
            // لنفترض أننا نقوم بتعريف دالة مخصصة بأنواع معلمات محددة

            // تعريف مصفوفة من أنواع المعلمات
            ParameterType[] parameterTypes = new ParameterType[]
            {
                ParameterType.Reference,
                ParameterType.Value,
                ParameterType.Array
            };

            // دالة مثال تستخدم هذه الأنواع من المعلمات
            // على سبيل المثال، تعيين دالة مخصصة افتراضية بأنواع معلمات محددة
            // (ملاحظة: معالجة الدوال المخصصة ستعتمد على قدرات واجهة برمجة تطبيقات Aspose.Cells)

            // حفظ المصنف لتوضيح التغييرات
            workbook.Save("ParameterTypeExample.xlsx");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


