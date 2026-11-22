---
title: "تعداد OperatorType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "تعداد Aspose.Cells.OperatorType. يمثل نوع المشغل للتنسيق الشرطي والتحقق من صحة البيانات"
type: docs
url: /ar/net/aspose.cells/operatortype/
---
## OperatorType enumeration

يمثل نوع المشغل للتنسيق الشرطي والتحقق من صحة البيانات.

```csharp
public enum OperatorType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| Between | `0` | يمثل المشغل Between للتنسيق الشرطي والتحقق من صحة البيانات. |
| Equal | `1` | يمثل المشغل Equal للتنسيق الشرطي والتحقق من صحة البيانات. |
| GreaterThan | `2` | يمثل المشغل GreaterThan للتنسيق الشرطي والتحقق من صحة البيانات. |
| GreaterOrEqual | `3` | يمثل المشغل GreaterOrEqual للتنسيق الشرطي والتحقق من صحة البيانات. |
| LessThan | `4` | يمثل المشغل LessThan للتنسيق الشرطي والتحقق من صحة البيانات. |
| LessOrEqual | `5` | يمثل المشغل LessOrEqual للتنسيق الشرطي والتحقق من صحة البيانات. |
| None | `6` | يمثل عدم وجود مقارنة. |
| NotBetween | `7` | يمثل المشغل NotBetween للتنسيق الشرطي والتحقق من صحة البيانات. |
| NotEqual | `8` | يمثل المشغل NotEqual للتنسيق الشرطي والتحقق من صحة البيانات. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class OperatorTypeDemo
    {
        public static void OperatorTypeExample()
        {
            // إنشاء مصنف جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة تنسيق شرطي فارغ
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];

            // تحديد نطاق التنسيق الشرطي
            CellArea ca = new CellArea { StartRow = 0, EndRow = 10, StartColumn = 0, EndColumn = 10 };
            fcs.AddArea(ca);

            // إضافة شرط باستخدام OperatorType.Between
            int conditionIndex = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "=A1", "100");
            FormatCondition fc = fcs[conditionIndex];
            fc.Style.BackgroundColor = System.Drawing.Color.Yellow;

            // إضافة شرط آخر باستخدام OperatorType.GreaterThan
            int conditionIndex2 = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.GreaterThan, "50", null);
            FormatCondition fc2 = fcs[conditionIndex2];
            fc2.Style.BackgroundColor = System.Drawing.Color.Green;

            // احفظ المصنف
            workbook.Save("OperatorTypeExample.xlsx");

            return;
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


