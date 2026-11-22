---
title: "IconSet.ShowValue"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية IconSet. احصل أو عيّن العلامة التي تشير إلى ما إذا كان يجب إظهار قيم الخلايا التي يُطبق عليها مجموعة الأيقونات هذه. القيمة الافتراضية هي true"
type: docs
url: /ar/net/aspose.cells/iconset/showvalue/
---
## IconSet.ShowValue property

احصل أو عيّن العلامة التي تشير إلى ما إذا كان سيتم إظهار قيم الخلايا التي تم تطبيق مجموعة الأيقونات عليها. القيمة الافتراضية هي true.

```csharp
public bool ShowValue { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class IconSetPropertyShowValueDemo
    {
        public static void Run()
        {
            // إنشاء مصنف
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // أضف بيانات تجريبية
            sheet.Cells["A1"].PutValue(10);
            sheet.Cells["A2"].PutValue(20);
            sheet.Cells["A3"].PutValue(30);
            sheet.Cells["A4"].PutValue(40);
            sheet.Cells["A5"].PutValue(50);

            // إضافة تنسيق شرطي لمجموعة الأيقونات
            int formatIndex = sheet.ConditionalFormattings.Add();
            FormatConditionCollection formatConditions = sheet.ConditionalFormattings[formatIndex];
            int index = formatConditions.AddCondition(FormatConditionType.IconSet);
            FormatCondition condition = formatConditions[index];

            // تعيين خصائص مجموعة الأيقونات
            condition.IconSet.Type = IconSetType.TrafficLights31;
            condition.IconSet.ShowValue = false; // This hides cell values and shows only icons
            condition.IconSet.Reverse = false;

            // تعيين النطاق للتنسيق الشرطي
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.StartColumn = 0;
            area.EndRow = 4;
            area.EndColumn = 0;
            formatConditions.AddArea(area);

            // احفظ المصنف
            workbook.Save("IconSetShowValueDemo.xlsx", SaveFormat.Xlsx);

            Console.WriteLine("Workbook saved with icon set conditional formatting (ShowValue = false).");
        }
    }
}
```

### انظر أيضًا

* class [IconSet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


