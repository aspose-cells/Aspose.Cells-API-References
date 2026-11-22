---
title: "IconSet.IsCustom"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية IconSet. تشير إلى ما إذا كانت مجموعة الأيقونات مخصصة. القيمة الافتراضية هي false"
type: docs
url: /ar/net/aspose.cells/iconset/iscustom/
---
## IconSet.IsCustom property

يشير إلى ما إذا كانت مجموعة الأيقونات مخصصة. القيمة الافتراضية هي false.

```csharp
public bool IsCustom { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class IconSetPropertyIsCustomDemo
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

            // إضافة تنسيق شرطي باستخدام مجموعة أيقونات مخصصة
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];
            
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
            
            // تعيين نوع مجموعة الأيقونات (باستخدام IconSetType صالح)
            condition.IconSet.Type = IconSetType.TrafficLights31;

            // تحقق من خاصية IsCustom (للقراءة فقط)
            Console.WriteLine("Is IconSet custom? " + condition.IconSet.IsCustom);

            // احفظ المصنف
            workbook.Save("output.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [IconSet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


