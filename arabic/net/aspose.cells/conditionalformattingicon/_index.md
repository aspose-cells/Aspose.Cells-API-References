---
title: "الفئة ConditionalFormattingIcon"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.ConditionalFormattingIcon. تمثل الأيقونة المخصصة لقاعدة تنسيق الخلايا الشرطي"
type: docs
url: /ar/net/aspose.cells/conditionalformattingicon/
---
## ConditionalFormattingIcon class

يمثل الأيقونة المخصصة لقاعدة تنسيق الخلايا الشرطي.

```csharp
public class ConditionalFormattingIcon
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [ImageData](../../aspose.cells/conditionalformattingicon/imagedata/) { get; } | يحصل على بيانات مجموعة الأيقونات. |
| [Index](../../aspose.cells/conditionalformattingicon/index/) { get; set; } | يحصل ويعيّن فهرس الأيقونة في مجموعة الأيقونات. |
| [Type](../../aspose.cells/conditionalformattingicon/type/) { get; set; } | يحصل ويعيّن نوع مجموعة الأيقونات. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [GetImageData](../../aspose.cells/conditionalformattingicon/getimagedata/)(Cell) | يحصل على بيانات الصورة مع إعداد الخلية. |
| static [GetIconImageData](../../aspose.cells/conditionalformattingicon/geticonimagedata/)(IconSetType, int) | احصل على بيانات مجموعة الأيقونات |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ConditionalFormattingIconDemo
    {
        public static void ConditionalFormattingIconExample()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى في المصنف
            Worksheet worksheet = workbook.Worksheets[0];
            
            // احصل على مجموعة تنسيقات الخلايا الشرطية
            ConditionalFormattingCollection cformattings = worksheet.ConditionalFormattings;
            
            // أضف تنسيقًا شرطيًا جديدًا إلى المجموعة
            int index = cformattings.Add();
            
            // الوصول إلى مجموعة شروط التنسيق
            FormatConditionCollection fcs = cformattings[index];
            
            // حدد نطاق الخلايا لتطبيق التنسيق الشرطي
            CellArea ca = new CellArea
            {
                StartRow = 0,
                EndRow = 10,
                StartColumn = 0,
                EndColumn = 0
            };
            
            // أضف نطاق الخلايا إلى مجموعة شروط التنسيق
            fcs.AddArea(ca);
            
            // أضف شرطًا لاستخدام مجموعات الأيقونات
            int conditionIndex = fcs.AddCondition(FormatConditionType.IconSet);
            FormatCondition fc = fcs[conditionIndex];
            
            // حدد نوع مجموعة الأيقونات
            fc.IconSet.Type = IconSetType.Arrows3;

            // خصّص الأيقونات الفردية داخل مجموعة الأيقونات
            ConditionalFormattingIcon cfIcon0 = fc.IconSet.CfIcons[0];
            cfIcon0.Type = IconSetType.Arrows3;
            cfIcon0.Index = 0;

            ConditionalFormattingIcon cfIcon1 = fc.IconSet.CfIcons[1];
            cfIcon1.Type = IconSetType.ArrowsGray3;
            cfIcon1.Index = 1;

            ConditionalFormattingIcon cfIcon2 = fc.IconSet.CfIcons[2];
            cfIcon2.Type = IconSetType.Boxes5;
            cfIcon2.Index = 2;

            // احفظ المصنف
            workbook.Save("ConditionalFormattingIconExample.xlsx");
            workbook.Save("ConditionalFormattingIconExample.pdf");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


