---
title: "FormatCondition.Priority"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية FormatCondition. أولوية قاعدة التنسيق الشرطي هذه. تُستخدم هذه القيمة لتحديد أي تنسيق يجب تقييمه وعرضه. القيم الرقمية الأقل لها أولوية أعلى من القيم الأعلى، حيث 1 هي أعلى أولوية"
type: docs
url: /ar/net/aspose.cells/formatcondition/priority/
---
## FormatCondition.Priority property

أولوية قاعدة التنسيق الشرطي هذه. تُستخدم هذه القيمة لتحديد أي تنسيق يجب تقييمه وعرضه. القيم الرقمية الأقل لها أولوية أعلى من القيم الرقمية الأعلى، حيث أن '1' هي أعلى أولوية.

```csharp
public int Priority { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormatConditionPropertyPriorityDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // أضف بيانات تجريبية
            for (int i = 0; i < 10; i++)
            {
                sheet.Cells[i, 0].PutValue(i + 1);
            }

            // إضافة تنسيق شرطي
            int formatIndex = sheet.ConditionalFormattings.Add();
            FormatConditionCollection formatConditions = sheet.ConditionalFormattings[formatIndex];
            
            // إضافة شروط
            int conditionIndex1 = formatConditions.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "2", "5");
            int conditionIndex2 = formatConditions.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "6", "9");

            // تعيين الأولويات
            formatConditions[conditionIndex1].Priority = 2;
            formatConditions[conditionIndex2].Priority = 1;

            // عرض استخدام خاصية Priority
            Console.WriteLine("Condition 1 Priority: " + formatConditions[conditionIndex1].Priority);
            Console.WriteLine("Condition 2 Priority: " + formatConditions[conditionIndex2].Priority);

            // احفظ المصنف
            workbook.Save("ConditionalFormattingPriorityDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


