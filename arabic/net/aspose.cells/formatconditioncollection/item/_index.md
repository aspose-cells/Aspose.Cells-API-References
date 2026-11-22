---
title: "FormatConditionCollection.Item"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية FormatConditionCollection. يحصل على شرط التنسيق حسب الفهرس"
type: docs
url: /ar/net/aspose.cells/formatconditioncollection/item/
---
## FormatConditionCollection indexer

يحصل على شرط التنسيق حسب الفهرس.

```csharp
public FormatCondition this[int index] { get; }
```

| معامل | الوصف |
| --- | --- |
| فهرس | فهرس شرط التنسيق للإرجاع. |

### قيمة الإرجاع

شرط التنسيق

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormatConditionCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // إضافة مجموعة شرط تنسيق
            int index = sheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = sheet.ConditionalFormattings[index];
            
            // إضافة شرط تنسيق
            fcc.Add(CellArea.CreateCellArea(0, 0, 0, 3),
                FormatConditionType.CellValue, OperatorType.Between, "=A1", "=B1");

            // الوصول إلى أول شرط تنسيق باستخدام خاصية Item
            FormatCondition condition = fcc[0];
            
            // عرض الصيغ
            Console.WriteLine("Formula1: " + condition.Formula1);
            Console.WriteLine("Formula2: " + condition.Formula2);
            
            // تعديل الصيغ باستخدام خاصية Item
            fcc[0].Formula1 = "=C1";
            fcc[0].Formula2 = "=D1";
            
            // عرض الصيغ المعدلة
            Console.WriteLine("Modified Formula1: " + fcc[0].Formula1);
            Console.WriteLine("Modified Formula2: " + fcc[0].Formula2);
        }
    }
}
```

### انظر أيضًا

* class [FormatCondition](../../formatcondition/)
* class [FormatConditionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


