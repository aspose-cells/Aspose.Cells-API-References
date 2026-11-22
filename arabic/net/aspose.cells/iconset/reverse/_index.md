---
title: "IconSet.Reverse"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية IconSet. احصل أو عيّن العلامة التي تشير إلى ما إذا كان يجب عكس الترتيب الافتراضي للأيقونات في مجموعة الأيقونات هذه. القيمة الافتراضية هي false"
type: docs
url: /ar/net/aspose.cells/iconset/reverse/
---
## IconSet.Reverse property

احصل أو عيّن العلامة التي تشير إلى ما إذا كان سيتم عكس الترتيب الافتراضي للأيقونات في مجموعة الأيقونات هذه. القيمة الافتراضية هي false.

```csharp
public bool Reverse { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class IconSetPropertyReverseDemo
    {
        public static void Run()
        {
            // إنشاء مصنف
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بيانات تجريبية
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            worksheet.Cells["A4"].PutValue(40);
            worksheet.Cells["A5"].PutValue(50);

            // إضافة تنسيق شرطي
            ConditionalFormattingCollection cfs = worksheet.ConditionalFormattings;
            int index = cfs.Add();
            FormatConditionCollection cf = cfs[index];
            
            // تعيين النطاق
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.EndRow = 4;
            area.StartColumn = 0;
            area.EndColumn = 0;
            cf.AddArea(area);

            // إنشاء تنسيق شرطي لمجموعة الأيقونات
            cf.AddCondition(FormatConditionType.IconSet);
            IconSet iconSet = cf[0].IconSet;
            
            // تكوين مجموعة الأيقونات
            iconSet.Type = IconSetType.Arrows3;
            iconSet.ShowValue = true;
            
            // إظهار خاصية Reverse
            Console.WriteLine("Original IconSet Reverse value: " + iconSet.Reverse);
            iconSet.Reverse = true;
            Console.WriteLine("Modified IconSet Reverse value: " + iconSet.Reverse);

            // احفظ المصنف
            workbook.Save("IconSetPropertyReverseDemo_out.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [IconSet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


