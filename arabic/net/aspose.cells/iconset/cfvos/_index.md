---
title: "IconSet.Cfvos"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية IconSet. احصل على مثيل CFValueObjects"
type: docs
url: /ar/net/aspose.cells/iconset/cfvos/
---
## IconSet.Cfvos property

احصل على مثيل CFValueObjects.

```csharp
public ConditionalFormattingValueCollection Cfvos { get; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class IconSetPropertyCfvosDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بيانات تجريبية
            for (int i = 0; i < 10; i++)
            {
                worksheet.Cells[i, 0].PutValue(i * 10);
            }

            try
            {
                // إضافة تنسيق شرطي
                int cfIndex = worksheet.ConditionalFormattings.Add();
                FormatConditionCollection fcs = worksheet.ConditionalFormattings[cfIndex];

                // تعيين النطاق للتنسيق الشرطي
                CellArea area = new CellArea();
                area.StartRow = 0;
                area.StartColumn = 0;
                area.EndRow = 9;
                area.EndColumn = 0;
                fcs.AddArea(area);

                // إضافة شرط مجموعة الأيقونات
                int conditionIndex = fcs.AddCondition(FormatConditionType.IconSet);
                FormatCondition condition = fcs[conditionIndex];

                // تعيين نوع مجموعة الأيقونات
                condition.IconSet.Type = IconSetType.TrafficLights31;

                // الوصول إلى خاصية Cfvos (للقراءة فقط)
                ConditionalFormattingValueCollection cfvos = condition.IconSet.Cfvos;

                // عرض معلومات حول مجموعة Cfvos
                Console.WriteLine("Number of CFValueObjects in the collection: " + cfvos.Count);

                // التنقل عبر المجموعة وعرض كل قيمة
                for (int i = 0; i < cfvos.Count; i++)
                {
                    ConditionalFormattingValue cfValue = cfvos[i];
                    Console.WriteLine($"CFValue {i + 1}: Type = {cfValue.Type}, Value = {cfValue.Value}");
                }

                // احفظ المصنف
                workbook.Save("IconSetCfvosDemo.xlsx");
                Console.WriteLine("Workbook saved successfully with icon set conditional formatting.");
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

* class [ConditionalFormattingValueCollection](../../conditionalformattingvaluecollection/)
* class [IconSet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


