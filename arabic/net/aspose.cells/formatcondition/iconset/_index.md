---
title: "FormatCondition.IconSet"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية FormatCondition. الحصول على كائن IconSet لتنسيقات الشرط. النوع الافتراضي للنسخة هو IconSetType وهو TrafficLights31. صالح فقط للنوع IconSet"
type: docs
url: /ar/net/aspose.cells/formatcondition/iconset/
---
## FormatCondition.IconSet property

احصل على نسخة "IconSet" من تنسيق الشرطي. نوع IconSetType للنسخة الافتراضية هو TrafficLights31. صالحة فقط للنوع = IconSet.

```csharp
public IconSet IconSet { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormatConditionPropertyIconSetDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // أضف بيانات تجريبية
            for (int i = 0; i < 10; i++)
            {
                sheet.Cells[i, 0].PutValue(i * 10);
            }

            // إضافة تنسيق شرطي
            int index = sheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = sheet.ConditionalFormattings[index];
            
            // تعيين نطاق الخلية
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.EndRow = 9;
            area.StartColumn = 0;
            area.EndColumn = 0;
            fcs.AddArea(area);

            // إضافة شرط وتعيين النوع إلى IconSet
            int conditionIndex = fcs.AddCondition(FormatConditionType.IconSet);
            FormatCondition condition = fcs[conditionIndex];
            
            // الحصول على IconSet وتكوينه
            IconSet iconSet = condition.IconSet;
            iconSet.Type = IconSetType.TrafficLights31;
            iconSet.ShowValue = true;
            iconSet.Reverse = false;

            // احفظ المصنف
            workbook.Save("IconSetDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [IconSet](../../iconset/)
* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


