---
title: "ConditionalFormattingValueCollection.Item"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ConditionalFormattingValueCollection. احصل على عنصر CFValueObject عند الفهرس المحدد"
type: docs
url: /ar/net/aspose.cells/conditionalformattingvaluecollection/item/
---
## ConditionalFormattingValueCollection indexer

احصل على عنصر CFValueObject في الفهرس المحدد.

```csharp
public ConditionalFormattingValue this[int index] { get; }
```

| معامل | الوصف |
| --- | --- |
| فهرس | الفهرس الذي يبدأ من الصفر للعنصر. |

### قيمة الإرجاع

العنصر عند الفهرس المحدد.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ConditionalFormattingValueCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // أضف بيانات تجريبية
                worksheet.Cells["A1"].PutValue(10);
                worksheet.Cells["A2"].PutValue(120);
                worksheet.Cells["A3"].PutValue(260);

                // إضافة تنسيق شرطي
                int cfIndex = worksheet.ConditionalFormattings.Add();
                FormatConditionCollection fcs = worksheet.ConditionalFormattings[cfIndex];

                // حدد النطاق للتنسيق الشرطي
                CellArea ca = new CellArea
                {
                    StartRow = 0,
                    EndRow = 2,
                    StartColumn = 0,
                    EndColumn = 0
                };
                fcs.AddArea(ca);

                // أضف شرط مجموعة أيقونات
                int conditionIndex = fcs.AddCondition(FormatConditionType.IconSet);
                FormatCondition condition = fcs[conditionIndex];
                IconSet iconSet = condition.IconSet;
                iconSet.Type = IconSetType.Arrows3;

                // احصل على ConditionalFormattingValueCollection
                ConditionalFormattingValueCollection cfvos = iconSet.Cfvos;

                // أضف قيمة إلى المجموعة
                int valueIndex = cfvos.Add(FormatConditionValueType.Number, "50");

                // إظهار الوصول إلى خاصية Item (المؤشر)
                ConditionalFormattingValue cfv = cfvos[valueIndex];

                // عرض القيمة من خاصية Item
                Console.WriteLine($"Conditional Formatting Value at index {valueIndex}:");
                Console.WriteLine($"  Type: {cfv.Type}");
                Console.WriteLine($"  Value: {cfv.Value}");
                Console.WriteLine($"  IsGTE: {cfv.IsGTE}");

                // احفظ المصنف
                workbook.Save("ConditionalFormattingValueCollectionItemDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
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

* class [ConditionalFormattingValue](../../conditionalformattingvalue/)
* class [ConditionalFormattingValueCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


