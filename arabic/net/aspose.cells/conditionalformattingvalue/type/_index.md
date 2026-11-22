---
title: "ConditionalFormattingValue.Type"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ConditionalFormattingValue. احصل أو عيّن نوع كائن قيمة التنسيق الشرطي هذا. ضبط النوع إلى FormatConditionValueType.Min أو FormatConditionValueType.Max سيضبط Value تلقائيًا إلى null"
type: docs
url: /ar/net/aspose.cells/conditionalformattingvalue/type/
---
## ConditionalFormattingValue.Type property

احصل على أو اضبط نوع كائن قيمة التنسيق الشرطي هذا. ضبط النوع إلى FormatConditionValueType.Min أو FormatConditionValueType.Max سيؤدي تلقائيًا إلى تعيين \"Value\" إلى null.

```csharp
public FormatConditionValueType Type { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ConditionalFormattingValuePropertyTypeDemo
    {
        public static void Run()
        {
            try
            {
                // إنشاء دفتر عمل جديد
                Workbook workbook = new Workbook();
                Worksheet ws = workbook.Worksheets[0];

                // أضف بعض البيانات النموذجية (مطلوبة لوجود التنسيق الشرطي)
                ws.Cells["A1"].PutValue(10);
                ws.Cells["A2"].PutValue(20);
                ws.Cells["A3"].PutValue(30);

                // إنشاء مجموعة تنسيق شرطي وإضافة شرط IconSet
                int cfIndex = ws.ConditionalFormattings.Add();
                FormatConditionCollection fcc = ws.ConditionalFormattings[cfIndex];

                int condIdx = fcc.AddCondition(FormatConditionType.IconSet);
                FormatCondition condition = fcc[condIdx];
                condition.IconSet.Type = IconSetType.Arrows3; // any valid icon set type

                // الحصول على مثيل ConditionalFormattingValue من مجموعة IconSet
                ConditionalFormattingValue cfv = condition.IconSet.Cfvos[0];

                // عيّن Type إلى Percent وخصص قيمة مطابقة
                cfv.Type = FormatConditionValueType.Percent;
                cfv.Value = 25; // 25%

                // قراءة وعرض Type و Value
                Console.WriteLine("After setting Type to Percent:");
                Console.WriteLine("  Type : " + cfv.Type);
                Console.WriteLine("  Value: " + cfv.Value);

                // غيّر Type إلى Min – وفقًا للتوثيق سيؤدي ذلك إلى إلغاء Value
                cfv.Type = FormatConditionValueType.Min;

                // قراءة وعرض Type و Value مرة أخرى
                Console.WriteLine("\nAfter setting Type to Min:");
                Console.WriteLine("  Type : " + cfv.Type);
                Console.WriteLine("  Value: " + (cfv.Value == null ? "null" : cfv.Value.ToString()));

                // احفظ المصنف (التنسيق الشرطي جزء من الورقة)
                workbook.Save("ConditionalFormattingValueTypeDemo.xlsx");
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

* enum [FormatConditionValueType](../../formatconditionvaluetype/)
* class [ConditionalFormattingValue](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


