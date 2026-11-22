---
title: "IconFilter.IconSetType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية IconFilter. تحصل وتعيّن مجموعة الأيقونات المستخدمة لهذا المعيار في الفلتر"
type: docs
url: /ar/net/aspose.cells/iconfilter/iconsettype/
---
## IconFilter.IconSetType property

يحصل ويضبط مجموعة الأيقونات المستخدمة لهذا المعيار.

```csharp
public IconSetType IconSetType { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class IconFilterPropertyIconSetTypeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // ملء بيانات عينة
            for (int i = 0; i < 10; i++)
            {
                worksheet.Cells[i, 0].PutValue(i * 10);
            }

            // إنشاء مرشح تلقائي
            worksheet.AutoFilter.Range = "A1:A10";
            FilterColumn filterColumn = worksheet.AutoFilter.FilterColumns[0];
            filterColumn.FilterType = FilterType.IconFilter;

            // احصل على مرشح الأيقونة
            IconFilter iconFilter = (IconFilter)filterColumn.Filter;

            // عرض IconSetType الحالي (الافتراضي هو None)
            Console.WriteLine("Current IconSetType: " + iconFilter.IconSetType);

            // تعيين مجموعة أيقونات الثلاث أسهم
            iconFilter.IconSetType = IconSetType.Arrows3;
            iconFilter.IconId = 1; // Show only middle arrow

            // تطبيق تنسيق شرطي لتصوير الأيقونات
            ConditionalFormattingCollection conditionalFormattings = worksheet.ConditionalFormattings;
            int index = conditionalFormattings.Add();
            FormatConditionCollection formatConditionCollection = conditionalFormattings[index];
            int conditionIndex = formatConditionCollection.AddCondition(FormatConditionType.IconSet);
            FormatCondition formatCondition = formatConditionCollection[conditionIndex];
            formatCondition.IconSet.Type = IconSetType.Arrows3;
            
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.EndRow = 9;
            area.StartColumn = 0;
            area.EndColumn = 0;
            formatConditionCollection.AddArea(area);

            // تغيير إلى مجموعة أيقونات إشارات المرور
            iconFilter.IconSetType = IconSetType.TrafficLights31;
            iconFilter.IconId = 2; // Show only green light

            // حفظ النتيجة
            workbook.Save("PropertyIconSetTypeDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [IconSetType](../../iconsettype/)
* class [IconFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


