---
title: "IconFilter.IconId"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية IconFilter. تحصل وتعيّن الفهرس الصفري لرمز في مجموعة الأيقونات"
type: docs
url: /ar/net/aspose.cells/iconfilter/iconid/
---
## IconFilter.IconId property

يحصل ويضبط الفهرس الصفري لرمز في مجموعة الأيقونات.

```csharp
public int IconId { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class IconFilterPropertyIconIdDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // ملء بيانات عينة
            for (int i = 0; i < 10; i++)
            {
                worksheet.Cells[i, 0].PutValue(i + 1);
            }

            // تطبيق تنسيق شرطي لمجموعة الأيقونات
            ConditionalFormattingCollection conditionalFormattings = worksheet.ConditionalFormattings;
            int index = conditionalFormattings.Add();
            FormatConditionCollection formatConditionCollection = conditionalFormattings[index];
            int conditionIndex = formatConditionCollection.AddCondition(FormatConditionType.IconSet);
            FormatCondition formatCondition = formatConditionCollection[conditionIndex];
            formatCondition.IconSet.Type = IconSetType.TrafficLights31;
            
            // تعيين النطاق باستخدام CellArea
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.EndRow = 9;
            area.StartColumn = 0;
            area.EndColumn = 0;
            formatConditionCollection.AddArea(area);

            // إنشاء مرشح تلقائي مع مرشح الأيقونات
            worksheet.AutoFilter.Range = "A1:A10";
            FilterColumn filterColumn = worksheet.AutoFilter.FilterColumns[0];
            filterColumn.FilterType = FilterType.IconFilter;
            
            // الحصول على المرشح الموجود بدلاً من إنشاء نسخة جديدة
            IconFilter iconFilter = (IconFilter)filterColumn.Filter;
            iconFilter.IconSetType = IconSetType.TrafficLights31;
            iconFilter.IconId = 0;

            Console.WriteLine("Current IconId value: " + iconFilter.IconId);

            // تعديل IconId لتصفية أيقونات مختلفة
            iconFilter.IconId = 1;

            workbook.Save("PropertyIconIdDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [IconFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


