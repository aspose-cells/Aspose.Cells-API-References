---
title: "ConditionalFormattingValue.Value"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ConditionalFormattingValue. احصل أو عيّن قيمة كائن قيمة التنسيق الشرطي هذا. يجب استخدامها بالاشتراك مع Type"
type: docs
url: /ar/net/aspose.cells/conditionalformattingvalue/value/
---
## ConditionalFormattingValue.Value property

احصل على أو اضبط قيمة كائن قيمة التنسيق الشرطي هذا. يجب استخدامه بالتزامن مع Type.

```csharp
public object Value { get; set; }
```

### ملاحظات

إذا كانت القيمة سلسلة وتبدأ بـ "=", فستُعالج كصيغة، وإلا سنعالجها كقيمة بسيطة.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ConditionalFormattingValuePropertyValueDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بيانات تجريبية
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            worksheet.Cells["A4"].PutValue(40);

            // إضافة تنسيق شرطي
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = worksheet.ConditionalFormattings[index];
            
            // إنشاء تنسيق شرطي لمجموعة الأيقونات
            int conditionIndex = fcc.AddCondition(FormatConditionType.IconSet);
            FormatCondition condition = fcc[conditionIndex];
            condition.IconSet.Type = IconSetType.Arrows3;

            // احصل على كائنات قيم التنسيق الشرطي
            ConditionalFormattingValueCollection cfvos = condition.IconSet.Cfvos;

            // عيّن القيم للأيقونات
            cfvos[0].Type = FormatConditionValueType.Min;
            cfvos[0].Value = 0;
            
            cfvos[1].Type = FormatConditionValueType.Percent;
            cfvos[1].Value = 33;
            
            cfvos[2].Type = FormatConditionValueType.Percent;
            cfvos[2].Value = 67;

            // عرض كيفية استخدام خاصية Value
            Console.WriteLine("First icon value: " + cfvos[0].Value);
            Console.WriteLine("Second icon value: " + cfvos[1].Value);
            Console.WriteLine("Third icon value: " + cfvos[2].Value);

            // احفظ المصنف
            workbook.Save("output.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ConditionalFormattingValue](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


