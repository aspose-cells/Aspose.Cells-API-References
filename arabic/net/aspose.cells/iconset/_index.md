---
title: "الفئة IconSet"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.IconSet. صِف قاعدة تنسيق الخلايا الشرطي IconSet. تُطبق قاعدة تنسيق الخلايا الشرطي هذه أيقونات على الخلايا وفقًا لقيمها"
type: docs
url: /ar/net/aspose.cells/iconset/
---
## IconSet class

وصف قاعدة تنسيق شرطي لمجموعة الأيقونات. يطبق هذا التنسيق الشرطي أيقونات على الخلايا وفقًا لقيمها.

```csharp
public class IconSet
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [CfIcons](../../aspose.cells/iconset/cficons/) { get; } | احصل على [`ConditionalFormattingIcon`](../conditionalformattingicon/) من المجموعة |
| [Cfvos](../../aspose.cells/iconset/cfvos/) { get; } | احصل على مثيل CFValueObjects. |
| [IsCustom](../../aspose.cells/iconset/iscustom/) { get; } | يشير إلى ما إذا كانت مجموعة الأيقونات مخصصة. القيمة الافتراضية هي false. |
| [Reverse](../../aspose.cells/iconset/reverse/) { get; set; } | احصل أو عيّن العلامة التي تشير إلى ما إذا كان سيتم عكس الترتيب الافتراضي للأيقونات في مجموعة الأيقونات هذه. القيمة الافتراضية هي false. |
| [ShowValue](../../aspose.cells/iconset/showvalue/) { get; set; } | احصل أو عيّن العلامة التي تشير إلى ما إذا كان سيتم إظهار قيم الخلايا التي تم تطبيق مجموعة الأيقونات عليها. القيمة الافتراضية هي true. |
| [Type](../../aspose.cells/iconset/type/) { get; set; } | احصل أو عيّن نوع مجموعة الأيقونات للعرض. سيقوم تعيين النوع بالتحقق تلقائيًا مما إذا كان عدد Cfvos الحالي يتوافق مع النوع الجديد. إذا لم يتوافق، سيتم مسح Cfvos القديمة وإضافة Cfvos الافتراضية. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class IconSetDemo
    {
        public static void IconSetExample()
        {
            // إنشاء كائن Workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // يضيف تنسيقًا شرطيًا فارغًا
            int index = sheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = sheet.ConditionalFormattings[index];

            // يضبط نطاق التنسيق الشرطي
            CellArea ca = new CellArea
            {
                StartRow = 0,
                EndRow = 2,
                StartColumn = 0,
                EndColumn = 0
            };
            fcs.AddArea(ca);

            // يضيف شرطًا
            int idx = fcs.AddCondition(FormatConditionType.IconSet);
            FormatCondition cond = fcs[idx];

            // احصل على مجموعة الأيقونات
            IconSet iconSet = cond.IconSet;

            // عيّن نوع الأيقونة
            iconSet.Type = IconSetType.Arrows3;

            // عيّن الخصائص الإضافية
            iconSet.ShowValue = true;
            iconSet.Reverse = false;

            // ضع قيم الخلايا
            sheet.Cells["A1"].PutValue(10);
            sheet.Cells["A2"].PutValue(120);
            sheet.Cells["A3"].PutValue(260);

            // حفظ ملف Excel
            workbook.Save("IconSetExample.xlsx");
            workbook.Save("IconSetExample.pdf");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


